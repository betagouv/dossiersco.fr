# Protocole d'évaluation de DossierSCO

## Préambule 

L'objet de ce document est de faire un retour d'expérience de l'expérimentation DossierSco et d'évaluer les conditions de sa généralisation. 
 
Dossiersco permet aux parents d'élèves inscrits au collège d'inscrire leurs enfants simplement sur internet. Cela leur permet en général de pouvoir faire la démarche sans avoir à se déplacer dans l'établissement, sans poser une demie journée de congé. Les familles plus en difficulté bénéficient également de DossierSCO, puisque l'établissement a moins à s'occuper des familles à l'aise avec le numérique, les agents peuvent prendre du temps pour aider les familles qui en ont besoin.

Certains établissements utilisent DossierSCO pour faciliter la partie administrative de l'inscription et de la re-inscription, pour passer plus de temps avec les familles sur les aspects pédagogiques, lors d'une réunion en  fin de journée par exemple.

Le service permet aux établissements de gérer simplement la campagne d'inscription et ses éventuelles relances. 

DossierSCO facilite la partie administrative pour permettre aux établissements d'avoir une relation de meilleure qualité avec les familles (et inversement).

Les éléments de diagnostic du problème ont été sondés auprès des étabissements pilotes. Le déploiement et les retours utilisateurs se font au fur et à mesure. 

## Résultat de l'expérimentation 

| Nb de collèges        | 2018  | 2019   | Evolution |
| :-------------------- | :---: | -----: | :-------: |
| Contactés             |       | 300    | 
| Inscrits à DossierSCO |       | 105    |
| Expérimentateurs      |       | 44     |
| Utilisateurs          | 4     | 24     | +600%

| Nb élèves             | 2018  | 2019   | Evolution |
| :-------------------- | :---: | -----: | :-------: |
| Inscrits à DossierSCO | 750   | 8000   | +1000%    |


Malgrè une croissance substancielle des usagers, on note un taux d'activation de 25% sur les établissements inscrits. 

La satisfaction moyenne sur la 2ème saison est de 4,2. 80% des parents ont pris le temps de donner leur satisfaction.
81% des parents sont satisfaits ou très satisfaits de DossierSCO.

A la question _l'année prochaine souhaitez-vous continuer à utiliser DossierSCO ou bien revenir au papier_, 87% des parents répondent préférer utiliser DossierSCO l'année prochaine.

### Le problème 

Les familles :

- doivent poser une demi-journée (au moins) de congé pour venir à la journée d'inscription  .
- remplissent des documents avec des informations déjà connus de l'administration
- n'ont pas un accueil personnalisé et/ou de qualité avc les établissements lors de l'inscription (puisque les toutes les familles font la queue pour déposser leur dossier).

_Informations récolté auprès de 12 familles ayant effectué des tests utilisateurs et des interviews lors de la première saison d'expérimentation et de 5 indétendants_

Les établissements utilisent un ETP d'environ 20 jours pour préparer la journée d'inscription : 

- photocopies
- organisation des plannings
- définition des pièces
- organisation des rôles de chaque personne intervenant le jour J
- journée d'accueil mobilisant une bonne partie de l'établissement
- ressaisie dans SIECLE des informations collectées
- relance des familles n'étant pas venues ou n'ayant pas amené les bonnes pièces

_Informations récolté auprès des 4 établissements parisien embarqué pour la première saison d'expérimenttion_

Joindre les familles à l'inscription. Les établissements n'avaient pas, avant DossierSCO, de capacité d'envoyer en masse des sms, canal qui s'avère particulièrement efficace notamment auprès des familles les plus en difficulté. 

### Fonctionnalités du produit durant cette phase d'expérimentation


