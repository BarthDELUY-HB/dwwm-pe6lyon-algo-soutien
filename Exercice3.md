# Exercice 3

## Énoncé
Exercice 3 : BOUCLES 
Difficulté : 1*
Écrivez la routine afficherÉtoiles( var nb_étoiles) qui reçoit en paramètre un entier positif et affiche à l'écran un nombre d'étoiles identiques à cette valeur.
Exemple : afficherÉtoiles(3) => ***

## Correction
/*

    CN1 : afficherÉtoiles(0) => 
    CN2 : afficherÉtoiles(1) => *
    CN3 : afficherÉtoiles(3) => ***
*/
PROCÉDURE afficherÉtoiles( var nb_étoiles)
DÉBUT

    TANT QUE nb_étoiles > 0 FAIRE
        Afficher '*'
        nb_étoiles <- nb_étoiles - 1
    FIN TANTQUE

FIN