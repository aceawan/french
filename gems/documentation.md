# Documentation

D intègre directement beaucoup de techniques de programmation moderne. En plus de la *programmation par contrats* et des *tests unitaires*, D permet de générer de la [documentation](https://dlang.org/phobos/std_variant.html) à partir du code source.

En lisant des commentaires dans un format standard pour documenter les types et les fonctions, la commande `dmd -D` génère une documentation au format HTML à partir des fichiers sources qui lui sont fournis. En fait, l'intégralité de la [documentation de Phobos](https://dlang.org/phobos) a été générée à l'aide de *DDoc*.

Les styles de commentaires suivants sont interprétés par DDoc pour générer de la documentation:

* `/// Trois barres obliques avant un type ou une fonction`
* `/++ Commentaire multi-ligne avec deux + +/`
* `/** Commentaire multi-ligne avec deux * */`

Jetez un coup d'œil au code source d'exemple pour découvrir quelques uns des champs que peuvent contenir ces commentaires.

### Pour aller plus loin

- [Fonctionnement de DDoc](https://dlang.org/spec/ddoc.html)
- [Documentation de la librairie standard](https://dlang.org/phobos)

## {SourceCode:incomplete}

```d
/**
  Calcule la racine carrée d'un nombre.

  Ici on pourrait mettre un paragraphe
  qui s'étend sur les bienfaits pour la
  société et pour la galaxie d'une fonction
  capable de calculer la racine carré d'un
  nombre.

  Example:
  -------------------
  double sq = sqrt(4);
  -------------------
  Params:
    number = le nombre dont on veut calculer
            la racine carrée.

  License: libre pour usage gratuit
  Throws: Ne déclenche aucune exception.
  Returns: la racine carrée de l'entrée.
*/
T sqrt(T)(T number) {
}
```
