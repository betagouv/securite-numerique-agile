# Se préparer à une démarche d'homologation

L'homologation de sécurité est un acte formel par lequel l'autorité responsable d'un système engage sa responsabilité en matière de gestion du risque. Elle est rendue obligatoire, pour les administrations, par le [décret n° 2010-112 du 2 février 2010](https://www.legifrance.gouv.fr/affichTexte.do?cidTexte=JORFTEXT000021779444&categorieLien=id), selon des modalités précisées par le [Référentiel Général de Sécurité](https://www.ssi.gouv.fr/administration/reglementation/confiance-numerique/le-referentiel-general-de-securite-rgs/liste-des-documents-constitutifs-du-rgs-v-2-0/).

Pour les entreprises privées, l'homologation n'est pas obligatoire mais n'en reste pas moins une excellente façon de témoigner, vis-à-vis des usagers, de la volonté de prendre en compte la sécurité numérique des services qu'elles proposent, et d'expliciter le niveau de maîtrise des risques qu'elles revendiquent.

Comme le rappelle le guide [_L'homologation de sécurité, en 9 étapes simples_](https://www.ssi.gouv.fr/actualite/lhomologation-en-9-etapes-simples-nouvelle-publication-de-lanssi/) :

> L'objectif de la démarche d'homologation \[...\] est de trouver un équilibre entre le risque acceptable et les coûts de sécurisation, puis de faire arbitrer cet équilibre, de manière formelle, par un responsable qui a autorité pour le faire.

Les livrables de l'atelier d'analyse des risques, tel que nous l'avons présenté dans ces pages, constituent un entrant nécessaire mais non suffisant à une démarche d'homologation.

Par conséquent, en vue de la préparation de l'homologation, l'équipe peut décider de donner la priorité à la réalisation et au suivi des mesures de sécurité pendant une itération.

### Décision provisoire

Par hypothèse, l'équipe à laquelle ce guide s'adresse cherche à mettre rapidement une première version incomplète du produit ou du service, puis à l'étoffer progressivement par incréments fonctionnels.

Dans ce contexte, l'équipe visera donc naturellement une **décision d'homologation provisoire**, afin d'adapter le niveau de risque résiduel accepté à un contexte donné. Sa validité sera limitée dans le temps, et conditionnée par des critères liés au volume d'exploitation, dans une unité appropriée : en nombre d'usagers, en volume de flux, etc.

L'équipe pourra moduler la durée et les critères de validité des homologations provisoires en fonction de la diffusion réellement constatée du service.

Ainsi une stratégie d'homologation pour la plateforme Le.Taxi pourrait se décliner en trois jalons :

* Un jalon « autorisation de tests » \(ADT\) pour une durée de 1 à 3 mois, menée exclusivement avec des usagers volontaires et donnant un consentement explicite
* Un jalon « autorisation provisoire d'exploitation », pour une durée maximale de 12 mois, et un plafond de 1000 courses
* Un jalon « mise en service ferme » tel que décrit ci-dessous

### Décision ferme

Une décision d'homologation ferme pourra être prononcée dès lors qu'un produit ou un service aura atteint son « régime de croisière ». Elle est généralement assortie d'une période de validité plus longue \(3 ans étant une valeur typique\) et vise le contexte d'exploitation normalement prévu, sans restrictions particulières d'usage.

Si l'équipe n'a pas eu recours aux services d'un·e expert·e SSI pendant les ateliers d'analyse des risques, ni à l'intervention d'un auditeur externe pour réaliser par exemple des tests d'intrusion ou une revue de code axée sur les besoins de sécurité, ces vérifications extérieures s'imposent comme préalables à une décision ferme.

Notez enfin qu'on prend soin de ne pas parler d'homologation « définitive » — le caractère évolutif du logiciel impose de réévaluer périodiquement les risques, quand bien même le logiciel serait resté inchangé — ce qui n'arrive en pratique que rarement…

### Rendre publique la décision d'homologation ?

Nous invitons les autorités responsables à rendre publiques, et facilement accessibles sur Internet, leurs décisions d'homologation.

La plateforme Le.Taxi, qui nous a fourni de la matière pour illustrer ce guide, en est à nouveau un exemple. Nous avons choisi de publier [sous forme brute le dossier d'homologation](https://github.com/sgmap/beta.ssi/blob/master/homologations/le_taxi.md) correspondant.

Cette invitation pose cependant une question sensible : dans la mesure où une décision d'homologation s'appuie sur le recensement des mesures de sécurité qui ont permis de déplacer, réduire ou supprimer un scénario de risque, _mais également_ de l'analyse des risques résiduels, c'est-à-dire des vulnérabilités qui peuvent encore exister, est-il dangereux de rendre publique cette analyse ? Pour dire les choses brutalement, n'est-ce pas une invitation aux _hackers_ et autres malveillants que de signaler quelles portes dérobées ils pourraient le plus facilement emprunter ?

Nous pensons que les codes sources ouverts, et au-delà le principe même du logiciel libre, vont dans le sens d'un meilleur service rendu aux usagers. Il est indéniable qu'ils contribuent substantiellement à toute l'économie numérique. Ils semblent par ailleurs être, pour l'administration publique en général, et plus précisément dans le cas français, une orientation stratégique se traduisant progressivement dans la loi. Nous croyons de moins en moins à « \[la sécurité par l'obscurité\]\([https://fr.wikipedia.org/wiki/Sécurité\_par\_l'obscurité](https://fr.wikipedia.org/wiki/Sécurité_par_l'obscurité)\) ».

Pour autant, il nous semble raisonnable que certaines portions du dossier d'homologation puissent ne pas être systématiquement communiquées, en particulier la section de l'analyse des risques traitant précisément des risques résiduels.

Après délibération, nous avons cependant choisi de publier également l'intégralité de l['analyse des risques](https://github.com/openmaraude/le.taxi/wiki/Analyse-des-risques) pour la plateforme Le.Taxi. Cette décision, prise en conscience d'un contexte particulier, ne saurait tenir lieu de modèle.

### Formaliser le dossier d'homologation

Nous ne détaillerons pas ici les étapes de la constitution du dossier ou de la commission d'homologation. Le guide [_L'homologation de sécurité, en 9 étapes simples_](https://www.ssi.gouv.fr/actualite/lhomologation-en-9-etapes-simples-nouvelle-publication-de-lanssi/) prend ici notre relais : simple, pratique et concis, nous pouvons témoigner sur la base de l'expérience réelle, qui nous a souvent servi dans ces pages, qu'il sera un compagnon précieux pour toutes les équipes Agiles qui souhaitent aboutir à une décision d'homologation.
