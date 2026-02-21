# 🏠 Saint-Eloi - Site Web

Site web pour les résidents de la résidence Saint-Eloi à Montpellier.

## 📁 Structure des fichiers

```
saint-eloi/
├── index.html      ← Le site (ne pas modifier)
├── config.json     ← ⭐ TOUTES LES DONNÉES À MODIFIER
├── manifest.json   ← Configuration PWA
├── sw.js           ← Service Worker (mode hors-ligne)
├── icon-192.png    ← Icône petite
├── icon-512.png    ← Icône grande
└── README.md       ← Ce fichier
```

---

## ✏️ COMMENT MODIFIER LES INFORMATIONS

### 🔑 Modifier les codes (WiFi, Portail)

1. Ouvrir `config.json`
2. Chercher la section `"codes"`
3. Modifier les valeurs :

```json
"codes": {
  "portail": "78965",        ← Code du portail
  "wifi_reseau": "Livebox-4988",  ← Nom du WiFi
  "wifi_mdp": "mayleen34090"      ← Mot de passe WiFi
}
```

4. Sauvegarder → Le site est mis à jour !

---

### 🕐 Modifier les horaires

Dans `config.json`, section `"horaires"` :

```json
"horaires": {
  "cuisine_ouverture": "08h00",
  "cuisine_fermeture": "22h00",
  "repas_midi_debut": "11h00",
  "repas_midi_fin": "14h00",
  "repas_soir_debut": "18h00",
  "repas_soir_fin": "21h00",
  "silence": "23h00"
}
```

---

### 📢 Ajouter une actualité

Dans `config.json`, section `"actualites"`, ajouter un bloc :

```json
{
  "id": "nouvelle-actu",
  "date": {
    "fr": "15 Mars",
    "en": "March 15",
    "ru": "15 марта",
    "ar": "15 مارس",
    "ka": "15 მარტი",
    "hy": "Մdelays 15"
  },
  "titre": {
    "fr": "Titre de l'actualité",
    "en": "News title",
    "ru": "Заголовок",
    "ar": "عنوان الخبر",
    "ka": "სათაური",
    "hy": "Delays"
  },
  "contenu": {
    "fr": "Le contenu de l'actualité ici...",
    "en": "News content here...",
    "ru": "Содержание...",
    "ar": "المحتوى...",
    "ka": "შინაარსი...",
    "hy": "Delays..."
  },
  "important": true,
  "actif": true
}
```

**Notes :**
- `important: true` → Encadré rouge
- `important: false` → Encadré normal
- `actif: false` → Masque l'actualité sans la supprimer

---

### 📞 Modifier le contact

Dans `config.json`, section `"contact"` :

```json
"contact": {
  "responsable": "Bastien",
  "telephone": "0613703810",
  "email": "contact@saint-eloi.fr"
}
```

---

## 🚀 MISE EN LIGNE SUR GITHUB PAGES

### Première fois (création)

1. **Créer un compte GitHub** sur [github.com](https://github.com)

2. **Créer un nouveau repository**
   - Cliquer sur "New repository"
   - Nom : `saint-eloi`
   - Cocher "Public"
   - Cliquer "Create repository"

3. **Uploader les fichiers**
   - Cliquer "uploading an existing file"
   - Glisser-déposer TOUS les fichiers
   - Cliquer "Commit changes"

4. **Activer GitHub Pages**
   - Aller dans Settings → Pages
   - Source : "Deploy from a branch"
   - Branch : `main` / `root`
   - Cliquer "Save"

5. **Attendre 2-3 minutes** → Le site est en ligne !
   - URL : `https://TON-PSEUDO.github.io/saint-eloi/`

---

### Modifications suivantes

#### Option A : Via le site GitHub (recommandé)

1. Aller sur `github.com/TON-PSEUDO/saint-eloi`
2. Cliquer sur `config.json`
3. Cliquer sur le crayon ✏️ (Edit)
4. Faire les modifications
5. Cliquer "Commit changes"
6. **C'est en ligne en 30 secondes !**

#### Option B : Via l'app mobile GitHub

1. Télécharger "GitHub" sur App Store / Play Store
2. Se connecter
3. Aller sur le repository `saint-eloi`
4. Modifier `config.json`
5. Commit → En ligne !

---

## 🎨 Fonctionnalités du site

| Fonctionnalité | Description |
|----------------|-------------|
| 🌍 Multilingue | 6 langues (FR, EN, RU, AR, KA, HY) |
| 🌙 Mode sombre | Bouton dans la barre de navigation |
| 🔤 Taille texte | Boutons A+ / A- pour ajuster |
| 📱 PWA | Installable sur téléphone |
| 📴 Hors-ligne | Fonctionne sans internet (après 1ère visite) |
| 📲 QR Code | Pour partager facilement |
| 💬 Chatbot | Réponses rapides aux questions |
| 📞 Appel direct | Boutons pour appeler/SMS/WhatsApp |

---

## ❓ Besoin d'aide ?

Si tu as des questions ou des problèmes :
1. Vérifie que `config.json` est bien formaté (pas de virgule en trop)
2. Utilise [jsonlint.com](https://jsonlint.com) pour vérifier le JSON
3. Attends 2-3 minutes après un commit pour voir les changements

---

## 📋 Checklist avant mise en ligne

- [ ] Vérifier les codes (portail, WiFi)
- [ ] Vérifier le numéro de téléphone
- [ ] Vérifier les horaires
- [ ] Vérifier les actualités
- [ ] Tester le site localement (ouvrir index.html)
- [ ] Créer les icônes (192x192 et 512x512 pixels)

---

*Dernière mise à jour : Février 2025*
