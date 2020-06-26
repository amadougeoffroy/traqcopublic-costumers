>## Vue d'ensemble

Il s'agit du panneau d'administration vu par l'utilisateur qui appartient au groupe d'utilisateurs Admin.

<img src="docs/_image/paneauadmin.png" alt="paneauadmin" width="650px">

Le menu supérieur comprend un logo pour l'image de marque de l'entreprise.

***Carte***  - ouvre la fenêtre principale de la carte de l'utilisateur.

***Utilisateurs***  - ouvre le panneau pour la liste des utilisateurs et les outils correspondants.

***Objets***  - ouvre un panneau pour la liste des objets et des outils pour la gestion des objets.

***Événements***  - ouvre un menu pour la création globale d'événements.

***Contenu***  - ouvre un menu pour les modèles d'e-mail, les modèles SMS, les icônes de carte et les icônes d'objet.

***Configuration***  - ouvre un menu pour les e-mails, les paramètres du serveur principal, la gestion des utilisateurs, la configuration des ports, les traductions linguistiques, les adresses IP bloquées, les outils supplémentaires, les plugins et les groupes de capteurs. 

***Journaux***  - ouvre un menu pour les journaux du serveur, les journaux des appareils non enregistrés et également le journal des rapports planifiés.

Les boutons de nom de compte d'utilisateur se composent d'un menu pour le suivi du bouton de redémarrage du service et du bouton de déconnexion de l'utilisateur.
Le pied de page de la page fournit des informations sur le nom de la plateforme, l'adresse IP de la plateforme, la version de la plateforme et la dernière date de mise à jour.
 
 
Le panneau d'administration pour l'utilisateur d'un groupe d'utilisateurs Manager se compose de différentes options de menu. L'utilisateur Manager a la possibilité d'avoir sa propre image de marque dans le menu " ***Logo*** ".

<img src="docs/_image/paneauadmin2.png" alt="paneauadmin2" width="650px">

>## Configuration

Panneau d'administration - Le programme d'installation dispose du menu de configuration de la messagerie, des paramètres du serveur, etc.

<img src="docs/_image/paneauadmin3.png" alt="paneauadmin3" width="180px">

>#### Email

<img src="docs/_image/paneauadminemail.png" alt="paneauadminemail" width="650px">

La configuration de la messagerie à l'aide du fournisseur par défaut nécessite de remplir uniquement ces champs:
***De nom***  - entrez un nom d'expéditeur

***Aucune adresse e-mail de réponse***  - entrez une adresse e-mail qui correspond à l'e-mail de l'expéditeur.

***Signature***  - entrez une signature qui apparaîtra dans chaque e-mail en bas de page.

***Utiliser un serveur SMTP***  - non.
 
Il existe au total 4 fournisseurs de messagerie parmi lesquels choisir - par défaut (serveur), Sendgrid, Postmark, Mailgun.

<img src="docs/_image/paneauadminemail2.png" alt="paneauadminemail2" width="450px">

Sengrid nécessite une clé API pour fonctionner.

<img src="docs/_image/paneauadminemail3.png" alt="paneauadminemail3" width="650px">

>#### Utilisateur

Le panneau "Utilisateur" offre la possibilité d'appliquer des paramètres à tous les nouveaux utilisateurs.

<img src="docs/_image/paneauadminuser.png" alt="paneauadminuser" width="650px">

***Autoriser l'enregistrement*** - Si activé, les nouveaux utilisateurs peuvent s'inscrire à partir de l'écran de connexion de la plateforme.

 * ***Activer les plans*** - Cette option active les plans pour les utilisateurs. Chaque plan peut être configuré pour autoriser des fonctionnalités spécifiques, une limite d'appareil et une période pour un prix fixe.
Fuseau horaire par défaut - Ce paramètre applique un fuseau horaire à tous les nouveaux utilisateurs enregistrés / créés.

***Heure d'été*** - Le cas échéant, définissez la date de l'heure d'été.

