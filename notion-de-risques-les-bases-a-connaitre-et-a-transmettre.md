## L’appréciation des risque : les bases à connaitre et à transmettre

**La valeur métier correspond à la valeur livrée aux utilisateurs et s’articule en *users stories*.** Les *users stories* au niveau le plus macroscopique (parfois appelées *epics*) revêtent généralement un enjeu de sécurité significatif vis-à-vis de l’un ou l’autre des critères suivants :

* \[D\] Disponibilité : la fonctionnalité peut être utilisée au moment voulu ;
* \[I\] Intégrité : les données sont exactes et complètes ;
* \[C\] Confidentialité : les informations ne sont divulguées qu'aux personnes autorisées ; 
* \[P\] Preuve : les traces de l’activité du système sont opposables en cas de contestation.

De par leur criticité vis-à-vis des enjeux opérationnels et réglementaires de l'organisme, ces qualités doivent être protégées face aux menaces jugées vraisemblables \(attaques informatiques, actes de fraude, erreurs, défaillances, etc.\)

### Exemple \(Le.Taxi\) :

| **User story** | **D** | **I** | **C** | **P** |
| --- | --- | --- | --- | --- |
| Un client transmet son identifiant, sa position et son numéro de téléphone | \* | \* | \* \* |  |
| Un client peut évaluer une course effectuée ou déclarer un incident |  | \* |  | \* |
| Un administrateur peut enregistrer ou radier un taxi |  | \* |  | \* |

> * * besoin important \* besoin notable

### Des besoins de sécurité aux événements redoutés

Chaque besoin de sécurité identifié constitue le point de départ pour décrire un ou plusieurs événements redoutés susceptibles de compromettre la valeur d'usage.

| **Evenements redoutés** | **Impact métier** | Sévérité |
| --- | --- | --- |
| Le système ne répond pas | Expérience utilisateurs dégradée -&gt; perte de clients | _\*_ |
| Un opérateur de taxis émet de fausses positions | Fausses adéquations clients-taxi -&gt; perte de clients | _\*_ |
| Un taxi fait une course d'approche en pure perte | Manque d'adhésion des taxis -&gt; offre trop faible | \*\* |
| Un taxi s'enregistre avec de fausses informations | Captation abusive de courses -&gt; perte de confiance, risque juridique | \* |

### Les risques résultent de la combinaison des éléments de l'analyse

Un risque décrit la réalisation d’un scénario de menace intentionnel ou accidentel :  
1. une source de risque \(un attaquant par exemple\)  
2. par le biais d’un composant vulnérable du SI  
3. provoque un événement redouté  
4. occasionnant des impacts sur la valeur métier, directs et indirects \(humains, opérationnels, juridiques, etc.\)

On lui associe une _criticité_ basée sur l'estimation conjointe de la _gravité_ des impacts et de la _vraisemblance_ du scénario de menace conduisant à l'événément redouté.

Chacune des 4 catégories ci-dessus correspondra à une couleur de post-its. Voici une suggestion pour la correspondance entre les couleurs:

* Bleu pour les “user stories” macroscopiques, que vous annoterez avec les besoins de sécurité énumérés ci-dessus
* Orange pour les sources de risque, le plus souvent des catégories d’attaquants
* Vert pour les composants du SI
* Rouge pour les événements redoutés

Commencez par ces quatre catégories qui ont tendance à constituer “l’angle mort” pour beaucoup d’équipes. Réservez une couleur plus classique, le jaune, pour lister séparément et à la fin de l’exercice:

* les mesures de sécurité déjà mises en place
* les mesures de sécurité à prendre, déjà connues ou qui ont émergé de la discussion

Cette correspondance n’est qu’une suggestion, c’est ce qui a marché pour nous; n’hésitez pas à en dévier si cela a du sens pour vous.

La notion d’une Abuser Story peut être intéressante pour les équipes déjà familières du jargon agile, puisqu’elle correspond au “revers” néfaste d’une “User Story”:

```
En tant que <attaquant>
Lorsque <un composant est vulnérable>
Afin de <provoquer un impact négatif>
Je souhaite <déclencher un événement redouté>
```



