# Promptfoo × OpenAI Agents — formation complète en français

Formation pratique et gratuite, en français, pour **évaluer, tester et sécuriser des agents IA construits avec OpenAI Agents SDK (JavaScript / TypeScript) et Promptfoo**.

**[Consulter la formation en ligne](https://tarakbz.github.io/promptfoo-openai-agents-fr/)** · [Documentation officielle Promptfoo](https://www.promptfoo.dev/docs/providers/openai-agents/) · [OpenAI Agents SDK](https://github.com/openai/openai-agents-js)

> **Publication officielle du cours :** [GitHub Pages](https://tarakbz.github.io/promptfoo-openai-agents-fr/), directement depuis la branche `main` du dépôt.

## Au programme

Ce cours en **25 chapitres** explique comment mettre à l'épreuve un agent au-delà de ses seules réponses textuelles :

- installation de Promptfoo et compatibilité officielle avec OpenAI Agents SDK ;
- utilisation du fournisseur natif `openai:agents:*` ;
- solution avec **fournisseur JavaScript personnalisé** lorsque le SDK utilisé est plus récent que la plage prise en charge nativement ;
- assertions, jeux de tests, critères d'évaluation et résultats ;
- appels d'outils, simulations (mocks), handoffs et garde-fous ;
- état conversationnel, sessions, entrées multimodales ;
- traces, trajectoires d'agents et OpenTelemetry ;
- *red teaming*, cas de régression et bonnes pratiques de sécurité ;
- atelier guidé en **TypeScript et YAML**, prompts et instructions IA en français.

Les noms des API, paramètres et identifiants de configuration restent inchangés pour garantir leur utilité dans le code.

## Lire la formation

- **En ligne :** [ouvrir le cours](https://tarakbz.github.io/promptfoo-openai-agents-fr/).
- **Hors ligne :** télécharger [`index.html`](./index.html) et l'ouvrir dans un navigateur.
- **Mobile :** le sommaire et la navigation fonctionnent sans JavaScript. La recherche, les boutons « Copier » et la sauvegarde de progression nécessitent JavaScript.

La page est entièrement statique : **aucun build, framework CSS, compte ou serveur n'est nécessaire** pour lire la formation.

## Démarrer les exercices

Prévoir Node.js et pnpm, ainsi qu'une clé API OpenAI si les exemples exécutent de vrais appels. Dans un projet dédié :

```bash
mkdir atelier-promptfoo-agents
cd atelier-promptfoo-agents
pnpm init
pnpm add -D promptfoo
pnpm add @openai/agents zod
```

Les exemples YAML et TypeScript sont fournis dans les chapitres du cours. Ne publiez **jamais** de clés API ou de traces contenant des données personnelles. Les évaluations avec des modèles externes peuvent entraîner des frais.

### Compatibilité du SDK

Le fournisseur natif de Promptfoo vérifie la compatibilité de `@openai/agents` : **consultez les exigences actuelles de la [documentation officielle](https://www.promptfoo.dev/docs/providers/openai-agents/)**. La compatibilité n'est pas garantie dès la sortie d'une nouvelle version.

Si le fournisseur natif refuse votre version du SDK, **conservez la version nécessaire à votre application** et utilisez un [fournisseur JavaScript personnalisé](https://www.promptfoo.dev/docs/providers/custom-api/) pour appeler l'agent via votre propre projet. Le chapitre « Compatibilité et installation » détaille les deux approches et les commandes de vérification.

## Architecture du dépôt

```text
.
├── index.html                  # Source HTML autonome du cours
├── README.md                   # Présentation et instructions
├── sitemap.xml                 # Sitemap SEO de la formation
├── .nojekyll                   # Désactivation de Jekyll pour GitHub Pages
├── CONTRIBUTING.md             # Contributions et corrections
├── LICENSE                     # Licence MIT du contenu original
└── .github/workflows/check.yml # Validation élémentaire lors des contributions
```

## Publication du cours sur GitHub Pages

La formation est accessible publiquement et gratuitement à cette adresse :

**[Consulter la formation Promptfoo × OpenAI Agents en français](https://tarakbz.github.io/promptfoo-openai-agents-fr/)**

GitHub Pages publie le fichier `index.html` depuis la branche `main`, dossier `/(root)`. Le site est une page HTML statique autonome, sans build ni framework nécessaire.

Pour retrouver ou modifier les réglages, ouvrir [Settings → Pages](https://github.com/tarakbz/promptfoo-openai-agents-fr/settings/pages). Les modifications du fichier `index.html` sur `main` sont automatiquement prises en compte après déploiement.

## Référencement et découverte

Le site utilise l'adresse canonique **https://tarakbz.github.io/promptfoo-openai-agents-fr/** dans le HTML et les métadonnées :

- `<title>` et `meta description` rédigés en français pour présenter la formation ;
- balises `canonical`, `og:title`, `og:description` et `og:url` pour l'identification et le partage ;
- données structurées [Schema.org `Course`](https://schema.org/Course) pour décrire la ressource pédagogique ;
- [`sitemap.xml`](./sitemap.xml) disponible à **https://tarakbz.github.io/promptfoo-openai-agents-fr/sitemap.xml** ;
- structure HTML sémantique et sommaire de navigation accessible sur mobile.

Pour améliorer la découverte :

1. Indiquer **https://tarakbz.github.io/promptfoo-openai-agents-fr/** dans le champ **Website** de la section **About** du dépôt.
2. Donner au dépôt une description précise : « Formation Promptfoo et OpenAI Agents SDK en français : évaluation LLM, tests TypeScript, outils, tracing et red teaming ».
3. Ajouter les *topics* GitHub : `promptfoo`, `openai-agents`, `agents-sdk`, `typescript`, `ai-evaluation`, `llm-testing`, `french`, `formation`.
4. Vérifier l'accès public au cours et au sitemap ; utiliser [Google Search Console](https://search.google.com/search-console/about) pour suivre la présence dans l'index et soumettre le sitemap si la propriété est validée.

**L'indexation par les moteurs de recherche ne peut pas être garantie** : le référencement dépend aussi de leurs règles d'exploration et de la qualité des liens pointant vers le site.

## Contribution

Les corrections techniques, améliorations pédagogiques et signalements de liens obsolètes sont les bienvenus. Voir [CONTRIBUTING.md](./CONTRIBUTING.md). Les changements de compatibilité doivent toujours être vérifiés avec la documentation officielle.

## Sources et indépendance

Support pédagogique **original**, rédigé en français et inspiré des fonctions présentées dans les documentations officielles :

- [Promptfoo — OpenAI Agents](https://www.promptfoo.dev/docs/providers/openai-agents/)
- [Promptfoo — fournisseurs personnalisés](https://www.promptfoo.dev/docs/providers/custom-api/)
- [OpenAI Agents SDK — projet officiel](https://github.com/openai/openai-agents-js)

Ce projet est **indépendant** et n'est **ni une traduction officielle, ni affilié ou approuvé** par Promptfoo ou OpenAI. Les marques citées appartiennent à leurs titulaires respectifs.

## Licence

La rédaction originale et les exemples propres à ce dépôt sont diffusés sous la [licence MIT](./LICENSE). La licence ne couvre pas les marques, documentations officielles et contenus appartenant à des tiers.
