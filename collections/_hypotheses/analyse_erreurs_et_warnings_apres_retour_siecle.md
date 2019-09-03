# Analyse erreurs et warnings après retour SIECLE


## Fiches Responsables et Correspondants importées avec anomalies

### Les téléphones

- TELEP_E_01 : Le numéro de tel fixe personnel renseigné "1234567890123" ne correspond ni à un format français ni à un format étranger. Celui-ci a quand même été pris en compte.

Les téléphones peuvent avoir un format non reconnus. Par contre, ils ne doivent pas contenir autre chose que des chiffres.

## Fiches élèves rejetées

- REJEL_ENTREE_B_02 : La date d'entrée "09/01/2016" est incohérente avec une scolarité (du 01/09/2015 au 31/08/2016) se passant dans un autre établissement. L'élève a été rejeté.

Bug siecle qui prend les dates au format anglais ?

## Fiches élèves importées avec anomalies

- ACDIV_B_01 : La division indiquée n'est pas rattachée au MEF de l'élève. La scolarité active de l'élève a été rejetée.

Comment avons récupéré la division ? N'était-elle pas attaché à un MEF ?

- MODCH_B_02 : Le nombre d'options obligatoires présentes dans le fichier est inférieur à celui imposé par le mef. Les options n'ont pas été prises en compte.

- MODCH_B_03 : Le nombre d'options obligatoires présentes dans le fichier est supérieur à celui imposé par le mef. Les options n'ont pas été prises en compte.

- INOPT_B_01 : Il n'existe aucun programme pour un code Mef "16710002110", un matico "347400" et un code modalité élection "O" . Les options n'ont pas été prises en compte.

- SCOPR_C_04 : La scolarité précédente envoyée (du 03/09/2018 au 01/09/2019) chevauche une autre scolarité présente dans SCONET (du 03/09/2018 au 02/04/2019). La scolarité an dernier n'a pas été prise en compte.

- SCOAC_F_01 : Le code MEF "10310019110" de l'élève est identique au code mef de la scolarité précédente pour ce même élève et dans la même année. La scolarité active, les motif et date de sortie n'ont pas été pris en compte.

Cas de l'élève redoublant ? Comment le signaler ? Il y a une balise dans SIECLE pour ça.

- OPOBL_C_01 : L'option "084300" de rang "2" n'est pas permise en tant qu'option obligatoire. Les options n'ont pas été prises en compte.

## Fiches Responsables et Correspondants importées avec anomalies

- PEPCS_B_01 : Ce représentant légal de l'élève ayant pour identifiant privé 99999, a pour lien avec l'élève Aide Sociale à l'Enfance. Son code PCS a été initialisé à 99 (profession non renseignée).

Dans le cas de certains liens (ici Aide Sociale à l'Enfance) il faut fournir un code PCS (profession ?) ? Est-ce que le PCS est le code profession ?

- PUSAG_A_01 : Le nom d'usage est identique au nom de famille, il ne sera donc pas pris en compte.


