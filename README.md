# PHP Défensif — Slide deck

Slide deck reveal.js pour une présentation de 40 minutes destinée aux développeurs et développeuses PHP, couvrant la programmation défensive avec PHP moderne (PHP 8.0 → PHP 8.5).

## Aperçu

Inspiré du talk *Extremely Defensive PHP* de Marco Pivetta (ocramius), modernisé avec toutes les nouveautés du langage :

- PHP 8.0 : constructor property promotion, union types, nullsafe, `throw` comme expression, named arguments, match
- PHP 8.1 : `readonly` properties, enums, intersection types, `never`, first-class callables, new in initializers
- PHP 8.2 : `readonly` classes, DNF types
- PHP 8.3 : constantes typées
- PHP 8.4 : property hooks, asymmetric visibility, lazy objects
- PHP 8.5 : attribut `#[NoDiscard]`

## Structure (~90 slides)

1. Introduction
2. Qu'est-ce que la programmation défensive ?
3. Le système de types
4. Immutabilité
5. Value Objects
6. Nullabilité maîtrisée
7. Encapsulation
8. Exceptions et résultats
9. Outils & CI
10. Top 10 des anti-patterns
11. Mise en pratique (refactoring)
12. Conclusion

## Lancement

Aucune build step nécessaire — toutes les ressources (reveal.js, highlight.js, GIF) sont **embarquées localement** dans `vendor/` et `assets/`. Le deck fonctionne intégralement **hors-ligne**.

Ouvre simplement `index.html` dans ton navigateur (double-clic ou `open index.html` sur macOS).

> Un serveur statique (`python3 -m http.server 8000`, `npx serve .`) n'est nécessaire que si tu ajoutes des fichiers markdown externes ou des modules ES, ou pour tester l'export PDF via `?print-pdf`.

## Raccourcis utiles

- `Espace` ou `→` : slide suivante
- `S` : speaker notes (vue présentateur)
- `O` ou `Esc` : vue d'ensemble (overview)
- `F` : plein écran
- `B` : écran noir (pause)
- `?` : aide

## Export PDF

Ouvrir l'URL avec `?print-pdf` (ex: `http://localhost:8000/?print-pdf`), puis imprimer en PDF depuis Chrome.

## Personnalisation

- Slides : `index.html`
- Thème custom : `css/custom.css`
- Thème reveal.js de base : `white` (modifiable dans `index.html`)
- Librairies vendues : `vendor/reveal.js/` (reveal.js 5.1.0) et `vendor/highlight.js/` (highlight.js 11.9.0)
- Images : `assets/`

## Licence

Faites-en bon usage. Si vous donnez le talk, créditer l'inspiration originale (ocramius) est apprécié.
