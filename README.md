# Promptfoo × OpenAI Agents — formation complète en français

Formation pratique et gratuite, en français, pour **évaluer, tester et sécuriser des agents IA construits avec OpenAI Agents SDK (JavaScript / TypeScript) et Promptfoo**.

**[Consulter la formation en ligne](https://claude.ai/artifact/6kBjDnxFYcvvcaty1mnZHz#no_universal_links)** · [Documentation officielle Promptfoo](https://www.promptfoo.dev/docs/providers/openai-agents/) · [OpenAI Agents SDK](https://github.com/openai/openai-agents-js)

> **Publication :** la formation est consultable sur [Claude Artifacts](https://claude.ai/artifact/6kBjDnxFYcvvcaty1mnZHz#no_universal_links). Le dépôt GitHub conserve la source HTML, l'historique et les contributions.

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

- **En ligne :** [ouvrir le cours](https://claude.ai/artifact/6kBjDnxFYcvvcaty1mnZHz#no_universal_links).
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
├── .nojekyll                   # Utile si GitHub Pages est activé ultérieurement
├── CONTRIBUTING.md             # Contributions et corrections
├── LICENSE                     # Licence MIT du contenu original
└── .github/workflows/check.yml # Validation élémentaire lors des contributions
```

## Publication du cours

La version publique actuelle de la formation est hébergée sur **Claude Artifacts** :

**[Ouvrir la formation française Promptfoo × OpenAI Agents](https://claude.ai/artifact/6kBjDnxFYcvvcaty1mnZHz#no_universal_links)**

Le fichier [`index.html`](./index.html) présent dans ce dépôt permet de conserver une copie portable du cours et de contribuer aux corrections. Le cours fonctionne également comme page HTML statique si vous choisissez plus tard un hébergement indépendant (par exemple GitHub Pages ou un domaine personnel).

## Référencement et découverte

Le fichier source `index.html` inclut un titre explicite, une description en français, une URL canonique correspondant à **l'Artifact public** (sans fragment `#no_universal_links`), des métadonnées Open Graph et des données structurées Schema.org de type `Course`.

**Limite importante :** la capacité des moteurs de recherche à explorer et indexer une page `claude.ai/artifact/...` dépend de Claude.ai. Ce dépôt ne contrôle pas ses en-têtes HTTP, son fichier `robots.txt`, ses directives d'indexation ni son sitemap. **Une URL publiée ne garantit pas son indexation.** Un sitemap servi sur GitHub ne peut pas, à lui seul, faire indexer une URL appartenant au domaine `claude.ai`.

Pour faciliter la découverte :

1. Ajoutez l'[URL publique de la formation](https://claude.ai/artifact/6kBjDnxFYcvvcaty1mnZHz#no_universal_links) dans le champ **Website** de la rubrique **About** du dépôt GitHub.
2. Complétez la description du dépôt et les *topics* : `promptfoo`, `openai-agents`, `agents-sdk`, `typescript`, `ai-evaluation`, `llm-testing`, `french`, `formation`.
3. Partagez le dépôt et la formation dans des ressources spécialisées en IA et développement francophone.
4. Si l'indexation autonome et la propriété du sitemap deviennent prioritaires, déployez également le HTML sur un hébergement que vous contrôlez et utilisez alors son URL canonique et son sitemap.

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
