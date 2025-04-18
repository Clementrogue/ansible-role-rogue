# ansible-role-rogue

# ansible-role-rogue (WordPress Deployment Role)

## Description

Ce rôle Ansible permet de déployer automatiquement un site WordPress avec Apache, PHP et MariaDB.  
Compatible avec les distributions basées sur **Debian (Ubuntu)** et **RedHat (Rocky Linux, CentOS)**.

---

## Fonctionnalités

- Installation d'Apache, PHP, MariaDB, wget, unzip
- Téléchargement et configuration de WordPress
- Création de la base de données WordPress et de l'utilisateur associé
- Configuration du VirtualHost Apache
- Prise en charge de `systemd` et des environnements Docker

---

## Variables par défaut

Fichier : `roles/wordpress/defaults/main.yml`

```yaml
wordpress_db_name: wordpress
wordpress_db_user: example
wordpress_db_password: examplePW
mysql_root_password: examplerootPW
wordpress_url: https://wordpress.org/latest.zip
```

## Structure du projet
```
roles/
└── wordpress/
    ├── defaults/
    ├── handlers/
    ├── meta/
    ├── tasks/
    ├── templates/
    ├── tests/
    └── vars/
```
