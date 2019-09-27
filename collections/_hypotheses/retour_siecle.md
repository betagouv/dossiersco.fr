# Retour Siecle

Problématique de parent ayant rempli deux fois (à la place de l'autre), et
perte des informations du père dans SIECLE au moment de l'import 

La date de début de scolarité n'est pas bonne, elle causera un blocage en fin
d'année :

> pour info, une mauvaise date de début d'année scolaire bloque, en fin
> d'année, la remontée vers LSU, vers AFFELNET, vers le DNB etc... 
-- Un membre de l'académie de Paris

Après le retour d'un établissement dans SIECLE :
> Des élèves ont perdu toutes leurs options, d'autres sont devenus orphelins et
> n'avaient plus de parents rattachés. C'est d'ailleurs ce qui a été perçu tout
> de suite et corrigé rapidement

Rencontre demandé pour lister les cas, et regarder ensuite comment progresser.


Un autre établissement dans l'académie de Nancy-Metz :

> côté établissement, le bilan est très négatif : toute notre base SIECLE est à
> reprendre
> 
> - tous les Madame sont passés Monsieur
> - Des mères séparées ont saisi leurs coordonnées 2 fois en sélectionnant 2
>   fois le lien mère (les père ont donc disparu de notre base)
> - Lorsque les mères ont changé leur nom (jeune fille ou épouse) cela défait
>   les liens des fratrie
> - etc...

Rencontre prévu mardi 10 pour avoir plus de détails.

---


On 16/09/2019 16:35,
> Encore un problème décelé aujourd’hui : l’import de dossiersco dans
> siècle a écrasé l’établissement d’origine de nos élèves entrant en sixième.
> Ils apparaissent tous comme étant originaires (...) de notre établissement
> (...) alors qu’on devrait avoir mention de leur école de provenance.

---

[retour SIECLE] Renseigner les ID_PRV_PER de ELEVE et PERSONNE avec PERSONNE_ID

Pour les représentants légaux qui existent déjà dans siecle (renseignés dans ResponsablesAvecAdresses.xml), utiliser le champs PERSONNE_ID dans ID_PRV_PER plutôt que notre identifiant interne resp_legal_id :

    <PERSONNE PERSONNE_ID="XXXXXXX">

Pour celles qui ne sont pas représentées dans siecle (crées dans DossierSCO), continuer à utiliser resp_legal_id.

Le retour de test à l'origine de cette évolution :

> 
> ERREUR GRAVE : Veuillez faire correspondre les ID_PRV_PER de ELEVE avec les ID_PRV_PER de PERSONNE
