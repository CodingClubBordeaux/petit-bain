<h1 align="center">
Coding club - Annexe sur le C
</h1>

</br>

# Bases du langage C

Le C est un langage de programmation de bas niveau réputé pour sa rapidité et son efficacité en mémoire. Les blocs de code sont délimités par des curly-brackets *{* et *}*, les déclarations se terminent par un *;*

## Variables et types de données:

En C, vous pouvez créer des variables pour stocker différentes sortes de données, comme des nombres, des chaînes de caractères, des tableaux etc. Les noms de variables sont sensibles à la casse et doivent commencer par une lettre ou un soulignement. Ces variables doivent être d'un certain type, le type définit quel type de valeur pourra être stocké dans cette variable. Voici quelques examples:

```c
int nombre_entier = 42;
float nombre_decimal = 3,14;
char *chaine_de_charactere = "Hello World!";
int tab_de_nombre[] = [42, 84, 128];
```

## Opérations de base:

Le C prend en charge les opérations mathématiques de base (+, -, \*, /) ainsi que les opérations logiques (&&, ||, !). Voici quelques examples:

```c
somme = 5 + 3;
difference = 10 - 2;
produit = 4 * 6;
quotient = 12 / 3;

vrai_et_faux = true && false;
vrai_ou_faux = true || false;
non_vrai = !true;
```

## Structures de contrôle:

Le C propose des structures de contrôle telles que les boucles (for, while) et les instructions conditionnelles (if, else) pour gérer le flux d'exécution du programme.

```c
for (int i = 0; i < 5; i += 1) {
  printf("%d\n", i);
}

int x = 0
while (x < 5) {
  printf("%d\n", i);
  x += 1;
}

if (nombre > 10) {
  printf("Nombre superieur a 10\n");
}
else if (nombre == 10) {
  printf("Nombre egal a 10\n");
}
else {
  print("Nombre inferieur a 10\n");
}
```

## Fonctions:

Les fonctions sont des blocs de code réutilisables qui effectuent une tâche spécifique. Elles peuvent prendre des paramètres en entrée et renvoyer une valeur en sortie. Les fonctions doivent préciser le type de chacun de leur paramètre et de leur retour.

```c
int carre(int x) {
  return (x * x);
}
```

## Tableaux et boucles :

Les tableaux en C permettent de stocker plusieurs valeurs du même type. Ils sont indexés à partir de zéro. Par convention, les tableaux de pointeurs sont terminés avec une cellule supplémentaire contenant un pointer vers NULL; 

```c
int nombres[4] = {1, 2, 3, 4};
for (int i = 0; i < 4; i++) {
    printf("%d\n", nombres[i]);
}
```