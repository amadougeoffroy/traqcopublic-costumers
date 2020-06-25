>## Fenêtre contextuelle de l'objet

<img src="docs/_image/fenetrecontaxtuelle.png" alt="fenetrecontaxtuelle" width="380px">

Dans la fenêtre contextuelle réduite, vous pouvez surveiller les informations de base et les capteurs. Une fois que vous avez cliqué sur «Afficher plus», vous verrez toutes les informations disponibles pour cet appareil, y compris les capteurs, les services et les données supplémentaires. Si vous souhaitez vérifier les paramètres que votre appareil envoie, veuillez visiter la section de gestion des capteurs.

<img src="docs/_image/appercurue.png" alt="appercurue" width="580px">

Il est également possible d'utiliser "l'aperçu de la rue" tout en surveillant votre appareil. Cette fenêtre s'actualisera automatiquement une fois que votre appareil se déplacera, vous pourrez donc "prévisualiser la rue" en temps réel.

>## Outils rapides d'objet

<img src="docs/_image/outilsrapides.png" alt="outilsrapides" width="580px">

1. ***Afficher l'historique***  - cela affichera instantanément l'historique de l'objet pour la période sélectionnée la plus courante.
2. ***Suivre***  - une nouvelle fenêtre apparaîtra où vous pourrez surveiller chaque objet individuellement, vous pouvez ouvrir plusieurs fenêtres en même temps.
3. ***Envoyer la commande***  - accès rapide pour envoyer la commande à l'appareil via gprs ou sms.
4. ***Modifier*** - modifiez le nom de l'appareil, imei, la précision, l'icône de changement, ajoutez des services et plus encore.

>## Modifier - Principal

<img src="docs/_image/mainedit.png" alt="mainedit" width="580px">

Pour ajouter un appareil, tout est requis: nom et nom de l'appareil ou identifiant. Vous pouvez modifier le nom et imei naytime.

>## Modifier - Icônes

<img src="docs/_image/editicones.png" alt="editicones" width="580px">

***Type d'icône:***

* ***Flèche*** - une flèche avec direction et couleur (vert, jaune, rouge) sera affichée. C'est la sélection par défaut et recommandée car elle vous donne le plus de contrôle et d'informations.
* ***Icône de rotation*** - l'icône du véhicule visible du haut sera affichée, elle tournera selon la direction.
* ***Icône*** - une icône simple sera affichée sans direction ni statut.

***Type d'icône - Flèche. Il y a 4 états:***

* ***Déplacement*** - lorsque la vitesse de l'appareil est supérieure à la vitesse minimale définie dans edit-> precision-> min. Vitesse de déplacement
* ***Arrêté*** - lorsque la vitesse de l'appareil est inférieure à la vitesse minimale définie dans éditer-> précision-> min. Vitesse de déplacement
* ***Hors ligne*** - si l'appareil n'envoie pas d'informations au serveur pendant 5 minutes ou plus ou s'il est déconnecté du serveur gps
* ***Ralenti du moteur*** - pour que le ralenti du moteur soit actif, vous devez ajouter un capteur d'allumage / extinction ou allumage / extinction du moteur, puis ajouter ces capteurs dans éditer-> précision-> heures du moteur (passer du gps). Le ralenti du moteur signifie que le contact / moteur est mis mais que l'appareil ne bouge pas.

>## Modifier - Avancé

<img src="docs/_image/advanced.png" alt="advanced" width="580px">

Dans la section avancée, vous pouvez remplir des informations facultatives, attribuer un appareil au groupe (pour créer un nouveau groupe, allez dans Configuration-> Groupes-> Ajouter).
 
* ***Afficher uniquement les commandes GPRS Tempaltes*** - si vous la cochez, seules les commandes gprs personnalisées seront affichées pour votre appareil dans Outils-> Commande Envoyer. Les modèles GPRS peuvent être créés dans Setup-> GPRS Tempaltes
* ***Mesure de carburant*** - si vous n'avez pas de capteurs de carburant connectés à votre appareil GPS, vous pouvez saisir des mesures ici afin qu'elles correspondent dans l'historique et les rapports.
* ***Transférer*** - La plate-forme copiera et enverra les données brutes du périphérique à l'adresse IP et au port donnés dans une connexion UDP ou TCP.
* ***Réglage de l'heure*** - cela ajustera manuellement l'heure individuellement pour le périphérique GPS sélectionné. Utilisé uniquement dans ces cas, lorsque vous ne parvenez pas à définir le fuseau horaire sur UTC 0 pour votre appareil.

>## Édition - Capteurs

Veuillez consulter la page de gestion des capteurs pour une documentation détaillée.

>## Modifier - Services

<img src="docs/_image/servicesedit.png" alt="servicesedit" width="580px">

Les services sont utilisés pour surveiller les assurances, la maintenance technique, le changement d'huile, la dépréciation des pièces automobiles, etc.

>## Modifier - Précision

<img src="docs/_image/precisionedit.png" alt="precisionedit" width="580px">

* ***Heures moteur*** - la sélection par défaut est le GPS, mais si vous avez un allumage ou un capteur moteur connecté à votre tracker gps, il est fortement recommandé de le sélectionner ici. Une fois sélectionné, si le contact est coupé, vous ne verrez pas l'historique inutile (comme la dérive), les heures du moteur, la distance, les événements comme la barrière géographique ou la survitesse ne seront pas déclenchés, vous obtiendrez donc les informations les plus précises, y compris les rapports.
* ***Min. vitesse de déplacement*** - si la vitesse est inférieure à min. vitesse, le déplacement ne sera pas enregistré.
* ***Min. différence de carburant pour détecter les remplissages de carburant*** - si la valeur du capteur augmente instantanément de 10 unités ou plus, le remplissage de carburant sera détecté.
* ***Min. différence de carburant pour détecter les vols de carburant***  - si la valeur du capteur diminue instantanément de 10 unités ou plus, le vol de carburant sera détecté.

Pour éviter que la plate - forme d'enregistrement faux mouvement lors d'un séjour à un endroit et les points GPS ne sont pas exacts « Valeur minimale « de Vitesse de déplacement doit être augmentée Additionaly si l' appareil dispose d' un capteur d'allumage -.. Ajouter arrêtera la plate - forme l' enregistrement des points de localisation lorsque le contact de l' objet est éteint.

>## Édition - Queue

<img src="docs/_image/editqueue.png" alt="editqueue" width="580px">

* ***Couleur de la queue*** - sélectionnez la couleur de la queue de l'objet
* ***Longueur de la queue*** - quelle est la longueur de la queue