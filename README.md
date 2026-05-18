Algorithme AnalysePhrase hd

Variables :
    caractere : caractère
    longueur, mots, voyelles : entier

Début

    longueur ← 0
    mots ← 1
    voyelles ← 0

    Lire(caractere)

    TantQue caractere <> '.' Faire

        longueur ← longueur + 1

        Si caractere = ' ' Alors
            mots ← mots + 1
        FinSi

        Si caractere = 'a' OU
           caractere = 'e' OU
           caractere = 'i' OU
           caractere = 'o' OU
           caractere = 'u' OU
           caractere = 'y' Alors

            voyelles ← voyelles + 1

        FinSi

        Lire(caractere)

    FinTantQue

    Afficher("Longueur de la phrase : ", longueur)
    Afficher("Nombre de mots : ", mots)
    Afficher("Nombre de voyelles : ", voyelles)

Fin
