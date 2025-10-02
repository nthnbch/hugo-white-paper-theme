# 🚀 Setup GitHub Repository

Ton thème est prêt à être publié ! Voici les étapes à suivre :

## ✅ Déjà fait :
- ✅ Git repo initialisé
- ✅ Commit initial créé (65 fichiers)
- ✅ Branche renommée en `main`
- ✅ Tag v1.0.0 créé

## 📋 Étapes à suivre :

### 1. Créer le repo sur GitHub

**Option A - Via l'interface web (recommandé):**

1. Va sur https://github.com/new
2. Remplis comme suit :
   - **Repository name:** `hugo-white-paper-theme`
   - **Description:** `A clean, modern Hugo theme featuring Fraktur typography and Material Design principles`
   - **Public** ✅ (obligatoire pour Hugo themes)
   - **NE COCHE PAS** "Add a README file" ❌
   - **NE COCHE PAS** "Add .gitignore" ❌
   - **NE COCHE PAS** "Choose a license" ❌
3. Clique sur "Create repository"

**Option B - Via terminal (si tu as gh CLI):**

```bash
gh repo create hugo-white-paper-theme --public --source=. --remote=origin --push
```

### 2. Pusher le thème (après création du repo)

Une fois le repo créé sur GitHub, exécute ces commandes :

```bash
# Depuis ce dossier (tu y es déjà)
cd /Users/bubu/Documents/GitHub/nathanswiss/themes/hugo-white-paper-theme

# Ajouter le remote
git remote add origin https://github.com/nthnbch/hugo-white-paper-theme.git

# Pusher le code
git push -u origin main

# Pusher le tag
git push origin v1.0.0
```

### 3. Vérifier que tout est en ligne

Va sur https://github.com/nthnbch/hugo-white-paper-theme et vérifie :
- ✅ Tous les fichiers sont là
- ✅ Le README s'affiche correctement
- ✅ Le tag v1.0.0 apparaît dans "Releases"

### 4. Créer une Release GitHub (optionnel mais recommandé)

1. Sur ton repo, va dans "Releases" → "Create a new release"
2. Choisis le tag `v1.0.0`
3. Title: `v1.0.0 - Initial Release`
4. Description: Copie le contenu de CHANGELOG.md
5. Publie la release

## 🔄 Ensuite : Convertir ton site principal en submodule

Une fois le repo créé et poussé, retourne dans ton repo principal :

```bash
# Retour au repo nathanswiss
cd /Users/bubu/Documents/GitHub/nathanswiss

# Sauvegarder le thème actuel (au cas où)
mv themes/hugo-white-paper-theme themes/hugo-white-paper-theme.backup

# Ajouter le thème comme submodule
git submodule add https://github.com/nthnbch/hugo-white-paper-theme.git themes/hugo-white-paper-theme

# Commit le changement
git add .
git commit -m "Convert theme to git submodule"
git push
```

## 🎉 Soumettre à Hugo Themes

Une fois tout ça fait :

1. Fork https://github.com/gohugoio/hugoThemes
2. Édite le fichier `config.yaml`
3. Ajoute cette ligne dans la liste des thèmes :
   ```yaml
   - https://github.com/nthnbch/hugo-white-paper-theme.git
   ```
4. Commit et crée une Pull Request
5. Attends la review de l'équipe Hugo

## 📝 Notes

- **Repo URL:** https://github.com/nthnbch/hugo-white-paper-theme
- **Demo URL:** https://nathan.swiss
- **License:** MIT
- **Version:** 1.0.0

---

**Besoin d'aide ?** N'hésite pas à demander !
