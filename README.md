# Portfolio — Hugues Fadonougbo

Développeur Full-Stack · Python & JavaScript — IA & automatisation · Cybersécurité · 5 ans d'expérience.
Cotonou, Bénin · stanleystawa3@gmail.com · +229 01 40 91 22 72

## Le site

`index.html` est une page vitrine **entièrement autonome** (une seule fichier, aucune dépendance externe) :
styles, scripts et images (base64) sont embarqués. Ouvrez-le tel quel dans un navigateur,
ou servez-le depuis n'importe quel hébergement statique (GitHub Pages, Netlify, Replit…).

## Contenu

- `index.html` — le portfolio complet (hero animé, compétences, projets, contact)
- `assets/` — les photographies originales optimisées utilisées sur le site
- `README.md` — ce fichier

## Sections

1. **Hero** — réseau de particules interactif (canvas), effet machine à écrire, compteurs animés
2. **À propos** — profil, langues, photo encadrée dégradée
3. **Compétences** — développement web (React, Next.js, Vue/Nuxt, Tailwind), données & SaaS, IA & automatisation, bots, cybersécurité, design, Kotlin & apps mobiles
4. **Projets** — StawaLend, BETIQ, Stanley Bot SaaS, Automatisation de contenu
5. **Contact** — email, téléphone, YouTube (HistoireAi-r6p)

## Sécurité

Page statique sans backend ni saisie utilisateur : CSP stricte (`default-src 'none'`),
`rel="noopener noreferrer"` sur les liens externes, `meta referrer no-referrer`,
aucun `eval`/`innerHTML`/handler inline, aucune ressource externe chargée.

## Lancer en local

```bash
python3 -m http.server 3000
# puis ouvrir http://localhost:3000
```
