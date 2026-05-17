# Astorya Ancenis — Site SEO local

Site vitrine optimisé SEO pour Astorya — agence de dépannage et infogérance informatique à Ancenis-Saint-Géréon (44150) et dans tout le Pays d'Ancenis.

## 🚀 Déploiement Vercel

### Option A — Déploiement par drag & drop (le plus simple)

1. Allez sur [vercel.com](https://vercel.com) et créez un compte (gratuit) si pas déjà fait
2. Cliquez sur **"Add New..." → "Project"**
3. Faites glisser le dossier complet du projet (ou son `.zip`) dans la zone d'upload
4. Vercel détecte automatiquement qu'il s'agit d'un site statique HTML
5. Cliquez sur **"Deploy"** — c'est tout, le site est en ligne en moins d'une minute

### Option B — Déploiement via GitHub (recommandé pour la suite)

1. Créez un dépôt GitHub (privé ou public) et poussez le contenu du projet
2. Sur Vercel : **"Add New..." → "Project" → Import Git Repository**
3. Sélectionnez votre dépôt
4. Framework Preset : **"Other"** (site HTML statique)
5. Output Directory : laissez vide ou mettez `.`
6. Cliquez sur **"Deploy"**

Chaque `git push` redéploiera automatiquement le site.

---

## 🌐 Configuration du sous-domaine `ancenis.astorya.fr`

### Côté Vercel
1. Dans le projet Vercel, allez dans **Settings → Domains**
2. Cliquez sur **"Add"** et saisissez `ancenis.astorya.fr`
3. Vercel vous donne un enregistrement DNS à créer (un CNAME)

### Côté gestionnaire DNS de `astorya.fr`
1. Connectez-vous à votre registrar / hébergeur DNS (OVH, Gandi, Cloudflare, etc.)
2. Dans la zone DNS de `astorya.fr`, ajoutez :

   | Type  | Nom        | Valeur                   | TTL  |
   |-------|------------|--------------------------|------|
   | CNAME | `ancenis`  | `cname.vercel-dns.com.`  | 3600 |

3. Propagation DNS : généralement 5 à 60 minutes (jusqu'à 24h dans les pires cas)
4. Une fois propagé, Vercel délivre **automatiquement le certificat HTTPS** (Let's Encrypt)

---

## ⚙️ Fichier `vercel.json` (déjà inclus)

Le fichier `vercel.json` à la racine du projet configure :
- Les redirections de la racine `/` vers `/index.html`
- Les headers de sécurité recommandés
- Le cache des assets statiques

---

## 📋 Après publication

1. Vérifier que `https://ancenis.astorya.fr` charge bien
2. Soumettre le sitemap dans [Google Search Console](https://search.google.com/search-console)
   URL du sitemap : `https://ancenis.astorya.fr/sitemap.xml`
3. Créer / mettre à jour la fiche **Google Business Profile** « Astorya Ancenis »
4. Obtenir des backlinks locaux (CCI Nantes-Saint-Nazaire, COMPA, annuaires du Pays d'Ancenis, partenaires)

---

## 📞 Coordonnées affichées

- Adresse : Place Saint-Pierre, 44150 Ancenis-Saint-Géréon *(à confirmer)*
- Téléphone : 02 85 52 13 95
- Email : contact@astorya.fr
- Horaires : Lun–Jeu 8h30–12h30 / 14h00–18h00 · Vendredi jusqu'à 17h30

## 🎯 SEO local — communes ciblées

Ancenis-Saint-Géréon (44150), Oudon (44521), Le Cellier (44850), Couffé (44521), Mésanger (44522), Vallons-de-l'Erdre (44540), Loireauxence (44370), Ligné (44850), Riaillé (44440), Joué-sur-Erdre (44440), Vair-sur-Loire (44150), Teillé (44440), Pannecé (44440).
