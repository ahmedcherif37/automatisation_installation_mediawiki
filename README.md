# automatisation_installation_mediawiki avec Ansible
création de 5 rôles 
1.	Le rôle apache :
o	un fichier tasks/main.yml contient les actions pour installer Apache, un appel à un fichier de configuration pour installer PHP et une notification pour redémarrer Apache ;
o	un fichier handler/main.yml contient les actions pour redémarrer le service Apache.
2.	Le rôle mariadb :
o	un fichier tasks/main.yml contient les actions pour installer MariaDB.
3.	Le rôle commun de MediaWiki :
o	un fichier defaults/main.yml contient les variables d'installation qui seront utilisées dans les rôles suivants.
4.	Le rôle confapache de MediaWiki :
o	un fichier meta/main.yml contient la dépendance avec le rôle commun ;
o	un fichier tasks/main.yml contient les actions pour configurer Apache pour MediaWiki.
5.	Le rôle confdb de MediaWiki :
o	un fichier meta/main.yml contient la dépendance avec le rôle commun ;
o	un fichier tasks/main.yml contient les actions pour configurer MariaDB pour MediaWiki.
