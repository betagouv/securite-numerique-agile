## Les ateliers suivants, itération après itération

Au fil des itérations, il deviendra périodiquement nécessaire d’actualiser ou d’affiner le résultat du premier atelier, par exemple lors des événements suivants :

* la réalisation d’une *user story* induit des évolutions d’architecture telles que l’ajout ou la modification d’un composant technique ;
* la réalisation d’une *user story* amène à exposer des données d’une autre nature que celles précédemment traitées \(des données personnelles par exemple, alors que ce n’était pas le cas auparavant\) ;
* l’équipe réalise un atelier dédié à une fonctionnalité spécifique du produit, qui adresse une ou plusieurs *user stories* plus particulièrement sensibles en termes de sécurité ;
* les retours des usagers amènent à évaluer différemment la valeur métier des différentes *user stories* ou les besoins de sécurité qui leur sont associés ;
* le nombre d’usagers ou le volume de transactions métier a sensiblement évolué, de telle sorte que l’exposition totale au risque a elle aussi évolué.

Comme pour les autres activités menées par les équipes agiles, le travail à réaliser alors est quasiment le même que lors du premier atelier. Au fil des itérations, l'équipe apprendra ainsi à tenir compte, dans son plan de charge, du temps consommé par les activités liées à la sécurité afin de lisser ce travail dans le temps - comme elle le fait pour les activités liées à la qualité.

### Dette sécuritaire

Par analogie avec la dette technique, une équipe peut être amenée à différer le traitement de certains risques, dans le but de mettre plus rapidement de nouvelles version du produit ou du service entre les mains des usagers afin d'obtenir des retours ; on parlera alors de « dette sécuritaire ».

Notez cependant que le terme de « dette technique » sert trop souvent d'excuse à des équipes qui ne maîtrisent pas réellement la qualité de leur code. Il est risqué de privilégier systématiquement la réalisation de nouvelles fonctionnalités sans investir dans des pratiques de conception telles que le refactoring, l'automatisation en soutien du test ou la mise en commun des connaissances. On pourra observer de la même manière une carence d'attention portée à l'analyse de risques.

Dans les deux cas, un atelier d'analyse des risques tel que nous l'avons décrit ci-dessus peut amener l'équipe à réserver une part importante de sa capacité, ou consacrer une itération entière, à la prise en compte de la sécurité du système.

