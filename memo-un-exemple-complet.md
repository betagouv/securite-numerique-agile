# Un exemple complet

Voici à titre d'illustration l'exemple détaillé du service Le.Taxi développée par l'Incubateur de Services Numériques de la DINSIC, extrait du Wiki: https://github.com/openmaraude/le.taxi/wiki/Anayse-des-risques

Les tableaux que nous livrons ci-dessous correspondent à la restitution formelle d'un des ateliers d'analyse des risques, sans retouche (autres que des évolutions de terminologie en cours de rédaction) ou ajout.

| User story | Besoin de sécurité |
|---------------|--------------------|
|Un taxi peut remonter sa position via l'API|Disponibilité : une position doit remonter sous 5 minutes<br/> Intégrité : altérations détectables|
|**Un client et un taxi conviennent d'une course** (scénario global décomposé en sous-scénarios ci-dessous)|Disponibilité : sous 5 minutes<br/>Intégrité : altérations détectables et corrigeables<br/>Confidentialité : l'information sur les courses est à diffusion limitée|
|Un client peut connaître les taxis à proximité (ou suivre un taxi en approche)|_idem_|
|Un client peut émettre une demande (« héler virtuellement » un taxi)|_idem_|
|Le taxi, puis le client peuvent confirmer la prise en charge|_idem_|
|Le taxi ou le client peut annuler la course|_idem_|
|Un client peut évaluer la course|Disponibilité : sous 72h|
|Un taxi peut signaler un problème lié à une course|Disponibilité : sous 72h|
|Un partenaire peut enregistrer un véhicule|Disponibilité : sous 72h<br/>Intégrité : altérations détectables|
|Un administrateur peut enregistrer un partenaire|Disponibilité : sous 72h<br/>Intégrité : altérations détectables|
|Un administrateur peut consulter les stats partenaires|Confidentialité : les statistiques sont à diffusion limitée|

| **Source de risques** | **Mode opératoire** | Vraisemblance |
|---------------|---------------|---------------|
|Attaquants externes (clients, hackers)| Un attaquant externe accède à la base de données | *** |
|Attaquants externes (clients, hackers)| Un attaquant externe surcharge le système | ** |
|Acteurs agréés (taxis, opérateurs) de mauvaise foi| Un partenaire surcharge le système | ** |
|Acteurs agréés (taxis, opérateurs) de mauvaise foi| Un partenaire tente de fausser la concurrence en envoyant de fausses positions | * |

| **Evenement redouté** | **Impact métier** | Sévérité |
|---------------|---------------|---------------|
| Le système ne répond pas | Expérience utilisateurs dégradée -> perte de clients | *** |
| Un opérateur de taxis émet de fausses positions | Fausses adéquations clients-taxi -> perte de clients| *** |
| Un taxi fait une course d'approche en pure perte | Manque d'adhésion des taxis -> offre trop faible | ** |
| Un taxi s'enregistre avec de fausses informations | Captation abusive de courses -> perte de confiance, risque juridique | * |

| **Composant du système** |
|---------------|
| [API](https://en.wikipedia.org/wiki/Application_programming_interface) TXP (Taxi Exchange Point) |
| Serveurs (1 serveur actuellement) |
| Données stockées |
| Administrateurs |
| Partenaires |

Les risques suivants sont actuellement traités par les mesures citées:

| Risque | Mesure existante |
|---------------|--------------------|
|Un partenaire tente de fausser la concurrence en envoyant de fausses positions|Signature cryptographique des remontées de positions par les partenaires|
|Un attaquant externe accède à des informations confidentielles en exploitant une faille|Fermeture des ports autres que HTTP/HTTPS au trafic issu d'adresses IP inconnues|
|Un attaquant externe accède à des informations confidentielles en usurpant l'identité du serveur|Echanges sécurisés par HTTPS|
|Un client de mauvaise foi hèle un taxi sans intention d'honorer sa commande|Transaction en 2 étapes, bannissement temporaire des clients abusifs|
|Un taxi fournit des courses ne respectant pas la qualité de service attendue|Enregistrement d'une notation attribuée par le client au taxi|
|Un client de mauvaise foi attribue abusivement une mauvaise note au taxi|Les notations sont associées à une course réelle spécifique|

Les risques résiduels suivants sont acceptés provisoirement, mais doivent être traités par les mesures citées en regard:

| Risque résiduel | Mesure à prendre |
|---------------|--------------------|
|Le système est indisponible suite à un déni de service|Redonder les serveurs|
|Un taxi ou VTC usurpe l'identité d'un véhicule légitime|En cours d'instruction|
