# Le canevas de l'analyse de risque

![](assets/canevas.png)

\(1\) **Les *user stories* et leurs besoins de sécurité**

Pour cette rubrique, il s’agit de recenser les principaux éléments de valeur d’usage mis en œuvre par le produit, et d’estimer leurs besoins de sécurité (DICP : disponibilité, intégrité, confidentialité, preuve). Ces éléments seront généralement exprimés sous forme de user stories.

L’objectif est d’identifier, pour chaque user story, quels sont les besoins de sécurité les plus importants afin d’orienter par la suite le travail d’identification des scénarios de risques pertinents. Le degré d’importance peut être pondéré par un indice simple. Par exemple, **• pour un besoin important et • • pour un besoin notable**. Un schéma similaire pourra être adopté pour les autres éléments de l’analyse. L’évaluation de l’importance d’un besoin de sécurité est souvent itérative et obtenue par comparaison au fur et à mesure de l’atelier ; un besoin identifié comme « important » traduit le fait qu’il est essentiel pour le produit.

Le point de départ de l’atelier – les user stories – est essentiel. En commençant par-là, l’équipe ancre dans le reste de l’atelier l’idée que les mesures de sécurité servent la valeur livrée aux usagers. En effet, pour chaque besoin de sécurité important relatif à une *user story*, il y a un ou plusieurs événements redoutés et au moins un scénario de risque susceptible de compromettre la proposition de valeur.

> Exemple
> 
> Un client peut émettre une demande \(héler virtuellement un taxi\), un client peut évaluer une course effectuée ou déclarer un incident.

\(2\) **Les sources de risques et leurs intentions**

Il s’agit de recenser les sources de risques – accidentelles ou intentionnelles, externes ou internes – susceptibles d’impacter la valeur d'usage : qui ou quoi pourrait porter atteinte aux besoins de sécurité. Le schéma ci-dessous résume quelques-unes des motivations à l’origine d‘attaques intentionnelles, et peut constituer un point de départ intéressant à la discussion lors de l’atelier.

![](assets/sources.png)

Il est recommandé de recenser les sources de risques de natures et de motivations variées pour disposer d’un échantillon de risques représentatif à partir duquel bâtir des scénarii dont les menaces et modes opératoires diffèrent.

> Exemple
>
> Opérateur concurrent cherchant à discréditer, voire saboter le service Le.Taxi \(malveillance\), mafia cherchant à collecter des données à caractère personnel pour les monnayer \(appât du gain\), etc.

\(3\) **Les sources de risques et leurs intentions**

