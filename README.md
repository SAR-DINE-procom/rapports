-------------------------------------------------------------------------------------
                         INSTITUT MINES-TELECOM, IMT ATlantique
                    Département Mathematical & Electrical Engineering
                              Technopôle de Brest-Iroise
                             CS 83818 - 29238 BREST Cedex 3     
-------------------------------------------------------------------------------------

Modèle de document LaTeX IMT Atlantique pour la rédaction de rapports de recherche
(validé par la DRI) ou des supports de cours et TP, *.tex (v2.3), *.sty (v3.9)

Maintenu par : Thierry LE GALL (poste 1378) - thierry.legall1@imt-atlantique.fr

-------------------------------------------------------------------------------------
1- Description du modèle:
-------------------------------------------------------------------------------------
lab_006
-------
|
|-ico : < ressources iconographiques (chartes, logos, ect..) utilisées par le modèle (*.pdf, *.png)
|  |
|  |-imta_logo.pdf : logo de l'IMT Atlantique (1ere et 4eme de couverture)
|  |
|  |-imta_map.png : carte des partenariats et implantations IMT Atlantique (4eme de couverture)
|  |
|  |-facebook.png : icône de réseau social IMT Atlantique (4eme de couverture)
|  |
|  |-instagram.png : icône de réseau social IMT Atlantique (4eme de couverture)
|  |
|  |-linkedin.png : icône de réseau social IMT Atlantique (4eme de couverture)
|  |
|  |-youtube.png : icône de réseau social IMT Atlantique (4eme de couverture)
|  |
|  |-imta_triangles.pdf : figure de style du service de la com. (1ere de couverture)
|
|
|-img : < figures, images du corps du document (résultats de simulation, etc...) (*.jpg, *.png) >
|  |
|  |-structure_trame_tx.jpg : exemple de figure au format (*.jpg) intégrée (au corps du document)
|  |
|  |-structure_trame_tx.png : exemple de figure au format (*.png) intégrée (au corps du document)
|  
|
|-src : < fichiers sources (*.tex) et produits de compilation LaTeX (*.pdf, *.aux, etc...)
|  |
|  |-tp_latex_lab_006.tex : fichier source (*.tex) du modèle (éditable et modifiable)
|
|
|-sty : < fichiers de style particuliers associés au modèle IMT Atlantique (*.sty) >
|  |
|  |-imta.sty : fichier de style du modèle de document IMT Atlantique (n'a pas besoin d'être édité)
|  |
|  |-awesomebox.sty : fichier de style pour les icônes de signalement de paragraphes (corps du document)

-------------------------------------------------------------------------------------
2- Utilisation du modèle:
-------------------------------------------------------------------------------------
2.1 décompresser localement l'archive (*.zip)
2.2 ouvrir le fichier tp_latex_lab_006.tex dans un éditeur LaTeX
2.3 sauvegarder le fichier tp_latex_lab_006.tex sous un nouveau nom (*.tex)
    au même emplacement dans le sous-répertoire "src"
2.4 compiler le fichier enregistré (Ctrl +F7 dans TeXnicCenter)
2.5 visualiser le *.pdf obtenu (F5 dans dans TeXnicCenter)

3- Résolution des problèmes de compilation:

Le modèle "tp_latex_lab_006.tex" est validé en édition LaTeX to PDF dans les environnements
suivants :

- TeXnicCenter 2.02 (stable) + compilateur MiKTeX 2.9.6888 / Windows 7 ou Windows 10 (x64)
- TeXstudio 2.12.10 + compilateur MiKTeX 2.9.6888 / Window 7 ou 10 (x64)
- TeXstudio 2.12.6 / UBUNTU 18.04 LTS
- TeXstudio 4.2.1 / UBUNTU 22.04.3 LTS

Toutefois, des erreurs de compilation peuvent intervenir à la première utlisation
du modèle sur une machine dont le compilateur MikTeK (Windows) ou TeXlive (Unix)
ne dispose pas initialement de tous les styles requis (packages manquants).

-------------------------------------------------------------------------------------
Résolution des erreurs de compilation (droits d'administrateurs requis) :
-------------------------------------------------------------------------------------
/Windows :

- Lancer l'application "MiKTeX Console" en mode administrateur
- Overview -> Check for Updates (mise à jour du conpilateur)
- Packages -> Identifier les packages manquants (message d'erreur de compilation) et les installer

/UBUNTU 18.04, 20.04, 22.04.3 LTS - Ouvrir un Terminal (crtl+alt+t)

~$ sudo apt-get update (verifie les mises à jour disponibles pour l'OS)
~$ sudo apt-get upgrade (installe les mises à jour disponibles pour l'OS)

~$ sudo apt-cache search texlive (identifie les packages disponibles de texlive)

~$ sudo apt-get install texlive-lang-french (résolution de : 'newtxtext.sty' not found)
~$ sudo apt-get install texlive-fonts-extra (résolution de : 'babel.sty' Package label error)



 
