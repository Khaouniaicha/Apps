# 🎓 حفل التخرج 2026 — Cérémonie de Graduation

Site web interactif de la cérémonie de remise des diplômes.  
موقع تفاعلي لتوثيق حفل التخرج.

---

## 📁 Structure du projet

```
graduation-project/
├── index.html      ← Page principale (tout-en-un)
├── data.json       ← Contenu : images, vidéos, galeries
├── vercel.json     ← Configuration déploiement Vercel
├── .gitignore      ← Fichiers à ignorer
└── README.md       ← Ce fichier
```

---

## 🚀 Déploiement — Étape par étape

### ÉTAPE 1 — Créer un compte GitHub (gratuit)
1. Aller sur **https://github.com**
2. Cliquer **Sign up** → remplir : nom d'utilisateur, email, mot de passe
3. Confirmer l'email reçu

---

### ÉTAPE 2 — Créer le repository GitHub
1. Sur GitHub, cliquer le bouton **"+"** en haut à droite → **New repository**
2. Nom du repo : `graduation-2026` (ou autre)
3. Laisser en **Public**
4. Ne PAS cocher "Add README" (vous en avez déjà un)
5. Cliquer **Create repository**

---

### ÉTAPE 3 — Uploader les fichiers sur GitHub
Sur la page du nouveau repo vide, cliquer **"uploading an existing file"** :
1. Glisser-déposer **tous les fichiers** du dossier :
   - `index.html`
   - `data.json`
   - `vercel.json`
   - `.gitignore`
   - `README.md`
2. En bas, écrire dans le champ : `Premier déploiement`
3. Cliquer **Commit changes**

---

### ÉTAPE 4 — Créer un compte Vercel (gratuit)
1. Aller sur **https://vercel.com**
2. Cliquer **Sign Up** → choisir **Continue with GitHub**
3. Autoriser Vercel à accéder à GitHub

---

### ÉTAPE 5 — Déployer sur Vercel
1. Sur le dashboard Vercel, cliquer **Add New → Project**
2. Trouver votre repo `graduation-2026` → cliquer **Import**
3. Laisser tous les paramètres par défaut
4. Cliquer **Deploy**
5. ✅ Votre site est en ligne ! URL du type : `graduation-2026.vercel.app`

---

## 🔄 Mise à jour du contenu (après déploiement)

Pour modifier les images ou textes, éditez `data.json` sur GitHub :
1. Ouvrir `data.json` sur GitHub
2. Cliquer l'icône ✏️ (Edit)
3. Modifier le fichier
4. Cliquer **Commit changes**
5. ✅ Vercel redéploie automatiquement en ~30 secondes

---

## 🌐 Domaine personnalisé (optionnel, gratuit)

Sur Vercel → votre projet → **Settings → Domains** :
- Ajouter votre domaine personnalisé si vous en avez un
- Vercel configure le SSL automatiquement

---

## 📝 Modifier le contenu — `data.json`

Chaque section du site correspond à une clé dans `data.json` :

| Clé | Section |
|-----|---------|
| `reception` | Accueil des invités |
| `opening` | Ouverture officielle |
| `graduates` | Entrée des diplômés |
| `shows` | Spectacles |
| `honors` | Remise des prix |
| `closing` | Clôture |
| `diplomas_delivery` | Remise des diplômes |
| `certificates_delivery` | Remise des attestations |
| `honor_certificates` | Certificats d'honneur |
| `delivery_moments` | Moments de remise |

Pour ajouter une image dans une section :
```json
{
  "url": "https://VOTRE-URL-IMAGE.jpg",
  "caption": {
    "ar": "وصف بالعربية",
    "fr": "Description en français",
    "en": "Description in English"
  }
}
```

---

## 🛠️ Technologies

- HTML5 / CSS3 / JavaScript vanilla
- Polices : Amiri, Cormorant Garamond, Playfair Display
- Images : Unsplash (remplaçables par vos propres photos)
- 0 dépendance — fonctionne sans npm, sans build
