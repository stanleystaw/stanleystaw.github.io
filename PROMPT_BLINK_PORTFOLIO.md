# 🧊 Prompts Blink — Portfolio optimisé (3D & cinématique)

Récupérés depuis le tutoriel « Tutoriel site 3D - Blink » (@frenchstartupper)
et blink.new/prompts/portfolio, puis **adaptés à ton profil réel**.

- Lien Blink : https://taap.it/nzABEIq
- Tutoriel : https://adaptable-countess-491.notion.site/Tutoriel-site-3D-Blink-3d8ba358733f80ab80bdc8f8552ab655

**La méthode du tutoriel** : référence visuelle → structure SANS 3D → direction artistique → 3D → scroll → micro-interactions → optimisation → mobile.
> « Il vaut généralement mieux faire 8 prompts précis successifs qu'un gigantesque prompt demandant tout parfaitement du premier coup. »

Colle les prompts **dans l'ordre**, un par un, dans Blink.

---

## PROMPT 1 — Structure & direction artistique (SANS 3D)

```
Create a premium dark-themed portfolio landing page for Hugues Fadonougbo,
a Full-Stack Developer (Python & JavaScript, Kotlin, AI & automation,
cybersecurity) based in Cotonou, Benin. 5 years of experience.

Visual direction: cinematic dark navy background (#070b14), accent gradient
cyan → violet → pink, oversized headlines with tight tracking, generous
negative space, refined editorial layouts, minimal interface elements.

Structure:
- Full-screen hero: name, rotating role titles (Full-Stack Developer,
  Python & JavaScript specialist, AI & automation expert, cybersecurity
  enthusiast, UI/UX designer, Kotlin mobile app developer), availability
  badge, contact meta (Cotonou Benin, +229 01 40 91 22 72,
  stanleystawa3@gmail.com)
- Animated stats strip: 5+ years experience, 4 selected projects,
  7 expertise domains, 2 professional languages
- Scrolling technology marquee: Python, JavaScript, TypeScript, Node.js,
  Kotlin, AI & LLM, Automation, Cybersecurity, UI/UX, SQL, Turso/libSQL,
  Bots, Blender 3D
- About section with a real photograph framed by an animated gradient border
- 7 skill cards, each with its own accent color: Web development,
  Data & SaaS, AI & automation, Bots & integrations, Cybersecurity,
  Design & tools, Kotlin & mobile apps
- 4 project cards with real photography: StawaLend (decentralized finance
  lending MVP, Lead Dev & Product Designer), BETIQ (AI & data automation,
  Full-Stack & AI dev), Stanley Bot SaaS (multi-user bot management platform,
  Turso/libSQL), Content Automation (Python + AI pipeline for TikTok/YouTube)
- Contact panel: email, phone, YouTube channel HistoireAi-r6p

Use real photographic imagery only (developer workspace at night, financial
growth charts on tablet, dark analytics dashboard, chatbot conversation on a
smartphone, video editing studio). Do NOT use mobile-money kiosk or generic
fintech stock photos.

Do not add 3D yet. Focus first on creating an exceptional static art
direction and layout.
```

## PROMPT 2 — Vraie 3D sur le titre hero

```
Now add real 3D to the hero heading only. Do not redesign the rest.

Split the main title character by character. Each character should:
- fly in from depth on load (translateZ -220px to 0, rotateX 90deg to 0),
  staggered per character and per line
- then float in a continuous 3D wave: subtle rotateY, translateZ and
  vertical oscillation, each character with its own phase

The whole heading must sit in a 3D perspective (about 1100px) with
preserve-3d, and tilt subtly toward the cursor with heavy damping.

Keep the paragraph below completely static.
Use Three.js / React Three Fiber or pure CSS 3D transforms.
It should feel like premium interactive art direction, not a gimmick.
```

## PROMPT 3 — Particules & scroll cinématique

