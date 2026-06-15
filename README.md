# PHP Défensif — Slide deck

Slide deck reveal.js pour une présentation de 40 minutes destinée aux développeurs et développeuses PHP, couvrant la programmation défensive avec PHP moderne (PHP 8.0 → PHP 8.5).

## Aperçu

Inspiré du talk *Extremely Defensive PHP* de Marco Pivetta (ocramius), modernisé avec toutes les nouveautés du langage :

- PHP 8.0 : constructor property promotion, union types, nullsafe, `throw` comme expression, named arguments, match
- PHP 8.1 : `readonly` properties, enums, intersection types, `never`, first-class callables, new in initializers
- PHP 8.2 : `readonly` classes, DNF types
- PHP 8.3 : constantes typées
- PHP 8.4 : property hooks, asymmetric visibility, lazy objects
- PHP 8.5 : opérateur pipe `|>`, attribut `#[NoDiscard]`, `array_first()`/`array_last()`, stack traces sur erreurs fatales, constantes `final`

## Structure (~90 slides)

1. Introduction
2. Qu'est-ce que la programmation défensive ?
3. Le système de types
4. Immutabilité
5. Value Objects
6. Nullabilité maîtrisée
7. Encapsulation
8. Exceptions et résultats
9. Nouveautés PHP 8.5
10. Outils & CI
11. Top 10 des anti-patterns
12. Mise en pratique (refactoring)
13. Conclusion

## Lancement

Aucune build step nécessaire — reveal.js est chargé depuis le CDN.

```bash
# Soit via un serveur statique
python3 -m http.server 8000
# puis ouvrir http://localhost:8000

# Soit avec npx
npx serve .
```

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
- Thème reveal.js de base : `night` (modifiable dans `index.html`)

## Licence

Faites-en bon usage. Si vous donnez le talk, créditer l'inspiration originale (ocramius) est apprécié.
