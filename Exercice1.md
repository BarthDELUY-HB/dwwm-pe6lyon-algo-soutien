# Exercice 1

## Énoncé
Exercice 1 : CONDITIONS
Difficulté : 1*
a) Écrire un algorithme qui :
- reçoit en paramètres deux nombres différents,
- et renvoie le plus grand des deux.
b) Même exercice avec trois nombres distincts.
c) Même exercice avec quatre nombres distincts. 

## Correction
a.
/*
    Comparer 2 nombres et renvoyer le plus grand
        => renvoyer 1 des deux

        CN1 : comparer2Nombres(4,1) => 4 (1ère position)
        CN2 : comparer2Nombres(1, 4) => 4 (2ème position)
*/
FONCTION comparer2Nombres(var nb1, var nb2)
DÉBUT
    SI nb2 > nb1 ALORS
        Renvoyer nb2
    FINSI
    Renvoyer nb1
FIN

b.
/*
    Comparer 3 nombres et renvoyer le plus grand
        => renvoyer 1 des trois
*/
FONCTION comparer3Nombres(var nb1, var nb2, var nb3)
DÉBUT
    SI nb2 > nb1 ET nb2 > nb3 ALORS
        Renvoyer nb2
    FINSI
    SI nb3 > nb1 ET nb3 > nb2 ALORS
        Renvoyer nb3
    FINSI
    Renvoyer nb1
FIN

c.
/*
    Comparer 4 nombres et renvoyer le plus grand
        => renvoyer 1 des quatre
*/
FONCTION comparer4Nombres(var nb1, var nb2, var nb3, var nb4)
DÉBUT
    SI nb2 > nb1
        ET nb2 > nb3
        ET nb2 > nb4 ALORS
        Renvoyer nb2
    FINSI
    SI nb3 > nb1
        ET nb3 > nb2
        ET nb3 > nb4 ALORS
        Renvoyer nb3
    FINSI
    SI nb4 > nb1
        ET nb4 > nb2
        ET nb4 > nb3 ALORS
        Renvoyer nb4
    FINSI
    Renvoyer nb1
FIN