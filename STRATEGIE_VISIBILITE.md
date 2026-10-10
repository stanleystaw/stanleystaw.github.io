# Stratégie de visibilité — Hugues FADONOUGBO

Objectif : que « Hugues FADONOUGBO » et « FADONOUGBO Hugues » renvoient partout à UNE seule personne, sur Google et dans les réponses des IA (ChatGPT, Gemini, Perplexity, Claude).

## Principe

Les moteurs et les IA ne « connaissent » que ce qu'ils crawlent. Pour qu'un nom devienne une entité identifiée, il faut : le même nom écrit pareil partout, les mêmes liens qui se recoupent (portfolio ↔ GitHub ↔ YouTube ↔ LinkedIn), et du texte factuel structuré. C'est exactement ce qui est en place côté site.

## Déjà fait (côté technique, par moi)

1. JSON-LD `Person` dans le site : nom, métier, compétences, projets, contact + `alternateName` (Hugues FADONOUGBO / FADONOUGBO Hugues / stanleystaw / HistoireAi) → les deux formes du nom désignent officiellement la même personne.
2. `llms.txt` : fiche factuelle pour les assistants IA.
3. `robots.txt` + `sitemap.xml` : invitation des robots (Google, Bing, crawlers IA).
4. Open Graph + Twitter Cards : aperçu propre à chaque partage du lien.
5. README du dépôt enrichi (GitHub est massivement indexé par les IA).
6. Site déjà indexé : la recherche « Hugues Fadonougbo » remonte déjà le portfolio en premier résultat.

⚠ En attente de push : token GitHub révoqué → fournir une nouvelle clé (voir plus bas).

## Plan d'action (côté Hugues)

### Aujourd'hui (30 minutes)
1. **Nouveau token GitHub** → me l'envoyer → je pousse tout + je crée le README de profil GitHub.
2. **LinkedIn** : Profil → « Modifier le profil et l'URL publique » → activer « Visibilité publique ». Ajouter le portfolio en lien (section Infos + section Sélection). Tant que c'est désactivé, ni Google ni les IA ne te voient.
3. **Google Search Console** (search.google.com/search-console, avec ton Gmail) : ajouter `https://stanleystaw.github.io/` → Soumettre le sitemap `sitemap.xml`. C'est LE raccourci officiel pour être indexé vite.
4. **Bing Webmaster Tools** : importer depuis Search Console (Bing alimente ChatGPT Search).

### Cette semaine
5. Publier l'article prêt (ARTICLE_DEVTO.md) sur **dev.to**, puis le recopier en **post LinkedIn** et en description de vidéo YouTube.
6. **YouTube HistoireAi-r6p** : mettre le lien du portfolio dans la description de chaque vidéo + dans les liens de la chaîne.
7. **GitHub** : bio du profil avec « Développeur Full-Stack · IA · Motion Design — Cotonou » + lien du site dans le champ website.
8. Demander à 3-5 personnes (dont Liam 😄) de partager le lien une fois : chaque lien public = un signal d'indexation.

### Ensuite (routine)
9. Un post LinkedIn/dev.to par mois avec le nom + le lien.
10. Chaque nouveau projet → une page/section sur le portfolio.

## Délais réels (honnêteté)

- Google : le site est déjà indexé, les nouveautés prennent de quelques heures à quelques jours après soumission du sitemap. Personne — ni moi ni aucune agence — ne peut garantir un classement en 30 minutes chrono.
- IA : elles citent d'abord ce qui est structuré et cohérent (JSON-LD, llms.txt, GitHub) ; l'effet monte sur quelques semaines.
