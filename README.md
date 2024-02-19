<h1 align="center">
Coding club - Petit Bain
</h1>

</br>

## Prérequis 🔑

Si vous êtes sur un ordinateur du Coding-Club, exécutez cette commande pour charger le sujet `sudo rebuild petit-bain`. Vous pouvez sauter cette section, ces prérequis sont remplis automatiquement.

Sinon pour pouvoir suivre cette activité, vous devez avoir installé sur votre ordinateur:

- Un éditeur de code (Visual Studio Code)
- Un terminal (bash, powershell)
- Un compilateur C (gcc)

## Les Règles 🧾

- Toute IA est interdite; ChatGPT, Google Bard, Bing AI, Github Copilot, etc.
- Toute forme de plagiat est interdite; vous devez écrire votre code vous-même.
- Vous pouvez utiliser internet pour chercher de l'aide, mais vous ne pouvez pas copier/coller du code.
- Seule la fonction  `write` est autorisée pour ces exercices.
- Jouez le jeu, les conditions en piscine seront pire 😉

# Exercices 📝

## 0 - Hello World! ✨

Fichier: `hello_world.c`

Pour cet exercice "0" le code vous est donné, essayez de le-comprendre et n'hésitez pas à poser des questions sur son fonctionnement.

```c
void hello_world(void)
{
  write(1, "Hello World!", 12);
}
```

Pour comprendre ce bout de code n'oubliez pas [l'annexe sur le langage C](./Annexe-C).
Vous y trouverez plus d'informations sur les grandes lignes du C, sa syntaxe et surtout comment compiler et exécuter son code !
## 1 - my_print_alpha 🔡

Fichier: `my_print_alpha.c`

Ecrivez une fonction qui, en commençant par `a`, affiche l'alphabet dans l'ordre alphabétique, sur une seule ligne.

**Affichage attendu:**

`abcdefghijklmnopqrstuvwxyz`

**Prototype de la fonction:**

```c
void my_print_alpha(void);
```

> [!TIP]
> Pour l'instant votre terminal s'affiche à la suite de votre ligne de lettres, c'est normal. Si vous le souhaitez vous pouvez chercher sur internet comment régler ce problème. *Un fameux caractère '\n' pourrait vous aider.*

## 2 - my_ispos ➕

Fichier: `my_ispos.c`

Ecrivez une fonction qui écrit `"P"` si le chiffre donné en paramètre est positif *(ou nul)*, ou `"N"` s'il est négatif.

**Appel de la fonction:**
```c
my_ispos(-42);
my_ispos(42);
```

**Affichage attendu:**

`N`
`P`

Prototype de la fonction:

```c
int my_ispos(int n);
```

> [!TIP]
> Les deux caractères sont sur la même ligne ? Regardez le TIP de l'exercice précédent, il vous sera d'une grande aide.

## 3 - my_putnbr 🔢

> [!IMPORTANT]
> Désormais la difficulté des exercices va rapidement augmenter ! Pas d'inquiétude si vous vous retrouvez coincé, les cobras sont là pour vous aider.

Fichier: `my_putnbr.c`

Ecrivez une fonction qui afficher le nombre donné en paramètre *(en utilisant toujours uniquement `write`)*.

**Appel de la fonction:**
```c
my_putnbr(-42);
my_putnbr(0);
my_putnbr(-2147483647);
```

**Affichage attendu:**

`-42`
`0`
`-2147483647`

Prototype de la fonction:

```c
void my_putnbr(int n);
```

## 4 - my_putstr 🖨️

Fichier: `my_putstr.c`

Ecrivez une fonction qui affiche, un-par-un, les caractères d'une chaîne de caractère.
L'adresse du premier caractère de la string est donné en tant que pointeur en paramètre.

Cette fonction doit **renvoyer** une valeur, ne l'oubliez pas !

**Appel de la fonction:**
```c
my_putstr("Hello World!");
my_putstr(" Wow!\n");
```

**Affichage attendu:**

`Hello World! Wow!`

**Retour(s) attendus:**

| Valeur | Type |
| :--: | :--: |
| 84 | Pointeur invalide |
| 0 | Fini avec succès |

Prototype de la fonction:

```c
int my_putstr(char const *str);
```

> [!TIP]
> Chaîne de caractère, valeur de retour, kesako ? Lisez l'annexe pour plus d'informations sur toutes ces notions.
## 5 - my_swap 🔄️

Fichier: `my_swap.c`

Ecrivez une fonction qui échange le contenu de deux pointeurs d'entiers passés en paramètre.

Prototype de la fonction:

```c
void my_swap(int *a, int *b);
```

## 6 - my_getnbr 🔟

Fichier: `my_getnbr.c`

Ecrivez une fonction qui lit une chaîne de caractère et retourne le nombre entier contenu dans celle-ci.
La fonction doit être capable de fonctionner avec les nombres négatifs.

**Appel de la fonction:**
```c
my_getnbr_base("-42");
```

**Retour attendu:**

```c
-42
```

| Valeur | Type |
| :--: | :--: |
| -84 | Pointeur invalide / Chaîne de caractère invalide |
| 0 | Chaîne de zéro charactère donné |
| >= 1 | Valeur de la chaîne de caractère |
|  |  |

Prototype de la fonction:

```c
int my_getnbr_base(char const *str);
```

## Fini? 🏁

Il vous reste deux défis à accomplir pour pouvoir réellement dire que vous avez roulé sur le Petit Bain: [star](./star.pdf) et [mini-printf](./mini-printf.pdf).

> [!NOTE]
> Ces deux sujets sont entièrement rédigés en Anglais, **comme tous les sujets à Epitech**.