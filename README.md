Description
Ce projet consiste à recréer la fonction printf de la bibliothèque standard stdio.h, en utilisant uniquement la bibliothèque stdarg.h pour la gestion des arguments variadiques et la fonction write de unistd.h pour l'affichage.

L'objectif est de reproduire les mêmes fonctionnalités et la même valeur de retour que la fonction originale.

Ce projet, entièrement réalisé en C, m'a permis de mieux comprendre l'utilisation de la bibliothèque stdarg.h, ainsi que le fonctionnement interne de la fonction printf.

Utilisation
Cloner le projet

Dans votre terminale :
  git clone git@github.com:herirand/FT_PRINTF.git
  cd FT_PRINTF

Tester la bibliothèque
Comme il s'agit d'une bibliothèque que vous pouvez intégrer dans vos projets, vous devrez créer un fichier main.c pour tester son fonctionnement. Voici un exemple simple de fichier :

Copier le code
#include "ft_printf.h"

int main(void)
{
    ft_printf("Test de ft_printf : %s\n", "fonctionne !");
    return (0);
}

Compiler et exécuter
Vous avez deux options pour compiler et tester la bibliothèque :

*Utiliser make
Si vous avez déjà votre propre code ailleurs, vous pouvez générer uniquement la bibliothèque avec :
  make

*Compiler directement avec gcc
Si vous souhaitez tester rapidement avec un fichier main.c :

  gcc ft_printf.c ft_printf_utils.c main.c -o test_ft_printf
  ./test_ft_printf
  
Ce projet est une excellente ressource pour mieux comprendre les bases du C et l'implémentation de fonctionnalités avancées avec des arguments variadiques. 🚀
