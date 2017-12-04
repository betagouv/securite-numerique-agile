## L'analyse des risques: les bases à connaitre et transmettre

La valeur métier correspond à la valeur livrée aux utilisateurs et s’articule en users stories. Les users stories au niveau le plus macroscopique (epics) représentent un enjeu de sécurité significatif vis-à-vis de l’un ou l’autre des critères suivants :
-  [D] Disponibilité : la fonctionnalité peut être utilisée au moment voulu ;
-  [I] Intégrité : les données sont exactes et complètes ;
-  [C] Confidentialité : les informations ne sont divulguées qu'aux personnes autorisées ; 
 - [P] Preuve : les traces de l’activité du système sont opposables en cas de contestation.

De par leur criticité vis-à-vis des enjeux opérationnels et réglementaires de l'organisme, les epics doivent être protégées face aux menaces jugées plausibles (attaques informatiques, actes de fraude, erreurs, défaillances, etc.)

### Exemple (plateforme dématérialisée de mise en relation de taxis et de clients) :

Un risque décrit la réalisation d’un scénario de menace intentionnel ou accidentel :
1. une source de menace
2. par le biais d’un composant vulnérable du SI
3. provoque un événement redouté
4. sur une valeur métier essentielle, occasionnant des impacts directs et indirects (humains, opérationnels, juridiques, etc.)

Chacune de ces catégories correspondra à une couleur de post-its. Voici une suggestion pour la correspondance entre les couleurs:
- Vert pour les “user stories” macroscopiques (parfois appelées “epics”), que vous annoterez avec les besoins de sécurité énumérés ci-dessus
- Orange pour les sources de menace, le plus souvent des catégories d’attaquants
- Bleu pour les composants du SI
- Rouge pour les événements redoutés

Commencez par ces quatre catégories qui ont tendance à constituer “l’angle mort” pour beaucoup d’équipes. Réservez une couleur plus classique, le jaune, pour lister séparément et à la fin de l’exercice:
- les mesures de sécurité déjà mises en place
- les mesures de sécurité à prendre, déjà connue ou qui ont émergé de la discussion

Cette correspondance n’est qu’une suggestion, c’est ce qui a marché pour nous; n’hésitez pas à en dévier si cela a du sens pour vous.

La notion d’une Abuser Story peut être intéressante pour les équipes déjà familières du jargon agile, puisqu’elle correspond au “revers” néfaste d’une “User Story”:

```
En tant que <attaquant>
Lorsque <un composant est vulnérable>
Afin de <provoquer un impact négatif>
Je souhaite <déclencher un événement redouté>
```
