# Pointage Terminal : installation

Le dossier `pointage-pwa/` contient toute l'appli. Il suffit de le mettre en ligne (gratuit), puis de l'ajouter à l'écran d'accueil.

## 1. Mettre le dossier en ligne

**Netlify (le plus simple)**
1. Créer un compte gratuit sur netlify.com.
2. Ouvrir app.netlify.com/drop et glisser le dossier `pointage-pwa`.
3. Netlify donne une adresse en `.netlify.app`. Dans les réglages du site, tu peux la renommer en quelque chose de peu devinable.

**GitHub Pages**
1. Créer un dépôt, y envoyer le contenu de `pointage-pwa/` à la racine.
2. Settings > Pages > Deploy from a branch > `main` / `(root)`.
3. L'adresse sera `https://<ton-compte>.github.io/<dépôt>/`.

## 2. Installer sur le téléphone

- **iPhone** (Safari obligatoire) : ouvrir l'adresse, bouton Partager, « Sur l'écran d'accueil ».
- **Android** (Chrome) : ouvrir l'adresse, menu ⋮, « Installer l'application ».

Ouvre ensuite l'appli depuis l'icône, pas depuis le navigateur.

## 3. À savoir

- **Tes données restent sur le téléphone.** La page en ligne ne contient que le code. Personne ne voit tes horaires.
- **Sur iPhone**, l'appli installée a son propre stockage : elle ne retrouve pas ce que tu as saisi dans Safari. Installe d'abord, utilise ensuite.
- **Sauvegarde** : CONFIG > EXPORTER crée un fichier JSON. RESTAURER le recharge (il remplace tout). Fais-le de temps en temps, surtout avant de changer de téléphone.
- **Export des heures** : JOURNAL > EXPORT CSV (ouvrable dans Excel).
- **Hors ligne** : l'appli fonctionne sans réseau après la première ouverture. La police terminal (VT323) vient de Google Fonts ; sans elle, une police monospace standard prend le relais.
- **Sous-tâches** : CONFIG > SOUS-TÂCHES RÉPÉTITIVES crée la liste (réservée à l'emploi A). Pendant une session sur A, les boutons de sous-tâche apparaissent dans le statut : en changer clôt le segment en cours et en ouvre un nouveau, le temps est ventilé dans le bloc SOUS-TÂCHES. Si tu en choisis une dans les 2 minutes après l'entrée, elle s'applique à toute la session.
- **Mettre à jour** : remplacer les fichiers en ligne, puis changer `VERSION` dans `sw.js` (version actuelle : `pointage-v2`, la suivante serait `pointage-v3`) pour que les téléphones rechargent le cache. L'appli installée se met à jour à la réouverture, parfois après l'avoir fermée puis rouverte une seconde fois. Tes données sont conservées.
- La page contient `noindex` : les moteurs de recherche ne devraient pas la lister.