***Limite d'appareils*** - Un nombre défini d'appareils que l'utilisateur est en mesure de créer ou il peut être désactivé pour permettre un nombre illimité d'objets. (Ce paramètre ne s'applique que si les plans ne sont pas activés)

***Expiration de l'abonnement après plusieurs jours*** - Durée spécifique jusqu'à l'expiration de l'utilisateur après la première inscription. Peut également être désactivé. (Ce paramètre ne s'applique que si les plans ne sont pas activés)

***Autorisations*** - Ce sont les autorisations pour les fonctionnalités que chaque nouvel utilisateur recevra lors de l'inscription. (Ce paramètre s'applique uniquement si les plans ne sont pas activés)

Pour ajouter des plans payants aux utilisateurs, l'option "Activer les plans" doit être cochée.
Dans le coin droit de l'onglet "Plans", sélectionnez le "+" pour créer un nouveau plan.

<img src="docs/_image/paneauadminuser2.png" alt="paneauadminuser2" width="650px">

Une nouvelle fenêtre s'ouvrira, vous invitant à remplir le titre du plan, le prix, la limite d'objet et la durée. Dans l'onglet "Autorisations", vous pouvez sélectionner les fonctionnalités que l'utilisateur peut utiliser pour des plans spécifiques. La devise est utilisée en fonction des paramètres de l'onglet "Passerelle de facturation".

<img src="docs/_image/paneauadminuser3.png" alt="paneauadminuser3" width="650px">

>#### Passerelle de facturation

Dans cet onglet, vous pouvez configurer des passerelles de paiement si des plans payants sont créés et activés.
Chaque passerelle de paiement nécessitera un jeu de clés et d'autres informations remplies pour fonctionner. Veuillez vous référer à la documentation fournie par la passerelle ou contacter leur support pour obtenir de l'aide sur l'acquisition des informations requises.

>#### Ports de suivi

Il s'agit d'une liste de tous les ports pour chaque protocole intégré.

<img src="docs/_image/portsuivi.png" alt="portsuivi" width="650px">

Dans cet onglet, vous pouvez activer / désactiver, modifier le numéro de port du protocole et ajouter des paramètres supplémentaires si nécessaire. Tous les paramètres peuvent être trouvés ici .

<img src="docs/_image/portsuiviadd.png" alt="portsuiviadd" width="650px">

>#### Les langues

Il s'agit d'une liste de toutes les langues disponibles sur la plateforme.
S'il y a des traductions incorrectes pour votre langue, vous pouvez les ajuster dans les paramètres de langues. Ils sont situés à droite de l'écran. Sous "Actions", sélectionnez "Traduire" pour corriger les traductions.
Le nom et la disponibilité de la langue peuvent également être modifiés à l'aide de l'option "Modifier".

>#### IP bloquées

Avec cet outil, vous pouvez bloquer une adresse IP pour éviter d'inonder le serveur de messages indésirables provenant d'un périphérique ou d'un serveur.
Pour bloquer une adresse IP, sélectionnez l'icône "+" à droite de l'écran.

<img src="docs/_image/ipbloques.png" alt="ipbloques" width="550px">

>#### Outils

À partir de l'onglet "Outils", il existe des contrôles pour les sauvegardes et le nettoyage de la base de données.

>#### Sauvegardes de bases de données

<img src="docs/_image/database.png" alt="database" width="650px">

**Type:**

***Automatique*** - celles-ci sont effectuées automatiquement par le système sur nos serveurs externes si le plan de sauvegardes quotidiennes est actif.

***Personnalisé*** - permet de télécharger des sauvegardes de base de données sur votre propre serveur externe.

***Période*** : à quelle fréquence le système doit envoyer des sauvegardes à un serveur externe.

***Heure*** : pendant quelle heure les sauvegardes de la base de données doivent être planifiées. L'heure est prise à partir de l'heure actuelle des serveurs.

Nettoyage de la base de données d'historique de l'appareil
Les options suivantes vous permettent de contrôler la fréquence de nettoyage de la base de données. Ceci est utilisé pour éviter d'inonder la base de données, ce qui entraînera des problèmes de disponibilité des logiciels.

<img src="docs/_image/databaseclean.png" alt="databaseclean" width="550px">

Pour que le système nettoie automatiquement la base de données, le "Nettoyage automatique des données d'historique" doit être activé.

Le système permet 2 méthodes de nettoyage:

***Heure du serveur*** - cette option nettoie la base de données tous les 30 jours pour chaque appareil depuis le premier démarrage du logiciel.

***Dernière connexion*** - cette option nettoie la base de données tous les 30 jours depuis la première connexion des appareils.

***Taille actuelle de la base de données*** - combien la base de données prend de l'espace sur le disque dur.

>#### Plugins

À partir de cet onglet, vous pouvez activer certains outils et fonctionnalités qui ne sont pas activés par défaut.
Tous les plugins et explications peuvent être trouvés ici .

>#### Groupes de capteurs

Avec cet outil, vous pouvez créer un groupe de capteurs à partir duquel plusieurs capteurs peuvent être appliqués à un appareil en même temps. Cela permet d'éviter le processus manuel de création des mêmes capteurs pour chaque appareil individuellement.
Pour créer un groupe de capteurs, sélectionnez l'icône "+" dans le coin droit. Une fois le menu affiché, accordez un titre au groupe de capteurs et appuyez sur Enregistrer. Le groupe de capteurs apparaîtra dans la liste. Pour ajouter des capteurs au groupe, sous les actions à droite, sélectionnez l'icône d'engrenage et appuyez sur modifier.

<img src="docs/_image/groupecapteurs.png" alt="groupecapteurs" width="550px">

Vous pouvez ajouter autant de capteurs que nécessaire. Une fois les capteurs créés, accédez à l'onglet capteur de l'objet et en bas du menu, sélectionnez le groupe de capteurs que vous avez créé dans la liste déroulante "Groupes de capteurs".

<img src="docs/_image/capteuredit.png" alt="capteuredit" width="550px">

>#### Passerelle SMS

Cet outil est utilisé pour transférer des messages SMS de la plate-forme vers un appareil de suivi ou un téléphone mobile. Soit pour la configuration automatique du dispositif de suivi GPS, soit pour recevoir des alertes.
Le service de passerelle SMS doit être acheté auprès d'un fournisseur externe, tel que Plivo, BulkSMS ou tout autre.
Nous avons également une application SMS Gateway pour les appareils Android, qui transmettra les messages SMS à d'autres utilisateurs, appareils. L'application peut être téléchargée ici .

<img src="docs/_image/passerellesms.png" alt="passerellesms" width="650px">

***Activer la passerelle SMS*** - Activez ou désactivez la passerelle SMS configurée dans le panneau d'administration pour les autres utilisateurs. Dans ce cas, chaque utilisateur devra configurer sa propre passerelle SMS.

***Utiliser la même passerelle pour les messages système*** - Permet aux utilisateurs d'utiliser la passerelle configurée dans le panneau d'administration pour les messages système, par exemple, l'activation du périphérique GPS.

***Méthode de demande*** - Les méthodes disponibles sont GET et POST. Reportez-vous à la documentation du fournisseur de passerelle SMS pour la méthode correcte.

***En-têtes de passerelle SMS*** - En- têtes requis par le fournisseur de passerelle SMS.

***URL de la passerelle SMS*** - Une chaîne URL complète qui sera utilisée pour envoyer des messages SMS.

