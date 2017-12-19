# Le canevas de l'analyse des risques

L'articulation entre les éléments de l'analyse des risques est résumée par le schéma suivant :

![](assets/canevas.png)

\(1\) Les user stories et leurs besoins de sécurité

Pour cette rubrique, il s’agit de recenser les principaux éléments de valeur d'usage mis en œuvre par le produit, et à estimer leurs besoins de sécurité \(DICP : disponibilité, intégrité, confidentialité, preuve\). Ces éléments seront généralement exprimés sous la forme de user stories.

L’objectif est d’identifier pour chaque user story quels besoins sont importants, afin d’orienter par la suite le travail d’identification des scénarios de risques pertinents. Le degré d’importance peut être pondéré par un indice simple, par exemple : **• besoin important, •• besoin notable**. \(En cas de divergences parmi les participants, on peut procéder à un exercice de type « [dot vote](https://en.wikipedia.org/wiki/Dot-voting) ».\) Un schéma similaire pourra être adopté pour les autres éléments de l'analyse.

Le point de départ de l’atelier – les user stories – est important. En commençant par là, l’équipe ancre le reste de l’atelier dans l’idée que les mesures de sécurité servent à assurer la valeur livrée aux usagers. En effet, pour chaque besoin de sécurité important d’une valeur métier, il y a un événement redouté et au moins un scénario de risque susceptible de compromettre la proposition de valeur.

\(2\) Les sources de risques

Il s’agit de recenser les sources de risques – accidentelles ou intentionnelles, externes ou internes – susceptibles d’impacter la valeur métier : qui ou quoi pourrait porter atteinte aux besoins de sécurité. Le schéma ci-dessous résume visuellement ce qui peut motiver des attaques intentionnelles, et peut fournir un bon point de départ à la discussion lors de l’atelier.

![](assets/sources.png)

\(3\) Les événements redoutés et leur gravité

Un événement redouté correspond au non-respect d’un besoin de sécurité : chaque besoin de sécurité associé à chaque user story est donc décliné sous la forme d’un ou plusieurs événements redoutés. On précisera bien le ou les impacts \(sur les missions, sur la sécurité des personnes, financiers, juridiques, sur l'image, sur l'environnement, sur les tiers, etc.\) ainsi que le niveau de gravité estimé.

Afin de faire le lien à ce stade avec les sources de risques identifiées dans l’étape \(2\), il peut être pertinent de mentionner les sources de risques les plus plausibles susceptibles d’en être à l’origine. Enfin, dans un souci d’efficacité, l’équipe s’intéresse en première approche aux événements redoutés associés aux besoins de sécurité « importants ».

\(4\) Les composants vulnérables

Il s’agit d’identifier les composants du produit qui contribuent à la réalisation des user stories identifiées dans l’étape \(1\), et susceptibles d’être concernés ou ciblés par les sources de risques de l’étape \(2\).

L’identification des composants peut être structurée comme suit :

* Physique : locaux, infrastructures, espaces physiques de communication
* Organisations : structures organisationnelles, processus, ressources humaines
* Systèmes numériques matériels et logiciels : systèmes informatiques et de téléphonie, réseaux supports de \(télé\)-communication.

\(5\) Les scénarios de risques \(abuser stories\) et les mesures de traitement

La finalité de l’atelier est d’identifier les risques numériques dimensionnants à prendre en compte pour bâtir ou compléter la politique de sécurité du système.

* Dans l’étape \(5\), l’équipe commence par dresser une liste de scénarios de risques – les abuser stories – en confrontant les sources de risques \(2\), les événements redoutés \(3\) et les composants vulnérables \(4\). Concrètement, il s’agit de voir de quelle façon chaque source de risque retenue peut impacter des composants du produit, par exploitation notamment de leurs vulnérabilités ou d’un facteur externe aggravant, pour générer un événement redouté.

* Puis, pour chaque abuser story répertorié, l’équipe définit l’**option de traitement du risque** la plus appropriée \(éviter, réduire, transférer, accepter\). Dans le cas où le risque doit être réduit, les participants définissent les mesures de sécurité complémentaires qu'il faudra mettre en œuvre, en plus des mesures existantes ou déjà prévues. Leur réalisation est priorisée par l’équipe au même titre que les autres user stories.

La section suivante présente l'intégralité de l'analyse des risques pour la plateforme Le.Taxi et vous permettra d'observer l'articulation des différents éléments présentés ici sur un cas pratique.

