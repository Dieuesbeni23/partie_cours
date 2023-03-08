ALGORITHME Voyelle;

VARIABLE
text : caractère ; 
i, j, nbr, nbr1 : entiers;

DEBUT
nbr = 0;
nbr1 = 0;
Ecrire("Veillez saisir une phrase");
Lire(text);
Pour i <- 0 à len(text)
	si mid(text, i, 1) = " " alors
		nbr <- nbr +1;
	Finsi
Finpour

Ecrire("Le nombre de mot est", nbr);
Pour j <- 0 à len(text);
	si mid(text, i , 1) = "a" ou si mid(text, i, 1) = "e"
	ou mid(text, i , 1) = "o" ou si mid(text, i, 1) = "u"
	si mid(text, i , 1) = "y" ou si mid(text, i, 1) = "i" alors
		nbr1 <- nbr1 +1
	Finsi
Finpour
Ecrire ("Cette phrase comte",Nbr1 ,"voyelle");
FIN


ALGORITHME Somme_disticnt

VARIABLES 
Tab1 : Tableau [i] entier;
Tab2 : Tableau [j] entier;
j,i,Somme,Valeur_identique, Valeur_distinct : entiers;

DEBUT 
Somme <- 0;
Pour i allant de 0 à (n-1) faire
	Ecrire("Complétez le tableau", i+1);
	lire(Tab[i]);
Finpour
Pour j allant de 0 à (n-1) faire
	Ecrire("Complétez le tableau", j+1);
	lire(Tab[j]);
Finpour 
si (Tab[i] = Tab[j]) alors
	valeur_identique <- Tab[i] = Tab[j];
sinon 
	Valeur_distinct <-  Tab[i] <> Tab[j]; 
	Somme <- Somme + Valeur_distinct
Finsi
Ecrire(Somme,"élements disctinct", Valeur_distinct);
FIN
