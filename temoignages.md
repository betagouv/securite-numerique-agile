# Témoignages

Cette section est amenée à s'enrichir au fil des contributions \(voir la section suivante\). Nous avons choisi d'y présenter pour l'instant quelques retours qui nous paraissaient saillants à l'issue du premier appel à commentaires lancé par l'ANSSI et la DINSIC en septembre 2017.

### Témoignage de Thomas Coquelin \(1er appel à commentaires\)

> Nous n’avons pas de contraintes d’homologation par une autorité de contrôle externe à chaque mise en production.
>
> Le délai typique entre le début de l’implémentation d’une User Story et sa mise en production va d’une semaine pour une US volumineuse à quelques dizaines de minutes pour un bug critique en production.
>
> Voici ce que nous essayons de mettre en place :
>
> * Dissociation des fonctions de contrôle SSI des fonctions d’accompagnement sécurité \(coachs\)
> * Les coach forment les équipes à la SSI et accompagnent la mise en place de la méthode
> * Le PO et l’équipe étudient les questions de sécurité lors du Story Mapping, ils sollicitent des expertises SSI spécifiques.
> * Chaque User Story comporte une classification DICP des valeurs métier, des événements redoutés avec les scenarios de risques associés pondérés, les critères d’acceptation prenant en compte l’atténuation des risques.
> * Le story Mapping produit également des User Story dédiées à des problèmes de sécurité, elles sont taggés « abuser story » mais répondent au même formalisme que les autres User Story.
> * Toutes les Users Stories sont pondérées en charge et en valeur. La valeur d’une « abuser story » est fonction du risque qu’elle couvre.
> * Lors de l’implementation de la User Story, le dossier de sécurité est mis à jour au même titre que le reste de la documentation. On a donc une vue incrémentale de la securité dans les User Stories et globale dans le dossier de sécurité.

### Témoignage de Eric Quinton

> Pour ma part, et pour aller au plus vite \(un objectif des méthodes agiles\) en essayant de couvrir tous les cas de figure, je préfère m’attacher à suivre des référentiels de bonne pratique. J’utilise d’ailleurs les critères ASVS de l’OWASP, qui ont l’avantage d’être exhaustifs, réfléchis, adaptés au niveau de sécurité recherché. En les suivant, on s’assure \(au moins en première approche\) de ne pas laisser une faille béante par un simple oubli : je vois malheureusement trop d’applis web litigieuses sur le plan de la sécurité. Par exemple, en 1 an, c’est 2 applis \(une fournie par une municipalité, l’autre par une université\) qui m’ont envoyé mon mot de passe associé à mon login en clair dans ma messagerie \(sans commentaire\).

### Témoignage d'OccSImore

> La méthode utilisée se rapproche de celle proposée, à ceci près que les exigences de sécurité sont formalisées en début de projet au cours d’un atelier dédié, puis adaptées ensuite au fil des sprints. Elles le sont sous la forme « d’user story » fonctionnelles ou techniques. Le projet fait ensuite appel à sa discrétion à l’expert SSI qui lui est affecté. Les risques sont évalués à la fin du projet et en fonction du niveau de risque, le Product Owner \(PO\) peut décider d’accepter que le produit soit proposé à la mise en production. Au-delà d’un certain niveau de risque, une instance hors du projet doit se prononcer.
>
> Les sachants SSI sont aujourd’hui en général en sous-effectif dans les organisations. De plus, ces profils dans le domaine du développement sont encore plus rares. Les organisations peuvent donc être confrontées à des difficultés quant à la mise en œuvre de la démarche par l’impossibilité d’affecter une ressource. L’intégration systématique risque d’être une pratique impossible à suivre. A défaut, la présence de l’expert SSI lors de la réunion de planification, ainsi qu’une rencontre régulière entre le PO et l’expert SSI est indispensable.





