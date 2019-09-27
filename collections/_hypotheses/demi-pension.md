# Demi Pension


## Proposer aux familles d'autoriser le prélèvement des frais de demi-pension

formulaire existe dans la version d'Etienne ANDRE du DossierSCO Access.

---

## configurer le nombre de jours de demi-pension

>  Christophe Robillard @krichtof · 2 months ago
> 
> En tant qu'admin d'un établissement, j'aimerai demander aux familles qui s'inscrivent à la demi-pension si c'est pour 4 jours ou 5 jours par semaine.
> 
> Demandé notamment par le collège Pierre Mendès-France

A voir, peut-être qu'utiliser le système de régime de demi-pension proposé dans le fichier XML (structure ou nomenclature ?) de SIECLE serait suffisant.

---

##  Collecter les identifiants bancaires des responsables financiers estimant bénéficier d'une bourse

Je le pose ici vis à vis de la demi-pension, bien que ça parle de bourse.
Je le colle aussi dans [champs_obligatoires.md](champs_obligatoires.md)

- Solution simple : en faire une pièce attendue téléchargeable (IBAN)
- à noter : refus du téléservice des bourses de recueillir la saisie de l'IBAN par les familles (casus belli avec Bourse.beta)
- Action diplomatique : indiquer aux familles le lien vers le simulateur de bourse du ministère


---

Inscrire à la cantine avec tarification QF


En tant qu'agent, je souhaite connaitre le quotient familial d'une famille.
Pour ce faire, la famille doit indiquer son numéro d'allocataire ainsi que son code postal.

Le quotient familial est disponible grâce à Api Particulier. Voir [la documentation technique](https://api.gouv.fr/api/api-particulier.html#doc_tech)



Contexte
--------

Irritant important pour l'intendance

### Process actuel (papier) : 
Le Département de Paris (service DASCO) obtient de la CAF les QF des collégiens, envoie la notification aux familles par courrier postal. Les collèges demandent copie de la notification au  moment de l'inscription. Conséquence négative pour les familles : application du tarif de cantine le plus élevé, en l'absence de notification. Pour les agents : relances fastidieuses pour obtenir le QF, puis pour le recouvrement des créances.

### Process DossierSCO 2018 : la famille télécharge la notification par smartphone. Questions non réglées :
- l'irritant des avis manquants demeure
- l'intendance voit un double flux de notifications (papier et photo sur dossierSCO). Comment simplifier  ?

### Process par API particulier
Après autorisation par la DINSIC, APIpart donne un token a l'établissement qui permet de consulter les QF des familles, avec l'identifiant CAF préalablement récupéré sur DossierSCO.

- [x] demander l'accès à l'API pour lycée Arago
- [ ] tester avec une famille
- [ ] industrialiser




>  Pierre de MAULMONT @Pierre2Maulmont · 6 months ago
> 
> Demande d'autorisation d'accès à APIpart, pour le lycée ARAGO, postée le 13/1/19, pour les données QF, avis d'imposition, adresse d'imposition. Attente de la réponse du Pole juridique de la DINSIC.


>  Pierre de MAULMONT @Pierre2Maulmont · 6 months ago
> 
> Contact pris avec 1er adjoint à la maire de Paris Objectif : constituer un plan B pour récupérer directement les QF des familles, si autorisation d'accès des collèges par APIpart s'avérait trop compliquée


>  Pierre de MAULMONT @Pierre2Maulmont  · 2 months ago
> 
> Demande validée le 2 mai par API.gouv


>  Lucien @LucienMLD · 2 months ago
> 
> Faut-il demander l'identifiant CAF. Comment faire la requête pour API ?


>  Christophe Robillard @krichtof · 2 months ago
> 
> La doc est ici : https://api.gouv.fr/api/api-particulier.html#doc_tech


