# Ali Chams Eddine — Portfolio

Portfolio immersif et artistique de **Ali Chams Eddine**, Sound Designer, Compositeur et Chercheur en Anthropologie du Son (Grand Tunis, Tunisie).

---

## 🚀 Guide de démarrage sur Ubuntu

### 1. Prérequis sur Ubuntu
Assurez-vous que **Node.js** (version 18 ou supérieure) et **npm** sont installés :
```bash
sudo apt update
sudo apt install nodejs npm -y
node -v
npm -v
```

---

### 2. Installation et Lancement local

```bash
# 1. Cloner le projet depuis GitHub (ou naviguer dans le dossier)
git clone https://github.com/VOTRE_NOM_UTILISATEUR/VOTRE_DEPOT.git
cd VOTRE_DEPOT

# 2. Installer les dépendances
npm install

# 3. Lancer le serveur de développement local
npm run dev
```
Le site s'ouvre sur `http://localhost:3000` (ou le port affiché dans le terminal).

---

### 3. Compilation pour la Production

Pour générer les fichiers finaux prêts pour le web :
```bash
npm run build
```
Tous les fichiers statiques optimisés (HTML, CSS, JavaScript, images et assets audio) sont générés dans le dossier **`dist/`**.

---

### 4. Déploiement sur GitHub Pages (Automatique)

Le projet inclut déjà une action GitHub automatique (`.github/workflows/deploy.yml`).

Pour activer le déploiement automatique sur GitHub :
1. Poussez votre code sur GitHub :
   ```bash
   git add .
   git commit -m "Déploiement initial du portfolio"
   git branch -M main
   git push -u origin main
   ```
2. Rendez-vous sur votre dépôt GitHub dans votre navigateur.
3. Cliquez sur **Settings** > **Pages** (dans le menu de gauche).
4. Dans la section **Build and deployment** > **Source**, sélectionnez **GitHub Actions**.
5. Votre site sera automatiquement compilé et mis en ligne avec une adresse du type :  
   `https://<votre-nom-d-utilisateur>.github.io/<nom-du-depot>/`

---

### 5. Déploiement sur Vercel ou Netlify (Alternative en 1 clic)

Vous pouvez également connecter ce dépôt GitHub à **[Vercel](https://vercel.com)** ou **[Netlify](https://netlify.com)** :
- **Build command** : `npm run build`
- **Output directory** : `dist`
- Déploiement automatique avec certificat SSL HTTPS gratuit.