Un événement redouté \(ER\) correspond au non-respect d’un besoin de sécurité d'une *user story* : chaque besoin de sécurité associé à une _user story_ de l'étape \(1\) se décline donc sous la forme d’un ou plusieurs événements redoutés. On précisera bien le ou les impacts \(sur les missions ou la sécurité des personnes, financiers, juridiques, d'image, environnementaux, collatéraux, etc.\) ainsi que le niveau de gravité estimé.

L’objectif étant d’identifier en priorité les événements redoutés dont les conséquences seraient difficilement surmontables. En première approche, l'échelle de cotation peut se limiter à un indice de priorité, par exemple : P1 – ER à retenir, P2 – ER à considérer dans un second temps. De façon plus élaborée, une échelle de cotation à 3 niveaux ou plus pourra être adoptée : **• gravité faible, •• moyenne, ••• élevée**.

Un événement redouté est exprimé sous la forme d’une expression courte qui permet de comprendre facilement le préjudice lié à la *user story* concernée. Il est recommandé de mentionner dans l’intitulé de l’ER la source de risque la plus vraisemblable susceptible d’en être à l’origine. Enfin, dans un souci d’efficacité, l’équipe s’intéresse en première approche aux événe- ments redoutés associés aux besoins de sécurité « importants ».

> Exemple
>
>_Un opérateur concurrent, se faisant passer pour un client, hèle un taxi qui réalise une course d’approche en pure perte._

\(4\) **Les composants vulnérables**

Il s’agit d’identifier parmi les composants du produit ceux contribuant à la réalisation des _user stories_ identifiées dans l’étape \(1\) et susceptibles d’être concernés ou ciblés par les sources de risques de l’étape \(2\). Il est recommandé de préciser, pour chaque composant, quelles sont les vulnérabilités que ces sources de risque pourraient exploiter.

> Exemple
>
> Base de données Le.Taxi \(accès en lecture/écriture depuis Internet, modification fréquente\).

L’identification des composants peut être structurée comme suit :

* **Infrastructures physiques :** bâtiments, locaux, espaces physiques permettant l'activité et les échanges de flux 
* **Organisations :** structures organisationnelles, processus métiers et supports, ressources humaines
* **Systèmes numériques matériels et logiciels :** systèmes informatiques et de téléphonie, réseaux de communication.

Le degré de granularité dans la description des composants sera adapté au niveau de connaissance du produit lors de l’atelier. Enfin, les composants prioritaires à recenser sont ceux qui contribuent \(de façon directe ou indirecte\) aux _user stories_ ayant des besoins de sécurité « importants ».

Afin d’étendre le périmètre de l’appréciation des risques, vous pouvez compléter cette étape en identifiant quelles parties prenantes de l’écosystème seraient susceptibles d’être exploitées pour faciliter une attaque sur un composant du produit (reportez-vous à la fiche mémo précédente). Les parties prenantes critiques à considérer en priorité sont celles qui ont un lien avec un les composants recensés.

> Exemple
>
> Prestataire informatique assurant la télémaintenance du serveur qui héberge la base de données Le.Taxi.

\(5\) **Les scénarii de risques \(*abuser stories*\) et les mesures de traitement**

La finalité de l’atelier est d’identifier les risques numériques de référence à prendre en compte pour bâtir ou compléter la politique de sécurité du produit.

L’équipe commence par dresser une liste de **scénarios de risques** – abuser stories – en confrontant les sources de risques \(2\), les événements redoutés \(3\) et les composants vulnérables \(4\). Concrètement, il s’agit de voir de quelle façon chaque source de risque retenue peut impacter des composants du produit, par exploitation notamment de leurs vulnérabilités ou d’un facteur externe aggravant, pour générer un événement redouté. Chaque *abuser story* peut ensuite être classiquement évalué en terme de vraisemblance, puis de criticité à partir de la gravité de l'événement redouté associé.

> Exemple
>
> Un attaquant externe accède aux informations à caractère personnel des clients en usurpant l'identité du serveur Le.Taxi ou en exploitant une vulnérabilité non corrigée.
> Un client de mauvaise foi attribue abusivement une mauvaise note au taxi.

Pour chaque abuser story répertoriée, l’équipe peut définir si besoin **l’option de traitement du risque** la plus appropriée (éviter, réduire, transférer, accepter). Dans le cas où le risque doit être réduit, les participants identifient les **mesures de sécurité** complémentaires qu’il faudra mettre en œuvre, en plus des mesures existantes ou déjà prévues. Leur réalisation est consignée par l’équipe au même titre que les autres *user stories*.

Enfin, l'équipe peut clore l'atelier en identifiant les **risques résiduels**. Ces derniers concernent :

  * les _abuser stories_ non traitées \(acceptées en l'état\) ou seulement partiellement \(mesures de sécurité mises en place, mais ne réduisant pas complètement ou suffisamment le risque\).

  * les _abuser stories_ faisant l'objet d'un transfert du risque, lequel ne couvre généralement pas l'ensemble des impacts \(exemple : l'assurance ne couvre pas l'atteinte à l'image\).

  * pour affiner dans un deuxième temps : les besoins de sécurité de l'étape \(1\) et les événements redoutés de l'étape \(3\) non déclinés en abuser stories.

Un certain travail \(souvent subjectif\) de consolidation des risques résiduels est à effectuer par l'équipe afin de disposer d'un bilan à jour et reflétant l'état de maîtrise du risque numérique du produit. Les risques résiduels les plus significatifs seront en priorité recensés et mis en évidence. Par exemple, l'usage d'échelles de cotation en gravité, vraisemblance et criticité, associé à des seuils d'acception du risque, constituera une aide précieuse pour hiérarchiser les risques résiduels avec objectivité et cohérence. Notons enfin que ce bilan, enrichi au fil des ateliers d'analyse de risque, sera complété des éventuelles vulnérabilités résiduelles identifées à l'issue des audits de sécurité.

La section suivante présente l'intégralité de l'analyse des risques pour la plateforme Le.Taxi et vous permettra d'observer l'articulation des différents éléments présentés ici sur un cas pratique.
