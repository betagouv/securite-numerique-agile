# Le canevas de l'analyse des risques

L'articulation entre les éléments de l'analyse des risques est résumée par le schéma suivant :

![](/assets/canevas.png)

\(1\) Les user stories et leurs besoins de sécurité

Pour cette rubrique, il s’agit de recenser les principaux éléments de valeur d'usage mis en œuvre par le produit, et à estimer leurs besoins de sécurité \(DICP : disponibilité, intégrité, confidentialité, preuve\). Ces éléments seront généralement exprimés sous la forme de user stories.

L_’objectif est d’identifier pour chaque user story quels besoins sont importants, afin d’orienter par la suite le travail d’identification des scénarios de risques pertinents. Le degré d’importance peut être pondéré par un indice simple, par exemple : **• besoin important, •• besoin notable**. \(En cas de divergences parmi les participants, on peut procéder à un exercice de type « _[_dot vote_](https://en.wikipedia.org/wiki/Dot-voting)_ ».\) Un schéma similaire pourra être adopté pour les autres éléments de l'analyse._

_Le point de départ de l’atelier – les user stories – est important. En commençant par là, l’équipe ancre le reste de l’atelier dans l’idée que les mesures de sécurité servent à assurer la valeur livrée aux usagers. En effet, pour chaque besoin de sécurité important d’une valeur métier, il y a un événement redouté et au moins un scénario de risque susceptible de compromettre la proposition de valeur._

\(2\) Les sources de risques  
Il s’agit de recenser les sources de risques – accidentelles ou intentionnelles, externes ou internes – susceptibles d’impacter la valeur métier : qui ou quoi pourrait porter atteinte aux besoins de sécurité. Le schéma ci-dessous résume visuellement ce qui peut motiver des attaques intentionnelles, et peut fournir un bon point de départ à la discussion lors de l’atelier.

![](/assets/sources.png)

_Il est recommandé d’associer un indice de pertinence à chaque source de risque, ceci afin d’identifier les sources de risques potentiellement les plus vraisemblables, dangereuses et/ou déterminées qu’il convient de prendre en compte en priorité dans l’analyse de risque. Bien identifier et nommer les sources de risques facilite grandement l’identification des événements redoutés et des abuser stories._

\(3\) Les événements redoutés et leur gravité

Un événement redouté \(ER\) correspond au non-respect d’un besoin de sécurité : chaque besoin de sécurité associé à chaque user story est donc décliné sous la forme d’un ou plusieurs ER. Il convient ensuite d’estimer le niveau de gravité des impacts occasionnés par l’ER: impacts sur les missions, sur la sécurité des personnes, financiers, juridiques, sur l'image, sur l'environnement, sur les tiers, etc. Afin de faire le lien à ce stade avec les sources de risques identifiées dans l’étape \(2\), il peut être pertinent d’exprimer les ER en mentionnant la ou les sources de risques les plus plausibles susceptibles d’en être à l’origine. Enfin, dans un souci d’efficacité, l’équipe s’intéresse en première approche aux événements redoutés associés aux besoins de sécurité « importants ».

Exemple : « Un opérateur concurrent, se faisant passer pour un faux client, hèle un taxi qui fait une course d’approche en pure perte ».

\(4\) Les composants vulnérables  
Il s’agit d’identifier les composants du produit qui contribuent à la réalisation des user stories identifiées dans l’étape \(1\), et susceptibles d’être concernés ou ciblés par les sources de risques de l’étape \(2\). Il est recommandé de préciser pour chaque composant ses vulnérabilités potentielles que des sources de risque seraient susceptibles d’exploiter.

Exemple : « base de donnée accessible depuis Internet ».

_L’identification des composants peut être structurée comme suit :_

* _Physique : locaux, infrastructures, espaces physiques de communication_
* _Organisations : structures organisationnelles, processus, ressources humaines_
* _Systèmes numériques matériels et logiciels : systèmes informatiques et de téléphonie,_
  _réseaux supports de \(télé\)-communication._

_Le degré de granularité dans la description des composants doit être adapté selon le niveau de connaissance du produit lors de l’atelier. Les composants prioritaires à recenser sont ceux qui contribuent \(de façon directe ou indirecte\) aux valeurs métiers essentielles ayant des besoins de sécurité importants._

\(5\) Les scénarios de risques \(abuser stories\) et les mesures de traitement

La finalité de l’atelier est d’identifier les risques numériques dimensionnants à prendre en compte pour bâtir ou compléter la politique de sécurité du système.

* Dans l’étape \(5\), l’équipe commence par dresser une liste de scénarios de risques – les abuser stories – en confrontant les sources de risques \(2\), les événements redoutés \(3\) et les composants vulnérables \(4\). Concrètement, il s’agit de voir de quelle façon chaque source de risque retenue peut impacter des composants du produit, par exploitation notamment de leurs vulnérabilités ou d’un facteur externe aggravant, pour générer un événement redouté. Les risques sont formalisés sous la forme d’abuser stories et leur pertinence évaluée selon les règles de cotation retenues pour le projet.

* Puis, pour chaque abuser story répertorié, l’équipe définit l’option de traitement du risque la plus appropriée \(éviter, réduire, transférer, accepter\). Dans le cas où le risque doit être réduit, le groupe de travail définit les mesures de sécurité complémentaires qu'il faudra mettre en œuvre, en plus des mesures existantes ou déjà prévues. Leur instanciation est priorisée par l’équipe au même titre que les autres user stories.

_L’identification des scénarios de risques, particulièrement ceux qui sont intentionnels, nécessite une certaine expertise en cybersécurité. Ceci est d’autant plus vrai pour les cas d’attaques sophistiquées, mettant en œuvre un séquencement planifié de modes d’actions sur plusieurs composants – techniques et humains généralement – du produit et de son écosystème._

_De même que pour l’identification des événements redoutés, dans un objectif d’efficacité, l’équipe s’intéresse en priorité aux abuser stories associés aux sources de risques les plus prégnantes._

La section suivante présente l'intégralité de l'analyse des risques pour la plateforme Le.Taxi et vous permettra d'observer l'articulation des différents éléments présentés ici sur un cas pratique.

