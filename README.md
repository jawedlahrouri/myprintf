[![Academic Year](https://img.shields.io/badge/Epitech-Tek1-blue?style=for-the-badge&logo=epitech&logoColor=white)](https://www.epitech.eu/)
[![Language: C](https://img.shields.io/badge/Language-C-00599C.svg?style=for-the-badge&logo=c)](https://en.wikipedia.org/wiki/C_(programming_language))
[![Module](https://img.shields.io/badge/Module-B--CPE--101-informational?style=for-the-badge)](#)

# 🖨️ MyPrintf — Moteur d'Écriture Formatée en C (printf clone)

**MyPrintf** est une réimplémentation complète et optimisée de la fonction de la bibliothèque C standard `printf`. Packagée sous la forme d'une bibliothèque statique autonome `libmy.a`, elle gère les arguments variadiques (`<stdarg.h>`), la conversion de bases numériques et le formatage de chaînes.

---

## 🎯 Spécificateurs de Conversion Supportés

| Spécificateur | Description du Type & Sortie |
|---|---|
| `%c` | Caractère simple (`char`). |
| `%s` | Chaîne de caractères (`char *`). |
| `%d`, `%i` | Entier relatif signé en base 10 (`int`). |
| `%u` | Entier naturel non signé en base 10 (`unsigned int`). |
| `%o` | Nombre non signé converti en base octale (base 8). |
| `%x` | Nombre non signé converti en base hexadécimale minuscule (`0-9a-f`). |
| `%X` | Nombre non signé converti en base hexadécimale majuscule (`0-9A-F`). |
| `%p` | Pointeur d'adresse mémoire affiché en hexadécimal préfixé par `0x`. |
| `%%` | Caractère pourcent littéral échappé. |
| Drapeau Espace (`' '`) | Préfixe les entiers positifs par un espace d'alignement. |

---

## 🛠️ Compilation de la Bibliothèque

```bash
make        # Génère la bibliothèque statique 'libmy.a'
make clean  # Supprime les fichiers objets temporaires
make fclean # Supprime les fichiers objets et la bibliothèque libmy.a
make re     # Recompile l'ensemble
```

---

## 💡 Exemple d'Utilisation

```c
#include "my.h"

int main(void)
{
    int score = 42;
    char *user = "Student";

    my_printf("Hello %s ! Votre score est de %d (hex: 0x%x)\n", user, score, score);
    return 0;
}
```