```
Add an interactive particle network canvas behind the hero: cyan, violet,
pink and amber nodes connected by thin lines, gently repelled by the cursor.

Add scroll-triggered animations with GSAP ScrollTrigger (or Intersection
Observer): masked line reveals on titles, fade + vertical movement on text,
slow scale reveals on images, animated counters on the stats strip.
Everything smooth and cinematic, synchronized with scroll progression.
No sudden transitions.
```

## PROMPT 4 — Micro-interactions (Framer Motion)

```
Add premium micro-interactions throughout the website using Framer Motion.
Animate:
- skill and project cards with slight 3D depth on mouse movement (tilt)
- animated gradient borders on the about photo and contact panel
- navigation links with animated underline
- buttons with subtle magnetic hover effects
- marquee pausing on hover
Keep every animation subtle. The website should feel luxurious and
cinematic, not playful.
```

## PROMPT 5 — Optimisation des performances (verbatim tutoriel)

```
Perform a complete performance optimization pass.
Focus especially on the 3D experience.
Optimize:
- geometry complexity
- textures
- image size
- WebGL rendering
- unnecessary re-renders
- animation performance
- lazy loading
Maintain 60 FPS whenever possible.
Do not degrade the visual quality unnecessarily.
Ensure smooth performance on modern laptops and smartphones.
```

## PROMPT 6 — Version mobile dédiée (verbatim tutoriel)

```
Create an optimized mobile version of the 3D experience.
Maintain the same creative direction but simplify expensive effects.
On mobile:
- reduce geometry complexity if necessary
- reduce particle count
- simplify lighting
- reduce cursor interactions
- preserve scroll storytelling
The mobile experience must remain premium and fluid.
```

---

## 🔥 BONUS — Le prompt complet du tutoriel (à personnaliser)

```
Create a world-class cinematic 3D website for [BRAND].

I want an experience inspired by premium Awwwards websites, luxury product
launches and high-end editorial art direction.

TECH STACK
Use:
- React
- Three.js
- React Three Fiber
- GSAP
- ScrollTrigger
- Framer Motion

DESIGN
Create a minimalist and premium visual direction.
Use:
- oversized editorial typography
- strong negative space
- asymmetrical layouts
- large visuals
- subtle gradients
- sophisticated lighting
- minimal interface elements

HERO
Create a full-screen 3D hero.
Place the product at the center of the scene.
Add realistic lighting, reflections and shadows.
The object should slowly move when idle and subtly react to cursor movement.

SCROLL EXPERIENCE
Create a continuous scroll-driven cinematic sequence.
The 3D object should remain persistent across several sections.
As the visitor scrolls:
- rotate the object
- change camera position
- zoom into details
- modify lighting
- introduce text
- transition between compositions
Use GSAP ScrollTrigger to synchronize everything with scroll progression.

MICRO-INTERACTIONS
Use Framer Motion for:
- text reveals
- image reveals
- button interactions
- navigation animations
- hover states

PERFORMANCE
Keep animations smooth and optimize the WebGL scene.
Target smooth 60 FPS performance.

RESPONSIVE
Create a dedicated mobile adaptation of the experience.
Simplify expensive 3D effects when necessary.

FINAL OBJECTIVE
The experience should feel like a premium interactive product film
transformed into a website.
Avoid generic landing-page components.
Avoid excessive effects.
Prioritize art direction, storytelling, composition and motion quality.
```

---

## 💡 Règles d'or du tutoriel

1. Une référence visuelle précise vaut mieux que « fais-moi un site magnifique ».
2. Construire la structure SANS la 3D d'abord.
3. Une seule scène 3D principale + 2-3 moments forts + beaucoup de respiration.
4. Décrire les animations physiquement (« la caméra tourne de 25° pendant que
   le titre sort du bas avec un masque »), jamais « ajoute des animations cool ».
5. Toujours finir par une passe performance + une version mobile simplifiée.
