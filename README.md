# Intégrer la sécurité numérique dans une démarche Agile

## Table des matières
### A qui s'adresse ce guide ?
### La prise en compte incrémentale du risque
### L'atelier d'analyse des risques
### Le premier atelier
### Notion des risques: les bases à connaitre et transmettre
### Que faire après l’atelier
### Les ateliers suivants, itération après itération
### Se préparer à une démarche d'homologation
### Formaliser un dossier d'homologation


## A qui s'adresse ce guide ?

Ce guide est intitulé "Intégrer la sécurité numérique dans une démarche Agile". Savoir précisément qui "est" ou "n'est pas" Agile est une question qui entraîne des débats sans fin; nous n'entendons pas répondre à cette question.

Nous avons conçu ce guide pour des équipes dans lesquelles notamment:
- le principal objectif est de livrer rapidement et fréquemment un produit ou un service à ses usagers, pour résoudre un problème auxquels ceux-ci sont confrontés ;
- des personnes dotées de compétences diverses (techniques et non techniques) travaillent ensemble au quotidien ;
- les membres de l'équipe ont assez d'autonomie pour décider ensemble, sans en référer à leur hiérarchie, de l'organisation de leur propre travail ;
- l'équipe porte une attention particulière à la qualité de ce qu'elle produit, s'outille en conséquence et cherche en permanence à s'améliorer.

Quant à la question de la sécurité numérique, elle concerne toutes les organisations et tous les types de projets. Ce guide ne prétend pas couvrir le sujet de façon exhaustive, mais à donner des éléments pratiques et concrets pour les équipes revendiquant une démarche Agile et présentant les caractéristiques ci-dessus.

Généralement, ces caractéristiques s'observent dans des équipes plutôt réduites, et s'accompagnent de pratiques telles que le management visuel (task board, etc.), l'utilisation systématique de tests automatisés, le déploiement continu et les outils Devops, le cadencement du travail en itérations, et ainsi de suite; cependant, prises individuellement aucune de ces propriétés n'est essentielle à "l'Agilité".

Nous désignons l'ensemble des intervenants d'une telle équipe par le terme "équipe produit". Afin d'éviter de trop ancrer notre discours dans celui de telle ou telle "chapelle" de cette grande communauté qu'est le mouvement Agile, nous ne distinguerons pas les rôles au sein de l'équipe de façon plus spécifique.

http://agilefocus.com/2009/02/06/agile-versus-agile/
http://referentiel.institut-agile.fr/

## La prise en compte incrémentale du risque: la clé de la "compatibilité" Agile

Dans une démarche EBIOS classique, l'équipe définit les enjeux de sécurité de l'application et les façons d'y répondre dès la phase de conception du projet. Certains risques sécuritaires impacteront l'expérience utilisateur avant même que le service ait un premier utilisateur.

Dans une démarche Agile, l’équipe cherche à livrer très tôt de la valeur à un public quie se veut croissant. Voici par exemple, illustrées graphiquement, deux conceptions opposées de ce que devrait être la “courbe de diffusion” d’un outil informatique.


Pour une équipe dont l'objectif est de livrer rapidement de la valeur à ses utilisateurs, l'évaluation du risque se fait en fonction du produit du nombre d’usagers par le risque encouru par chaque usager, pour déterminer une exposition totale réelle au risque d’attaques numériques.

Ainsi la prise en compte des enjeux de sécurité par une équipe agile est continue - tout au long de la construction et de l'amélioration du service - et "pragmatique" (note de bas de page: le terme n’est pas exactement celui qui convient, nous avons en tête quelque chose comme “satisficing” https://fr.wikipedia.org/wiki/Satisficing mais il n’a pas d’équivalent français) - qui priorise les efforts en fonction du risque réel et assume l’existence de risques résiduels.

La façon de traiter la question de la sécurité numérique est donc très différente. La figure ci-dessous superpose à la courbe de diffusion une courbe hypothétique représentant le jugement qu’un expert en sécurité pourrait porter sur un produit numérique.
L’important est donc de s’assurer qu’on arrive au point d’inflexion en ayant couvert les risques numériques les plus importants et non pas de traiter “tous les risques” en amont.

Consentir un travail conséquent en sécurité numérique en amont de ce point est donc doublement improductif. On aura dépensé des ressources qui auraient pu être investies dans une meilleure compréhension du besoin, alors que le gain réel en termes de sécurité sera resté très marginal.

## L'atelier d'analyse des risques: le coeur de la démarche

L’adage est bien connu: “Le meilleur moment pour planter un arbre, c’était il y a 20 ans; le deuxième meilleur moment, c’est maintenant.” En matière de sécurité numérique, le meilleur moment, c’est dès le début des travaux de réalisation, voire d’investigation. Le deuxième meilleur moment, c’est maintenant

