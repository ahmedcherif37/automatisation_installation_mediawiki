# automatisation_installation_mediawiki avec Ansible
création de 5 rôles 
1.	Le rôle apache :
 `* un fichier tasks/main.yml contient les actions pour installer Apache, un appel à un fichier de configuration pour installer PHP et une notification pour redémarrer Apache ; `
 `* un fichier handler/main.yml contient les actions pour redémarrer le service Apache. `
2.	Le rôle mariadb :
 `*	un fichier tasks/main.yml contient les actions pour installer MariaDB. `
3.	Le rôle commun de MediaWiki :
 `*	un fichier defaults/main.yml contient les variables d'installation qui seront utilisées dans les rôles suivants.`
4.	Le rôle confapache de MediaWiki :
 `*	un fichier meta/main.yml contient la dépendance avec le rôle commun ; `
 `*	un fichier tasks/main.yml contient les actions pour configurer Apache pour MediaWiki. `
5.	Le rôle confdb de MediaWiki :
 `*	un fichier meta/main.yml contient la dépendance avec le rôle commun ; `
 `*	un fichier tasks/main.yml contient les actions pour configurer MariaDB pour MediaWiki. `
