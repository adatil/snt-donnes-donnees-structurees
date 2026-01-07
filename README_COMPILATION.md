# Compilation des documents LaTeX

## Problèmes résolus

Les fichiers LaTeX ont été corrigés pour être compatibles avec tous les compilateurs :

1. **Emoji remplacé** : L'emoji ✏️ a été remplacé par la commande `\ding{46}` du package `pifont`
2. **Guillemets français** : Les guillemets « » ont été remplacés par les commandes LaTeX `\og{}` et `\fg{}`

## Compilation

Vous pouvez maintenant compiler les documents avec n'importe quel compilateur :

### Avec pdflatex (recommandé)
```bash
pdflatex TP_donnees_structurees_enonce.tex
pdflatex TP_donnees_structurees_corrige.tex
```

### Avec xelatex
```bash
xelatex TP_donnees_structurees_enonce.tex
xelatex TP_donnees_structurees_corrige.tex
```

### Avec lualatex
```bash
lualatex TP_donnees_structurees_enonce.tex
lualatex TP_donnees_structurees_corrige.tex
```

## Note

Pour obtenir les références et la table des matières correctes, lancez la compilation deux fois :

```bash
pdflatex TP_donnees_structurees_enonce.tex
pdflatex TP_donnees_structurees_enonce.tex
```

## Packages requis

Assurez-vous d'avoir les packages LaTeX suivants installés :
- `babel` (pour le français)
- `geometry`
- `hyperref`
- `enumitem`
- `xcolor`
- `pifont` (pour le symbole crayon)
