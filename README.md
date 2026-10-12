# Promptfoo × OpenAI Agents — formation complète en français

Formation pratique et gratuite, en français, pour **évaluer, tester et sécuriser des agents IA construits avec OpenAI Agents SDK (JavaScript / TypeScript) et Promptfoo**.

**[Consulter la formation en ligne](https://tarakbz.github.io/promptfoo-openai-agents-fr/)** · [Documentation officielle Promptfoo](https://www.promptfoo.dev/docs/providers/openai-agents/) · [OpenAI Agents SDK](https://github.com/openai/openai-agents-js)

> **Publication :** l'adresse GitHub Pages ci-dessus fonctionne après activation de GitHub Pages dans les paramètres du dépôt (instructions plus bas).

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
├── index.html                  # Cours complet et page d'accueil GitHub Pages
├── README.md                   # Présentation et instructions
├── sitemap.xml                 # Découverte de l'URL canonique du cours
├── .nojekyll                   # Désactive la transformation Jekyll
├── CONTRIBUTING.md             # Contributions et corrections
├── LICENSE                     # Licence MIT du contenu original
└── .github/workflows/check.yml # Validation élémentaire lors des contributions
```

## Hébergement gratuit avec GitHub Pages

Ce dépôt est conçu pour une **publication depuis la branche `main`**, sans étape de compilation :

1. Ouvrez **[Settings → Pages](https://github.com/tarakbz/promptfoo-openai-agents-fr/settings/pages)**.
2. Sous **Build and deployment**, choisissez **Deploy from a branch**.
3. Sélectionnez **`main`** et le dossier **`/(root)`**, puis **Save**.
4. Accédez à **https://tarakbz.github.io/promptfoo-openai-agents-fr/** une fois le déploiement terminé.

Les mises à jour de `index.html` sur la branche `main` déclenchent ensuite le mécanisme habituel de publication GitHub Pages. En cas de problème, consultez l'onglet **Actions** du dépôt.

Référence : [guide officiel de configuration GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Référencement et découverte

La page contient un **titre explicite**, une **meta description en français**, une URL **canonique**, les balises de partage Open Graph/Twitter et des **données structurées Schema.org** pour décrire le support pédagogique.

Le fichier [`sitemap.xml`](./sitemap.xml) déclare l'URL canonique. Pour faciliter la découverte par les moteurs :

1. Activez GitHub Pages et vérifiez que le cours répond en HTTP 200.
2. Ajoutez l'URL du site dans [Google Search Console](https://search.google.com/search-console/about) via la méthode de vérification proposée.
3. Soumettez **https://tarakbz.github.io/promptfoo-openai-agents-fr/sitemap.xml** si la propriété sélectionnée autorise ce chemin.
4. Ajoutez dans **About** du dépôt la description et l'adresse du site, puis les *topics* : `promptfoo`, `openai-agents`, `agents-sdk`, `typescript`, `ai-evaluation`, `llm-testing`, `french`, `formation`.

**Note :** un sitemap aide à la découverte, sans garantir l'indexation ou une position particulière dans les résultats.

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
