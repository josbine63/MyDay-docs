# MyDay - Documentation Website

Site web de documentation pour l'application iOS MyDay.

## 🚀 Déploiement sur GitHub Pages

### Étape 1 : Créer un dépôt GitHub

1. Va sur [GitHub](https://github.com) et connecte-toi
2. Clique sur le bouton "New" pour créer un nouveau dépôt
3. Nomme le dépôt (par exemple: `myday-docs` ou `myday-website`)
4. Rends-le public
5. Ne coche PAS "Initialize this repository with a README"
6. Clique sur "Create repository"

### Étape 2 : Upload les fichiers

Tu as deux options :

#### Option A : Via l'interface GitHub (plus simple)
1. Sur la page de ton nouveau dépôt, clique sur "uploading an existing file"
2. Glisse-dépose les fichiers : `index.html`, `styles.css`, `script.js`
3. Ajoute un message de commit (ex: "Initial commit")
4. Clique sur "Commit changes"

#### Option B : Via la ligne de commande
```bash
# Initialise le dépôt local
git init
git add index.html styles.css script.js README.md

# Commit les fichiers
git commit -m "Initial commit"

# Lie ton dépôt local au dépôt GitHub
git branch -M main
git remote add origin https://github.com/TON_USERNAME/TON_REPO.git
git push -u origin main
```

### Étape 3 : Activer GitHub Pages

1. Va dans les "Settings" de ton dépôt
2. Clique sur "Pages" dans le menu de gauche
3. Sous "Source", sélectionne "Deploy from a branch"
4. Sélectionne la branche "main" et le dossier "/ (root)"
5. Clique sur "Save"
6. Attends 1-2 minutes que le site se déploie

### Étape 4 : Accéder à ton site

Ton site sera disponible à l'adresse :
```
https://TON_USERNAME.github.io/TON_REPO/
```

Par exemple : `https://jocelyn.github.io/myday-docs/`

## 📝 Personnalisation

### Modifier le contenu

Tous les textes sont dans le fichier `index.html`. Tu peux :
- Changer les descriptions
- Ajouter des sections
- Modifier les informations de contact
- Ajouter le lien App Store quand l'app sera publiée

### Modifier les couleurs

Les couleurs sont définies dans `styles.css` au début du fichier :
```css
:root {
    --primary-color: #007AFF;     /* Couleur principale */
    --secondary-color: #5856D6;   /* Couleur secondaire */
    --text-dark: #1D1D1F;         /* Texte principal */
    --text-light: #6E6E73;        /* Texte secondaire */
}
```

### Ajouter des images

1. Crée un dossier `images` dans ton dépôt
2. Upload tes images (captures d'écran, logo, etc.)
3. Dans `index.html`, ajoute les images :
```html
<img src="images/ton-image.png" alt="Description">
```

## 🔗 Domaine personnalisé (optionnel)

Si tu veux utiliser ton propre nom de domaine (ex: `docs.myday.app`) :

1. Achète un domaine chez un registraire (Namecheap, Google Domains, etc.)
2. Dans les settings DNS de ton domaine, ajoute un enregistrement CNAME :
   - Type : CNAME
   - Name : docs (ou www)
   - Value : `TON_USERNAME.github.io`
3. Dans GitHub Pages settings, ajoute ton domaine personnalisé
4. Active "Enforce HTTPS"

## 📱 Fonctionnalités du site

- ✅ Design responsive (mobile, tablette, desktop)
- ✅ Navigation fluide avec défilement doux
- ✅ Animations au scroll
- ✅ Section FAQ
- ✅ Politique de confidentialité
- ✅ Section support/contact
- ✅ Compatible avec tous les navigateurs modernes

## 🎨 Structure des fichiers

```
.
├── index.html      # Page principale avec tout le contenu
├── styles.css      # Styles et design
├── script.js       # Interactivité et animations
└── README.md       # Ce fichier
```

## 📞 Support

Pour toute question sur le site web, contacte-moi ou ouvre une issue sur GitHub.

## 📄 Licence

Ce site est créé pour MyDay. Tous droits réservés.
