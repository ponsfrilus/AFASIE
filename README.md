# AFASIE — Amélioration de la formation des apprenti·e·s et stagiaires informaticien·ne·s à l'EPFL

## À propos de ce document

Ce document regroupe différentes idées d'amélioration pour la formation des des
apprenti·e·s et stagiaires informaticien·ne·s à l'EPFL. Il est disponible en PDF
ici : [AFASIE.pdf](https://github.com/ponsfrilus/AFASIE/blob/main/AFASIE.pdf).

## Quelques recommandations

* Les listes utilisent l'étoile (`*`), pas d'intentation pour le premier niveau,
  indentation de 2 espaces (pas de tabulation).
* Les titres utilisent le dièze (`#`). Un espace de séparation est présent avant
  et après les titres. Les titres de niveau 1 sont précédés d'un double espace.

## Pour générer la table de matière

La table des matières est générée avec le package [Atom] [md-toc].

## Pour générer le PDF

```
pandoc AFASIE.md \
    --pdf-engine=xelatex \
    -V mainfont="DejaVu Sans" \
    -V urlcolor=cyan \
    -V papersize:a4paper \
    -V monofont="FreeMono" \
    -V geometry:vmargin=2cm \
    -V geometry:hmargin=3cm \
    -V block-headings \
    -o AFASIE.pdf; \
  xdg-open AFASIE.pdf
```

[Atom]: https://atom.io
[md-toc]: https://atom.io/packages/md-toc
