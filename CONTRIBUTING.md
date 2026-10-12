# Contribuer à la formation

Merci de contribuer à cette ressource communautaire **en français**.

## Types de contributions

- Signaler une erreur dans un exemple JavaScript, TypeScript, YAML ou une commande CLI.
- Proposer une meilleure explication pédagogique ou une correction de formulation.
- Mettre à jour les informations de compatibilité **après vérification des sources officielles**.
- Ajouter des assertions, des cas de test ou des exercices pertinents.
- Améliorer l'accessibilité, le fonctionnement mobile ou les métadonnées SEO.

## Procédure

1. Ouvrir une *issue* décrivant le problème, avec le chapitre concerné et le comportement attendu.
2. Créer une branche depuis `main`, puis modifier `index.html` (cours statique autonome).
3. Tester dans un navigateur avec JavaScript activé et désactivé ; pour le menu mobile, vérifier particulièrement le mode sans JavaScript.
4. Vérifier que les extraits de code sont cohérents avec les API officiellement documentées au moment de la proposition.
5. Soumettre une *pull request* décrivant les modifications et les sources consultées.

## Convention éditoriale

- Rédiger en **français** les explications, les prompts, les consignes IA et les scénarios de test.
- Conserver exactement les identifiants techniques requis par les outils : API, clés YAML, noms de méthodes et chaînes de configuration.
- Ne pas figer le support sur une seule version du SDK : préciser la **compatibilité officielle** et documenter les solutions pour les versions plus récentes.
- Ne pas inventer de prise en charge d'une fonctionnalité sans référence officielle ou reproduction locale.
- Éviter les changements purement cosmétiques qui détériorent la lecture mobile.
- Ne jamais intégrer de clés API, de données personnelles ni de traces contenant des secrets.

## Vérification du site

Le cours est un simple `index.html` à la racine. Ouvrez-le directement sur ordinateur et mobile. Contrôlez les liens internes, les 25 chapitres, les exemples de code copiables dans un navigateur normal et la navigation sans JavaScript. Le workflow GitHub Actions exécute des vérifications de structure et de référencement.

## Droits et sources

Le contenu proposé doit être original ou compatible avec la [licence MIT](./LICENSE) du dépôt. Ne copiez pas de longs extraits de documentations tierces : privilégiez les liens, la paraphrase et les exemples originaux. Ce projet n'est pas une documentation officielle de Promptfoo ou d'OpenAI.
