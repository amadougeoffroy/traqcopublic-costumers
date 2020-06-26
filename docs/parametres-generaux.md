>## Paramètres disponibles

Les paramètres globaux sont utilisés dans le panneau d'administration -> Configuration -> Ports de suivi. Cliquez sur modifier près du numéro de port et saisissez le nom et la valeur du paramètre ci-dessous dans la section "Extra".
 
**Liste des paramètres disponibles:**
 
* ***ignoreFixTime / true ou false*** - principalement utilisé pour les appareils Queclink, si vous rencontrez des "sauts" dans l'historique, veuillez définir cette valeur sur false.
* ***étendu / vrai ou faux*** - pour le protocole xexun uniquement
* ***can / true ou false*** - pour le protocole aplicom uniquement
* ***hbm / true or false*** - protocole suntech
* ***includeAdc / true ou false*** - protocole suntech
* ***timeout / 1-9999*** - valeur du délai de connexion en secondes. Parce qu'il est parfois impossible de détecter une connexion TCP perdue, les anciennes connexions restent ouvertes. Sur la plupart des systèmes, le nombre de connexions ouvertes est limité, ce qui entraîne des problèmes pour établir de nouvelles connexions lorsque le nombre de périphériques est élevé ou que les connexions de données des périphériques sont instables.
* ***timeoverride / true ou false*** - une fois activé, l'heure du tracker gps sera décodée de la même manière que l'heure du serveur, cela résoudra le problème si le tracker envoie toujours une date et une heure incorrectes.

