# Sécurité du portfolio

## Architecture et limites
Ce dépôt publie un site statique sur GitHub Pages : aucun serveur applicatif, aucune base de données et aucun traitement des formulaires côté serveur dans ce dépôt. Les formulaires ouvrent le logiciel e-mail du visiteur. L'envoi effectif dépend de ce logiciel et de la confirmation de l'utilisateur. Ne jamais y saisir de secrets ou de données sensibles.

## Protections du code
- CSP avec liste d'empreintes SHA-256 des scripts autorisés ; aucun `unsafe-inline` pour JavaScript.
- Scripts événementiels HTML interdits ; connexions réseau, objets, iframes, workers, base URL et soumission HTTP de formulaires interdits par la CSP.
- Styles inline conservés pour les animations et la mise en page : protection de styles moins stricte que celle des scripts.
- Politique de référent `no-referrer` et liens externes à nouvel onglet avec `noopener noreferrer`.
- Affichage de données via `textContent`, sans interpolation de contenu visiteur en HTML dans le code examiné.
- Pas de script CDN tiers ni de dépendance JavaScript à installer sur le site.

## Modifier JavaScript
Après toute modification du contenu d'un script, recalculer son empreinte dans la CSP. Une empreinte périmée bloque le script et peut casser l'interface. Vérifier la console et les fonctionnalités dans un navigateur avant publication.

## Hébergement et compte GitHub
HTTPS et HSTS ont été observés au moment du contrôle. Les en-têtes personnalisés ne sont pas pilotés par ce dépôt sur GitHub Pages. `frame-ancestors` ne fonctionne pas dans une balise meta : une protection anti-encadrement exige un en-tête HTTP, donc un hébergement/proxy permettant de le définir. Ne pas ajouter un faux fichier `_headers` en prétendant qu'il est appliqué par GitHub Pages.

La double authentification, les passkeys, les accès tiers, les règles de branche et la protection des secrets du compte doivent être vérifiés dans GitHub. Aucun audit de ces réglages n'est affirmé ici.

Un jeton d'accès partagé dans une conversation doit être révoqué après utilisation. Ne jamais le committer. `.gitignore` aide à prévenir certains ajouts accidentels mais ne constitue pas une protection absolue.

## Signalement
Contact : stanleystawaca@gmail.com. Merci de décrire le problème sans publier de données confidentielles. Aucun test destructif, déni de service ou test sur un service tiers n'est autorisé par ce document.

Une revue statique et des tests ciblés ne garantissent pas l'absence de vulnérabilités.
