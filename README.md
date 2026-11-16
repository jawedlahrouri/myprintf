# 🖨️ MyPrintf — Formatted Output Printing Engine in C

[![Academic Year](https://img.shields.io/badge/Epitech-Tek1-blue?style=for-the-badge&logo=epitech&logoColor=white)](https://www.epitech.eu/)
[![Module](https://img.shields.io/badge/Module-B--CPE--101-informational?style=for-the-badge)](#)
[![Language](https://img.shields.io/badge/Language-C-00599C?style=for-the-badge&logo=c&logoColor=white)](#)

## 📘 Description
**MyPrintf** est une réécriture complète de la fonction standard `printf` de la bibliothèque C libc (`stdio.h`). Développé en utilisant les fonctions variadiques (`<stdarg.h>`), il gère la conversion et le formatage dynamique de chaînes, entiers, nombres flottants et pointeurs.

## ⚙️ Spécificateurs gérés
- `%d`, `%i` : Entiers signés en base décimale.
- `%u` : Entiers non-signés.
- `%s`, `%c` : Chaînes de caractères et caractères uniques.
- `%o`, `%x`, `%X` : Nombres en base octale et hexadécimale (minuscule / majuscule).
- `%p` : Adresses de pointeurs mémoire.
- `%b` : Conversion en base binaire.
- `%%` : Échappement du caractère pourcentage.
- Modificateurs de précision, de champ et de drapeaux (`#`, `0`, `-`, `+`).

## 🔨 Compilation
```bash
make
# Génère la bibliothèque statique libmy.a
```
