# Rapports – Projet PROCOM SAR'DINE

## Démarrer le projet
1. Se connecter avec le **SSO IMT Atlantique** sur Overleaf.  
2. Lier son compte **Overleaf** avec son compte **GitHub**.  
3. Vous avez reçu une invitation par mail pour rejoindre le projet **« rapports »** sur Overleaf.  (https://www.overleaf.com/2259418269vhznjjzsvbgg#9a2f5f) 

## Bonnes pratiques
- Après modification du code sur Overleaf, **synchroniser** avec GitHub :  
  `Menu → GitHub → Push`.
- Débutez votre message de commit avec votre nom :  
  `[Maxence] Rédaction de la première partie de l'introduction`. 

## Créer un nouveau rapport

### Sur GitHub
1. Aller dans le dépôt **`SAR-DINE-procom/rapports`**.  
2. Ouvrir l’onglet **Actions** → **New report scaffolding**.  
3. Cliquer sur **Run workflow**.  
   - Entrer un nom de dossier de rapport (**sans espace**, ex : `biblio_sar`).  

Le workflow lance un script Bash qui crée la structure du rapport et pousse les modifications sur le dépôt.  
⏱️ Durée : moins de 10 secondes.  

👉 La base de votre nouveau rapport sera disponible dans `src/<nom_du_rapport>`.

### Sur Overleaf
1. Aller dans le projet **« rapports »** (lié à GitHub).  
2. Menu → GitHub (Sync menu).  
3. Cliquer sur **Pull GitHub changes into Overleaf**.  

Vous pouvez à présent éditer le rapport de manière collaborative sur Overleaf.  

## Changer le rapport compilé dans Overleaf
- Menu → **Main document** : choisir le `main.tex` du dossier correspondant au rapport que vous voulez compiler.

## Compiler tous les rapports du dépôt dans GitHub
1. Aller dans le dépôt **`SAR-DINE-procom/rapports`**.
2. Ouvrir l'onglet **Actions** → **Build LaTeX Projects**.
3. Cliquer sur **Run workflow**.

Le workflow lance un script qui va récupérer une image docker pour compiler les projets LaTex, la compilation de tout le dépôt dure environ 2 minutes. Une fois le workflow complété, cliquez sur son titre et vous trouverez dans l'onglet summary un artifact appelé latex-pdfs qui comprend tous les rapports PDF. Cliquez dessus et le téléchargement de l'archive commencera.