| Fonctionnalités        | DossierSCO | Fiche de Renseignement | Insciption (lycée pou l'instant) |
| :--------------------- | :--------: | :--------------------: | :---------------: |
| modifier les informations de l'élève | x | x |  |
| choisir des options pédagogiques | x |  | x |
| modifier les informations des responsables légaux | x | x | |
| visualiser et modifier les informations d'un seul responsable légal | | x | x |
| signaler un suivi médical particulier | x |  |  |
| récupération des identifiant CAF | x | | |
| autorisation photo de classe | x | | |
| fournir des pièces jointes | x | | |
| validation des modifications avant intégation dans la BEE | x | x | x |
| (recolte du fedback des parents) | x | | | 
| inscription autonome des établissements à l'application | x | x | x |
| générer un questionnaire médical pré-rempli | x | | |
| environnement de démonstration avec données anonymisées | x |  |  |
| déduction de la carte des formations à partir de l'export SIECLE EleveComplete.xls | x | ne s'y prête pas | |
| modification de la carte des formations (création et mise à jour de mef et d'options) | x |  | x |
| définir les règles d'accès aux options | x | | x |
| générer les convocations (papier, email et sms) | x | | |
| contacter les familles (pour relance ou aute) par email et sms | x | | |

L'objectif n'est pas de refaire la fiche de renseigment (nous pourrions peut-être construire un lien vers cette fiche), mais plutôt d'aider les établissements à gérer la vie scolaire, les besoins administratifs, pour faciliter la relation entre les élèves, les parents et les agents.


Les inscriptions en 6ème (718 élèves validés dans 5 établissements) ont été traités en plus des réinscriptions en 5ème, 4ème et 3ème.

Un établissement est considéré comme :
- inscrit lorsqu'il a fournit son UAI sur le site dossiersco.fr (avant d'avoir cliqué sur le lien d'activation reçu par mail). 
- expérimentateur lorsqu'il a réussi à importer la base SIECLE.
- utilisateur lorsque des familles se sont connectées sur dossiersco.fr. 


#### Comment les parents s'inscrivent ?

Le téléphone portable est le canal le plus fiable pour joindre les familles (plus de 95% des familles sont joignables par sms). La relance par sms en fin de campagne permet ainsi de finaliser l'inscription de 96% des élèves. 
  
L'objectif est d'éviter toute ressaisie de la part des établissements.

Le moyen d'y parvenir est : 
1/ D'importer dans DossierSCO le fichier xml de nomenclature (incluant les options et les MEF)
2/ De générer un fichier xml d'import privé à télécharger dans la section "mise à jour" de SIECLE

L'objectif est que les données aient été rapatriées dans SIECLE avant la rentrée.

## Stratégie de déploiement

### Openlab

Un openlab a réuni une trentaine de personnes au lab 110 bis.
L'intrapreuneur a invité des personnes qu'il connaissait dans ses différents réseaux étendus.
Les personnes présentes sont venues par curiosité et certaines ont été convaincues par la culture de l'équipe qu'elles ont découvert à cette occasion. Elles ont pu constater que l'équipe s'intéressait aux utilisateurs.


### Autonomisation des établissements

L'ouverture du processus d'inscription a procuré une autonomie au segment d'établissements souhaitant s'inscrire à DossierSCO sans passer par une formation.

### Environnement de démonstration

Un environnement de démonstration avec des données anonymisées et une connexion facilitée a été mis en place pour que les établissements se rendent compte de l'expérience utilisateur aussi bien coté famille que coté agent avant de s'inscrire.

### Démarchage

L'intrapeneur a envoyé un mail à 10 établissements par académie, soit 300 établissements début mai.

Des appels ont été réalisés par des membres de l'équipe aux établissements inscrits.
Des ambassadeurs particulièrement actifs ont fait la publicité de DossierSCO dans leur accadémie, comme à Montpellier ou le collège La Garriguette a été très actif.
Sur l'accadémie de Paris, une stratégie particulière a été mise en place :
- la connexion était possible directement par l'ENT
- l'accadémie a elle-même invité les établissements de Paris à participer à l'expérimentation

### Hypothèses testées ou à tester

En reprenant la méthode d'analyse des produits numériques AARR, nous pourrions analyser nos hypothèses pour chaque étape :
- Acquisition : inscription d'un compte
- Activation : passage d'une inscription (ou d'un email d'intérêt) à au moins une classe sur DossierSCO
- Rétention : l'établissement reste d'une année sur l'autre
- Recommendation : l'établissement recommande le produit

| Etapes de la conversion | Testé et validé  | Testé et invalidé   | A tester |
| :-------------------- | :---: | -----: | :-------: |
| Acquisition | - Cibler des établissements impliqués dans le numérique (3/5 utilisateurs)<br/>  - Avancer d'une semaine la remontée dans SIECLE des nomenclatures pour les inscriptions en 6ème (a convaincu un établissement de l'académie de Créteil) | - Envoi massif d'emails à toute une académie (Paris: 15 inscrits sur 70 mails)<br/> - Se reposer sur la diffusion par l'académie (Paris, forte implication pourtant)<br/> - Se reposer essentiellement sur l'envoi d'emails<br/> - S'adresser à des utilisateurs qui n'ont pas le profil d'early-adopters pendant la phase d'expérimentation  | - Différents objets d'email, corps d'email<br/> - Démarchage par téléphone<br/> - Récupérer des listes d'établissements pro-numériques dans toutes les académies<br/> - Courrier postal avec brochure présentant DossierSCO<br/> - Inviter à un événement local pour présenter le produit<br/> - S'adresser à la presse spécialisée<br/> - Passer par les associations de parents d'élèves |
| Activation | - Onboarding autonome pour X établissements<br/> - Appel suite à l'inscription (condition à passer le pas de l'utilisation)<br/>  - Accompagner au téléphone sur démo pour tester une étape risquée (1 inscription des 6ème "gagnée") | - Appel après impression des convocations parents | - Renfort de 2 personnes pendant 2 mois pour recruter et accompagner les établissements<br/> - S'appuyer sur les ambassadeurs (les citer)<br/> - Formation des gestionnaires d'établissement<br/> - Proposer systématiquement un accompagnement à l'onboarding (téléphone ou face-à-face)
| Rétention  | - Appeler ou aller voir tous les établissements de l'an passé (rétention 75%) | Changement de personnel dans l'établissement qui fait sortir l'établissement du segment des early-adopters | - Recueil de feedbacks produit suite à la période des inscriptions, pour revenir avec un produit qui correspond mieux aux besoins<br/> - Questionnaires auprès des familles utilisatrices pour savoir comment améliorer le DossierSCO<br/> - Demander des témoignages écrits pour que les agents conscientisent ce qu'ils/elles ont apprécié dans DossierSCO. Un an plus tard, on pourra leur rappelé leur propre témoignage pour les convaincre de réutiliser DossierSCO
| Recommandation | - | - | - Organiser une démonstration /REX en local par des établissements utilisateurs<br/> - Demander aux utilisateurs des contacts d'établissements au profil early-adopters (voire une introduction)<br/> - Demander aux utilisateurs qu'ils parlent en bien de DossierSCO à la DSI et à l'académie<br/> - Communiquer sur les retours des établissements utilisateurs |

