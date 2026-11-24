# StockPro – publication GitHub Pages

## Fichiers
- `index.html` : application StockPro
- `manifest.webmanifest` : configuration d'installation PWA
- `service-worker.js` : cache hors connexion
- `icons/` : icônes Android/tablette

## Publication
1. Créer un dépôt GitHub public nommé `stockpro`.
2. Envoyer tous les fichiers et le dossier `icons` à la racine du dépôt.
3. Dans Settings > Pages, choisir `Deploy from a branch`, branche `main`, dossier `/ (root)`, puis Save.
4. Attendre la publication et ouvrir l'URL HTTPS fournie par GitHub Pages.
5. Ouvrir le site une première fois avec Internet. Sur Android/Chrome : menu ⋮ > Installer l'application (ou Ajouter à l'écran d'accueil).

## Données
Les données sont conservées dans le stockage local du navigateur (`localStorage`, clé `stockpro`). Elles restent sur l'appareil et le navigateur où elles ont été saisies. Faire régulièrement une sauvegarde/export avant de changer d'appareil ou d'effacer les données du navigateur.

## Sécurité importante
L'écran de connexion inclus est uniquement une barrière d'accès côté navigateur. Le nom d'utilisateur et le vérificateur du mot de passe sont présents dans le code public et cette protection peut être contournée par une personne technique. Ne pas utiliser ce paquet comme protection de données confidentielles. Pour un accès réellement privé, il faut connecter une authentification serveur (par exemple Supabase Auth) et protéger les données côté serveur. Le mot de passe fourni doit être changé s'il a été exposé dans un dépôt public.
