# NGINX-server
![rsz_nginx](https://user-images.githubusercontent.com/47100064/173198813-727c6b09-d901-4118-a76d-ee6ecdbe8ee1.png)

## SPECIFICITE de NGINX
A part le fait que Ngnix est un serveur web puissant, elle peut servir pour le "reverse proxing", "caching", "load balancing", ou "media streaming".
Elle peut aussi être utilisé comme proxy pour le courrier électronique (IMAP, POP3 et SMTP). 

## INSTALLATION
L'installation de Ngnix va dépendre des distributions linux qu'on va utilisé, Mais quelque soit ces systèmes, il faut toujours
éxecuté les commandes en tant que super utilisateur.

### 1- Debian, Ubuntu, ou Linux Mint 
On commence par mettre à jour la liste des paquets d'installation

`apt-get update`

On peut maintenant l'installé avec

 `apt install nginx`
 
 ###  2- Fedora, CentOS, ou Red Hat
 Il faut toujours commencé par un mis à jour des paquets d'installation
 
 `sudo dnf upgrade`
 
 Puis l'installation
 
 `sudo dnf install nginx`
 
 ### 3- Arch Linux et Manjaro
 ici on peut immédiatement procédé à l'installation
 
 `sudo pacman -Syu`
 
 `sudo pacman -S nginx`
 
 ##### Pour configurer ou utilisé Ngnix, les commandes suivantes s'adaptent à tous les distributions de linux cité ci-dessus
 
 1. Vérifier l'état du serveur
   
    `systemctl status nginx`
    
 2. Démarrer ou arrêté le serveur Ngnix

    `sudo systemctl start nginx`
    
    `sudo systemctl stop nginx`
     
 3.  Configurer le démarrage automatique du serveur au lancement du système

     `sudo systemctl enable nginx`
     
     `sudo systemctl disable nginx`
     
 4.  Recharger les services

     `sudo systemctl reload nginx`
     
     `sudo systemctl restart nginx`
     
 5.  Tester Ngnix en tapant localhost sur votre navigateur Préféré 