![](https://pad.etalab.studio/uploads/upload_468d3e89ffa3062c0f43a781e5081768.png)


![](https://pad.etalab.studio/uploads/upload_14ea157b86e98263eda9f15909ce49a7.png)


**Méthode de priorisation des hypothèses à tester - indispensable pour continuer le développement de DossierSCO**

Une manière de gérer les priorités est d'établir des matrices de gains potentiels en fonction du coût de mise en place. Ci dessous un exemple de gain potentiel par rapport au coût de tester la pertinence de chaque action :

![](https://pad.etalab.studio/uploads/upload_0c68ab448ff6ed3b39d5e0bf31418aa9.png)


Ci dessous une matrice représentant l'impact estimé sur l'activation et l'ampleur de l'incertitude par rapport à cet impact :

![](https://pad.etalab.studio/uploads/upload_eb5805c1f0cefa44396e8ab10648ea78.svg)

### Segmenter pour mieux déployer

#### Se concentrer sur les early adopters pour être efficaces pendant la phase d'expérimentation
L'épreuve du terrain a enseigné à l'équipe les critères selon lesquels un établissements est (ou non) un utilisateur potentiel durant la phase d'expérimentation. Ces premiers utilisateurs s'appelent *early-adopters* et se focaliser sur eux dans un premier temps permet :
- de maximiser le retour sur investissements (efforts et moyens), en ne perdant pas de temps avec ceux qui coûteront très cher à convaincre
- d'itérer sur le produit avec des utilisateurs plus motivés
- de créer des ambassadeurs qui nous permettront de convaincre les segments-cible suivants

![](https://pad.etalab.studio/uploads/upload_039575073cebc8161285362b6ffbc377.png)


**Profil des établissements innovateurs & early-adopters sur lesquels se focaliser pendant la prochaine phase d'expérimentation:**
1. Établissements ouverts au numérique (critère premier)
2. Effectif suffisant face à leur charge de travail courante
3. Personnels stables dans le temps


#### Premiers apprentissages sur la segmentation des établissements pour les itérations ultérieures

L'heure est à se concentrer sur un segment restreint et bien identifié : les early-adopters. Cependant nous avons pu identifier des critères de segmentations qui nous feront gagner du temps pour le développement ultérieur de DossierSCO, en nous permettant d'orienter les développements sur le produit. Les critères suivants appelent chacun des jeux de fonctionnalités différentes, il sera nécessaire de les prioriser pour le développement-produit + déploiement (qui doivent avancer ensemble) : 
- par la distance que les élèves ont à parcourir pour rejoindre leur collège
- par nombre d'élèves
- par spécificité du terrain (plan d'évacuation lié aux risques naturels : innondation, éboulement)
- par degré d'intégration avec l'environnement local (exemple : horaires aménagés pour faire de la musique ailleurs)
- par le niveau de service fourni par l'établissement (casier, internat)

C'est le déploiement sur une grande diversité de zones géographiques en deuxième saison qui a permis de dégager ces premiers éléments de segmentation des établissements.


Tous les collèges ne sont pas égaux et un collège peut appartenir à plusieurs segments. Il en existe d'ailleurs sans doute d'autres à découvrir. Dans une troisième saison, nous serions attentifs à faire émerger d'autres segments.

Pour comprendre au mieux chaque segment, une approche envisagée en troisième saison serait de rencontrer des groupes d'établissements par segment.

Pour répondre à la diversité des établissments, une piste à long terme serait de rendre DossierSCO beaucoup plus modulaire pour que chaque établissement sélectionne les éléments qui lui correspondent le mieux.



## Valeur perçue du service

### Pour les parents
- Pas de déplacement
- Pas de paperasse
- Réassurance quant à la complétude de l'inscription de leur enfant


### Pour les établissements 

- Inscription autonome à DossierSCO
- Récupération des convocations et des fiches infirmerie par classe
- Information sur le nombre d'élèves par option
- Paramétrage de la carte des formations
- Paramétrage des options pédagogiques par mef
- Paramétrage des régimes d'autorisation de sortie 


## Points d'attention en cas de généralisation

### Comment assurer la qualité du service à l'échelle

L'hébergement est réalisé sur des solutions de cloud. Un très grand nombre de noeuds (machines) peut être ajouté en quelques minutes en fonction du trafic. Ce nombre est réduit aussi rapidement lorsque la période de fort trafic est passée.

### Comment assurer le support

En saison 2, nous utilisons le service [Drift](https://www.drift.com/), suivi par l'équipe, et les emails.

La DSI de l'académie de Versailles nous a proposé de travailler ensemble pour mettre en place un protocole de support et un robot conversationnel pour faciliter le support.

Nous avons parlé d'utiliser le forum des gestionnaires, pour partager des questions mais surtout des protocoles et de la documentation.

### Urbanisation et articulation avec le reste des applications

- Articulation avec SIECLE
- Articulation avec Educonnect 
- Articulation avec le bouquet de téléservices
- Intégration de la charte graphique recommandée par le MEN

# Apprentissage en terme de méthode dans le cadre du dossier FTAP 

La confrontation régulière de l'équipe à la réalité de ses utilisateurs permer d'adapter les choix de conception aux attentes des utilisateurs. Une conception au plus près des besoins de ces utilisateurs favorise l'adoption du service.

Des pratiques ont permis d'associer les utilisateurs à la démarche.

## Familles

### Tests utilisateurs

Des tests utilisateurs réalisés très tôt lors du développement de la preuve du concept permettent de prendre connaissance des points les plus importants. Dans le cas de DossierSCO :
- l'accès au service
- les pièces jointes
_Si je n'ai pas honte la première fois que je montre mon application, c'est que je la montre trop tard._

Deux moments qui ont bien fonctionné pour que des parents acceptent de nous répondre :
- se poser à l'entrée de l'établissement lors d'un évènement comme une journée d'accueil trimestrielle des parents à l'occasion des conseils de classe.
- réaliser un test utilisateur au téléphone en contactant des parents qui ont rencontré des difficultés à se connecter.

### Entretiens utilisateurs

Une question simple posée à la fin de ces tests utilisateurs permet d'identifier plus précisément la valeur du service : si vous aviez le choix l'année prochaine entre utiliser DossierSCO et revenir au papier, quel serait votre choix et de demander pourquoi ? Dans le cas de DossierSCO les parents préfèrent continuer à l'utiliser dans 87% des cas pour deux raisons :
- ne pas se déplacer
- éviter le stress de l'enfant-messager : combien de temps le papier d'inscription va rester dans le cartable de l'élève ? A quel point sera-t'il chiffoné quand il sera finalement remis ?

### Les commentaires comme boucles de feedback

Scruter les commentaires négatifs déposés par les familles permet de les rappeler au téléphone ou de les contacter par mail pour expliciter des problèmes de production ou d'utilisabilité.

## Etablissements

### Openlab

Une stratégie qui a bien fonctionné pour organiser un openlab national, c'est de le faire au lab 110 bis.
Le buffet et les billets de train ont été pris en charge par l'attributaire du marché (Scopyleft).
La forme s'approchait de celle d'un forum ouvert.

#### Les apprentissages (points les plus positifs)

Des exemples d'éléments positifs que nous avons observés dans un openlab :

- des personnes frileuses découvrent la culture collaborative de l'équipe et sont rassurées.
- des utilisateurs partagent leur expérience, ce qui rassure les personnes qui ne sont pas encore utilisatrices.
- des échanges bidirectionnels ont lieu entre utilisateurs et développeurs.


#### Des points positifs à préserver

- L'absence de code vestimentaire facilite les échanges entre différents niveaux de hiérarchie. 
- Des courtes séquences de lancement de type "brise-glace" donnent confiance aux participants et permettent de mettre le groupe en mouvement.
- Former des cohortes ou des tribus à interroger (customer segments) pour évaluer un micro-feedback sur des questions qu'on pourrait se poser pendant le développement ou l'affinage du backlog (4-5 appels téléphoniques) : des cohortes de secrétaires, d'intendants, de proviseurs, de parents d'élève.

#### Des métriques à tester lors d'un openlab

- Question à poser pendant l'évènement et après : avez-vous perdu votre journée ?
- Question à poser aux ambassadeurs : combien avez-vous contacté de personnes ? Combien vous ont répondu ?
- Poser la question pendant l'openlab : voulez-vous devenir ambassadeur ?
- Question à poser après : avez-vous fait un retour d'expérience auprès d'autres collèges ? Avez-vous parrainé un autre établissement ?
- Question à poser pendant l'évènement Cohorte : une métrique pendant l'évènement : êtes-vous OK pour vous inscrire sur un slack pour vous contacter quand on se pose des questions ? Autres métriques (post) sur les réponses obtenus.

#### Après l'openlab

Des personnes ont créé des comptes et commencé à jouer avec l'application et formulé des demandes.

## Recruter un ambassadeur

- Sélectionner un établissement qui a montré son intérêt pour le produit par des relances.
- Si l'établissement est en province, être attentif à avoir une posture basse et à éviter des clichés associés à un pouvoir centralisé.
- Réaliser des entretiens téléphoniques avec les 3 têtes de l'établissement : proviseur, secrétaire et intendant (exemple pour un collège).
- Sélectionner la personne qui sera la plus motrice : la rencontrer en premier lors de la visite sur site.
- Lors de l'entretien avec la direction, se placer tout d'abord en posture d'écoute.


## Apprentissages techniques

DossierSCO est plutôt un outil pour enregistrer des changements d'état plutôt qu'un outil qui stocke des états. Une piste pour mieux épouser cette constatation serait d'adopter une approche de type event sourcing.

# Analyse du taux de conversion : facteurs ayant contribué à l'écart entre 105 inscrits et 24 utilisateurs 

Différents retours, quantitatifs et qualitatifs, de la part des établissements nous permettent d'emettre des hypothèses pour comprendre l'origine du taux de conversion de 25%.

Afin de comprendre l'origine du taux de perdition des établissements inscrits qui n'ont pas utilisés DossierSCO pour préparer leur rentrée, nous avons analysé des retours reçus en cours de campagne et contacté un échantillon d'établissements inscrits.

Certaines hypothèses sont génériques et d'autres propres à des étapes du tunnel de conversion. 

## Facteurs qui ont joué sur plusieurs phases

Nous avons noté des facteurs qui ont joué lors de plusieurs phases :
- des freins dans des académies pilotes, inconfortables avec le principe d'une expérimentation ciblant un sous-ensemble d'établissements sur un territoire donné ("tout ou rien"). Cela a notamment été le cas de l'Académie de Versailles, qui de fait n'a pas participé à l'expérimentation. Cet élément a également pesé sur l'acquisition.

- que les établissements expérimentateurs d'autres chantiers de dématérialisation par le ministère étaient réticents à tester une nouvelle application (notamment le déploiement du téléservice national de demande de bourse). Un meilleur ciblage des établissements pilotes, en adéquation avec les autres chantiers du ministère, pourraient contibuer à améliorer le taux de conversion. Cet élément a également pesé sur l'acquisition.
  
- une réelle attente dans certaines établissements en terme d'accompagnement pour prendre en main une nouvelle procédure numérique, aussi simple soit-elle. Cette observation est corroborée par les retours des académies qui mettent en oeuvre les dispositifs de support utilisateurs adressés aux établissements sur les autres projets du ministère.

- une diversité des pratiques d'un établissement à l'autre dans la gestion des inscriptions et ré-inscription. En effet, les calendriers et les informations demandées peuvent varier et dissuader un établissement d'utiliser un service générique.

- l'aspect expériemental a fait peur à certains établissements.

#### Aquisition : conversion des Contactés en Inscrits

Nous avons par définition moins d'élément de données sur le taux de déperdition des établissements ne nous ayant pas répondu. Il serait pertinent de leur adresser un questionnaire dédié. 


#### Aquisition : conversion des Inscrits en Expérimentateurs
Ce taux de perdition s'explique en partie par le profil de certains chefs d'établissement curieux. 

- Problème de mail d'activation : 
Près de la moitié des établissements n'ont pas reçu le mail d'activation suite à leur inscription sur DossierSCO. En tout 61 établissements inscrits n'ont pas activé leur compte. Pour plus d'une quinzaine d'établissements utilisateurs, les mails d'activation ont dû être renvoyés manuellement par l'équipe.

Le serveur mail n'étant pas hébergé à l'intérieur du réseau de l'Education Nationale, les mails envoyés automatiquement n'ont pas toujours été délivrés.

Une autre contre-mesure potentielle serait de demander à chaque DSI de chaque des 30 accadémies de white-lister l'adresse d'origine. Cette contre-mesure à été utilisée avec succès dans une académie.

- Les établissements attendent plus d'options de personnalisation de la campagne
Au delà des options pédagogiques, des régimes de pension (incomplet), des régimes de sortie, du quotient famillial et des justificatifs dématérialisés, les établissements demandent d'autres options de personnalisation de la campagne d'inscritpion comme la gestion des casiers ou l'organisation d'évacuation de secours. 

L'évolution du produit, menée en parallèle du recrutement des établissements, ne nous a pas permis de répondre à toutes les attentes remontées par les établissements à temps pour les convaincre de tester le produit.

Le collège de Paul LE FLEM 22, nous remonte par exemple que l'impossibilité de sélectionner 2 options parmi l'ensemble proposé est une carence du produit qui ne lui permet pas d'utiliser DossierSCO. 

- Problème d'import de la base Eleve
Une friction d'ergonomie a pu rebuter certains établissement. A l'import, les établissements doivent récupérer un fichier .xls à partir du fichier .zip téléchargé de SIECLE. Cette manoeuvre a pu mettre de côté une partie des utilisateurs peu à l'aise avec la bureautique. 

- Crainte d'une carence de ressources en raison d'un mouvement de personnel
Les établissements ayant des mouvements de personnels avant ou après le lancement de la campagne sont naturellement inquiets quant à leur capacité à utiliser un nouveau produit. 5 établissements intérrogés ont clairement donné cette raison pour justifier de leur retrait de l'expérimentation. 

- Les relances suites à l'inscription des établissements ont été faites trop tardivement, compte tenu des délais de préparation de la campagne. 

#### Activation : Conversion des Expérimentateurs en Utilisateurs
- Incertitude quant aux retours des données dans SIECLE
Les établissements inscrits n'ont pas pu expérimenter le retour des données dans SIECLE avant le début des inscriptions. Ils étaient donc incapables d'anticiper la charge de gestion réelle associée à l'utilisaton du service. 

[Détails des difficultés rencontrées dans la remontée des données dans SIECLE]

La plateforme de test de SIECLE (située à Clermont-Ferrand) n'a été disponible que tard au mois d'avril. Au moment de nos premiers tests de remontée vers SIECLE, la plateforme a à nouveau été indisponible pendant trois semaines. La remontée vers SIECLE nécessite de vérifier la correspondance de chaque donnée textuelle avec des codes spécifiques. Il a par exemple été nécessaire de faire de nombreux tests avant de trouver quel champs pouvait être utilisé pour que l'import privé reconnaisse un élève par son INE