L’atelier type d’analyse de risque lors d’une itération se déroule dans les conditions usuelles
pour des équipes agiles :
le format est présentiel,
toute l'équipe est présente, et seulement l'équipe (éventuellement renforcée d'un animateur ou expert sécurité),
la durée est limitée, quitte à programmer plusieurs ateliers (une durée de une heure minimum à trois heures maximum, avec une pause café, est appropriée).

Le support d’animation de l’atelier peut consister en une feuille au format paper board ou
Post-It géant. Au fur et à mesure de la discussion les éléments d’analyse des risques émergeront sous la forme de post-its de couleurs différentes; en fin d’atelier, voici un exemple du livrable de l’exercice.

[[ Photo ]]
## Le premier atelier

Préalablement au premier atelier, ou en début de séance, il est important de définir le périmètre de l’analyse : qu’est-ce qui est “dedans”, et engage la responsabilité de l’équipe et de sa hiérarchie; qu’est-ce qui est “dehors” et relève éventuellement d’autres acteurs.

Pour lancer ce premier atelier vous pouvez proposer le cadrage suivant: « Nous sommes un mois après le lancement du produit, et vous découvrez avec horreur un article dans la presse nationale qui fait état d’une énorme faille de sécurité exploitée avec succès. Quels sont les scénarios possibles qui vous viennent à l’esprit ?”

Cet exercice permettra de concentrer l’attention des participants sur les enjeux les plus importants, et permettra d’amorcer la discussion. Une fois que celle-ci cesse de produire de nouvelles idées, proposez aux participants de formaliser ce qui a émergé de l’atelier en consultant la section suivante.
L'analyse des risques: les bases à connaitre et transmettre

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
Vert pour les “user stories” macroscopiques (parfois appelées “epics”), que vous annoterez avec les besoins de sécurité énumérés ci-dessus
Orange pour les sources de menace, le plus souvent des catégories d’attaquants
Bleu pour les composants du SI
Rouge pour les événements redoutés

Commencez par ces quatre catégories qui ont tendance à constituer “l’angle mort” pour beaucoup d’équipes. Réservez une couleur plus classique, le jaune, pour lister séparément et à la fin de l’exercice:
les mesures de sécurité déjà mises en place
les mesures de sécurité à prendre, déjà connue ou qui ont émergé de la discussion

Cette correspondance n’est qu’une suggestion, c’est ce qui a marché pour nous; n’hésitez pas à en déviez si cela a du sens pour vous.

La notion d’une Abuser Story peut être intéressante pour les équipes déjà familières du jargon agile, puisqu’elle correspond au “revers” néfaste d’une “User Story”:

En tant que <attaquant>
Lorsque <un composant est vulnérable>
Afin de <provoquer un impact négatif>
Je souhaite <déclencher un événement redouté>

## Que faire après l’atelier

A l’issue du premier atelier, éventuellement de plusieurs ateliers si vous avez besoin de répéter l’exercice, il peut être intéressant d’en formaliser les résultats:

- l’analyse des risques peut être consignée dans un wiki ou autre espace documentaire facilement accessible par tous les membres de l’équipe
- les Abuser Stories peuvent être traitées comme les User Stories et ajoutées au backlog
- si l’équipe le fait pour les User Stories, elles peuvent être priorisées, annotées par leurs définitions de “Done” et éventuellement “Ready”
- la démonstration de la prise en compte des risques associés à une Abuser Story peut être faite par le biais de tests automatisés, comme c’est le cas pour les User Stories: au lieu de démontrer par un test qu’un scénario fonctionnel aboutit, on cherchera à démontrer au contraire qu’un vecteur d’attaque n’aboutit pas

## Les ateliers suivants, itération après itération

Au fur et à mesure des itérations, il va s’avérer périodiquement nécessaire d’actualiser le résultat du premier atelier, par exemple lors des événements suivants:

- la réalisation d’une “user story” induit des évolutions d’architectures telles que l’ajout ou la modification d’un composant technique
- la réalisation d’une “user story” amène à exposer des données d’une nature différente de celles qui étaient traitées (par exemple des données personnelles alors que ce n’étais pas le cas auparavant)
- des retours des usagers amènent à évaluer différement la valeur métier des différentes user stories, ou les besoins de sécurité associées à celles-ci
- le nombre d’usagers ou le volume de transactions métier a évolué sensiblement, de sorte que l’exposition totale au risque a elle aussi évolué

Comme pour les autres activités menées par les équipes agiles, le travail à mener alors est quasiment le même que lors du premier atelier.

## Comment aboutir à une décision d'homologation

- Renvoi vers le Guide en 9 étapes
- Rappeler le rôle de l'homologation
- Les types de décision d'homologation

