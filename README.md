# Linux server

this is my last project in `full stack web developer nanodegree`.

this project configure a linux server to run the `item catalog website`.

* ip address: `130.211.168.53 `
* ssh port: `2200`
* complete URL: `http://item-catalog-udaciy.tk/`


## software installed:

* finger
* apache2
* libapache2-mod-wsgi git
* libpq-dev
* python-dev
* postgresql
* postgresql-contrib
* python-pip
* Flask
* httplib2
* oauth2client
* sqlalchemy
* psycopg2
* sqlalchemy_utils

## configuration changes:

1. create new user `grader`
2. give sudo acces to grader
3. create public and private keys for my user and the grader user
4. change ssh port to 2200
5. Enforce key-based authentication
6. disable login for root
7. change tiem zone to utc
8. configure the firewall(ufw):
    * deny incoming
    * allow outgoing
    * allow 2200/tcp
    * allow www
    * allow ntp
    * then enable the ufw
9. install the applications listed above
10. configure apache server
11. configure postgresql database:
    * create new user named catalog
    * create a new database named catalog
    * give the privileges to only the new user
12. clone my `item catalog project` to /var/www/catalog
13. configure the project to work with apache and postgresql
14. update and upgrade the system


## third-party resources used:

* `google OAuth2` to provide login system in my website.
