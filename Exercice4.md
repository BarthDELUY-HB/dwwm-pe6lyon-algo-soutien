# Exercice 4

## Énoncé
Exercice 4 : BOUCLES
Difficulté : 2*
Écrivez la routine afficherÉtoilesMultiligne(var nb_étoiles) qui reçoit en paramètre un entier positif, et affiche un triangle d'étoiles dont le nombre de lignes est identique à cette valeur.
Exemple : afficherÉtoilesMultilignes(3) =>
*
**
*** 


## Correction
/*
    CN1 : afficherÉtoilesMultiligne(1) => *
    CN2 : afficherÉtoilesMultiligne(2) =>   *
                                            **
    CN3 : afficherÉtoilesMultiligne(3) =>   *
                                            **
                                            ***

    Étapes : 
            -> afficher une étoile par ligne mais le bon nombre de lignes
            -> mettre le bon nombre d'étoiles sur la ligne
*/
PROCÉDURE afficherÉtoilesMultiligne(var nb_étoiles)
DÉBUT
    Déclarer ligne_courante <- 1
    TANT QUE nb_étoiles > 0 FAIRE
        afficherÉtoiles( ligne_courante )
        Aller à la ligne
        ligne_courante <- ligne_courante + 1
        nb_étoiles <- nb_étoiles - 1
    FIN TANTQUE

FIN