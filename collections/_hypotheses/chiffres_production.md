---
title: Chiffres production
---
```
irb(main):006:0> DossierEleve.all.count
D, [2019-07-15T06:07:53.938757 #21] DEBUG -- :    (13.9ms)  SELECT COUNT(*) FROM "dossier_eleves" INNER JOIN "eleves" ON "eleves"."id" = "dossier_eleves"."eleve_id"
=> 17914
irb(main):007:0> DossierEleve.where("etat != 'pas connecté'").count
D, [2019-07-15T06:08:04.615342 #21] DEBUG -- :    (11.6ms)  SELECT COUNT(*) FROM "dossier_eleves" INNER JOIN "eleves" ON "eleves"."id" = "dossier_eleves"."eleve_id" WHERE (etat != 'pas connecté')
=> 7787


10 000 familles non connectées ?

=> Sans doute plusieurs établissement qui ont fait des chargements de base élève pour faire des tests. On y retrouve nos tests à nous (Poquelin pour l'ENT, Arago pour Siecle, ???)


rb(main):031:0> DossierEleve.select(:satisfaction).where("etat != 'pas connecté'").group('satisfaction').count
D, [2019-07-15T06:13:52.868568 #21] DEBUG -- :    (11.8ms)  SELECT COUNT("dossier_eleves"."satisfaction") AS count_satisfaction, "dossier_eleves"."satisfaction" AS dossier_eleves_satisfaction FROM "dossier_eleves" INNER JOIN "eleves" ON "eleves"."id" = "dossier_eleves"."eleve_id" WHERE (etat != 'pas connecté') GROUP BY "dossier_eleves"."satisfaction"
=> {0=>1538, 1=>154, 3=>795, 5=>2949, 2=>220, 4=>2131}

Soit, pour 7 787 familles connectées,

0: 1 538 / 7 787 ~= 20% de non exprimées

1: 154 / 7 787 ~= 2%
2: 220 / 7 787 ~= 3%
3: 795 / 7 787 ~= 10%
4: 2 131 / 7 787 ~= 27%
5: 2 949 / 7 787 ~= 38%

En prenant uniquement les familles qui se sont exprimées

1: 154 / 7 787 ~= 3%
2: 220 / 7 787 ~= 4%
3: 795 / 7 787 ~= 12%
4: 2 131 / 7 787 ~= 34%
5: 2 949 / 7 787 ~= 47%

irb(main):036:0> DossierEleve.select(:satisfaction).where("etat != 'pas connecté'").where(continuer_dossiersco: true).count
D, [2019-07-15T06:17:19.217575 #21] DEBUG -- :    (11.6ms)  SELECT COUNT("dossier_eleves"."satisfaction") FROM "dossier_eleves" INNER JOIN "eleves" ON "eleves"."id" = "dossier_eleves"."eleve_id" WHERE (etat != 'pas connecté') AND "dossier_eleves"."continuer_dossiersco" = $1  [["continuer_dossiersco", true]]
=> 4931

4 931 souhaitent continuer dossiersco (nous avons mis en place cette mesure tardivement). Soit 63%
```

