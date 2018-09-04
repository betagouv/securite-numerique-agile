# Se préparer à une démarche d'homologation

**L'homologation de sécurité est un acte formel par lequel l'autorité responsable d'un système engage sa responsabilité en matière de gestion du risque.** Elle est rendue obligatoire, pour les administrations[^1], par le [**décret n° 2010-112 du 2 février 2010**](https://www.legifrance.gouv.fr/affichTexte.do?cidTexte=JORFTEXT000021779444&categorieLien=id), selon des modalités précisées par le [**Référentiel Général de Sécurité (RGS)**](https://www.ssi.gouv.fr/administration/reglementation/confiance-numerique/le-referentiel-general-de-securite-rgs/liste-des-documents-constitutifs-du-rgs-v-2-0/). De même, elle est obligatoire pour tout produit traitant d'information relevant du secret de la défense nationale, comme précisé dans l'Instruction Générale Interministérielle 1300 \(IGI 1300\). Citons également la [*Loi de Programmation Militaire*](https://www.ssi.gouv.fr/entreprise/protection-des-oiv/protection-des-oiv-en-france/), dont le volet cyber \([**loi n° 2013-1168 du 18 décembre 2013**](https://www.legifrance.gouv.fr/eli/loi/2013/12/18/2013-1168/jo/article_22)\) Article impose aux opérateurs d'importance vitale le renforcement de la sécurité des systèmes d’information critiques qu’ils exploitent, mené dans le cadre d'une démarche d'homologation.

Lorsqu'elle n'est pas réglementairement imposée, **la démarche d'homologation reste toutefois une excellente façon de témoigner, vis-à-vis des usagers, de la volonté de prendre en compte la sécurité numérique des services proposés, et de valoriser le niveau de maîtrise des risques atteint[^1]**.

Comme le rappelle le guide relatif à [« _L'homologation de sécurité, en 9 étapes simples_ »](https://www.ssi.gouv.fr/actualite/lhomologation-en-9-etapes-simples-nouvelle-publication-de-lanssi/) :

> L'objectif de la démarche d'homologation \[...\] est de trouver un équilibre entre le risque acceptable et les coûts de sécurisation, puis de faire arbitrer cet équilibre, de manière formelle, par un responsable qui a autorité pour le faire.

Les livrables de l'atelier d'analyse des risques, tel que nous l'avons présenté dans ces pages, constituent un entrant nécessaire mais non suffisant à une démarche d'homologation. Par conséquent, nous recommandons de dédier un atelier à la préparation de la commission d'homologation (formalisation du dossier de sécurité, bilan des tests et audits de sécurité, consolidation des risques résiduels, suivi des mesures de sécurité et du plan d'action correctif).

### Homologation provisoire

Par hypothèse, l'équipe à laquelle s'adresse ce guide cherche à mettre rapidement en service une première version incomplète du produit, puis à l'étoffer par incréments fonctionnels.

Dans ce contexte, l'équipe se dirigera donc naturellement vers une **décision d'homologation provisoire, afin d'adapter le niveau de risque résiduel accepté à un contexte donné**. Sa validité sera limitée dans le temps et conditionnée par des critères liés au volume ou à l'intensité d'exploitation, dans une unité appropriée : en nombre d'usagers, en volume de transactions, etc.

Ces **critères de validité** doivent pouvoir être mesurés et surveillés afin d'objectiver que l'on respecte encore les conditions de validité de l'homologation provisoire. L'équipe pourra moduler la durée et les critères de validité des homologations provisoires successives en fonction de la diffusion réellement constatée du service.

Une stratégie d'homologation pour la plateforme Le.Taxi pourrait ainsi se décliner en trois jalons :

* un jalon « autorisation de tests » d'une durée de 1 à 3 mois, menée exclusivement auprès d'usagers volontaires sur consentement explicite ;
* un jalon « autorisation provisoire d'exploitation », d'une durée maximale de 12 mois et un plafond de 1 000 courses cumulées ;
* un jalon « mise en service ferme » tel que décrit ci-après.

### Homologation ferme

Une décision d'homologation ferme pourra être prononcée dès lors qu'un produit ou un service aura atteint son « régime de croisière ». Elle est généralement assortie d'une période de validité plus longue \(3 ans étant une valeur typique\) et vise le contexte d'exploitation normalement prévu, sans restrictions particulières d'usage.

Si l'équipe n'a pas eu recours aux services d'un expert en sécurité numérique lors des ateliers d'analyse de risque, ni à l'intervention d'un auditeur externe pour réaliser par exemple des tests d'intrusion ou une revue de code axée sur les besoins de sécurité, ces vérifications extérieures s'imposent comme préalables à une décision ferme.

La mise en place d'un **plan d'amélioration continue de la sécurité** pour les versions successives à venir du produit ou service est également un élément important de la décision d'homologation. Ce plan garantit la montée en puissance et en maturité de la sécurité du produit, et permet une gestion priorisée des **risques résiduels** selon leur criticité.

Notez enfin qu'on prend soin de ne pas parler d'homologation « définitive » — le caractère évolutif d'un produit avec une forte composante logicielle impose de réévaluer périodiquement les risques, quand bien même le produit serait resté inchangé — ce qui n'arrive en pratique que rarement…

### Formaliser le dossier d'homologation

Nous ne détaillerons pas ici les étapes de la constitution du dossier ou de la commission d'homologation. Le guide [_L'homologation de sécurité, en 9 étapes simples_](https://www.ssi.gouv.fr/actualite/lhomologation-en-9-etapes-simples-nouvelle-publication-de-lanssi/) prend ici notre relais : simple, pratique et concis, nous pouvons témoigner sur la base de l'expérience réelle, qui nous a souvent servi dans ces pages, qu'il sera un compagnon précieux pour toutes les équipes Agiles qui souhaitent aboutir à une décision d'homologation.

[^1]: La méthode présentée peut également servir de point de départ à une démarche de certification ou de qualification de solutions de sécurité.
