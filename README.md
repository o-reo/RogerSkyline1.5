# RogerSkyline1.5
An AdminSys initiation

*Partie Réseau et Sécurité*
Concernant le réseau sur la VM, voici les étapes à réaliser :
• Vous devez créer un utilisateur non root pour vous connecter et travailler.
• Utilisez sudo pour pouvoir, depuis cet utilisateur, effectuer les operations demandant
des droits speciaux.
• Nous ne voulons pas que vous utilisiez le service DHCP de votre machine. A vous
donc de la configurer afin qu’elle ait une IP fixe et un Netmask en /30.
• Vous devez changer le port par defaut du service SSH par celui de votre choix.
L’accès SSH DOIT se faire avec des publickeys. L’utilisateur root ne doit pas
pouvoir se connecter en SSH.
• Vous devez mettre en place des règles de pare-feu (firewall) sur le serveur avec
uniquement les services utilisés accessible en dehors de la VM.
• Vous devez mettre en place une protection contre les DOS (Denial Of Service
Attack) sur les ports ouverts de votre VM.
• Vous devez mettre en place une protection contre les scans sur les ports ouverts
de votre VM.
• Arretez les services dont vous n’avez pas besoin pour ce projet.
• Réalisez un script qui met à jour l’ensemble des sources de package, puis de vos
packages et qui log l’ensemble dans un fichier nommé /var/log/update_script.log.
Créez une tache plannifiée pour ce script une fois par semaine à 4h00 du matin et
à chaque reboot de la machine.
• Réalisez un script qui permet de surveiller les modifications du fichier /etc/crontab
et envoie un mail à root si celui-ci a été modifié. Créez une tache plannifiée pour
script tous les jours à minuit.
