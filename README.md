# UNMAINTAINED, but...

__This branch won't be updated anymore : I did switch to [Ansible Galaxy](https://galaxy.ansible.com/intro) and use the [galaxy](//github.com/loranger/ansible-playbooks/tree/galaxy) branch instead. Maybe you should too?__

The main goal of this switch is to being able to provision any docker from a simple playbook whereas cloning first this repository was a mandatory before.

Of course, galaxy is also able to provision a local machine, a remote server, a vagrant or any virtual machine; as usual.


In order to use galaxy properly, I had to create a repository for each existing role.

I didn't want to flood my github profile so I created an [organization](//github.com/cowops/) you can join.

Just ping me ;)


Ansible playbooks
=================

Usual and casual tasks for development debian server settings using ansible.

Roles
-----

This playbook install the following [1] :

#### System
  - [Basic packages and upgrade](roles/common) system
  - [Network Time Protocl](roles/ntp)
  - [Git distributed version control](roles/git) system
  - [Python](roles/python) programming language
  - [Go](roles/go) programming language
  - [rmate](roles/rmate) tool
  - [Ferm](roles/ferm) tool
  - [ZSH](roles/zsh) shell
  - [Prezto](roles/prezto) zsh enhancement
  - [Supervisor](roles/supervisor) daemon

#### Monitoring
  - [Collectd](roles/collectd) tool
  - [Scout Realtime](roles/scout_realtime) tool
  - [Packetbeat](roles/packetbeat) tool

#### PHP
  - [PHP Fast Process Manager](roles/php-fpm) or [PHP Apache module](roles/php-apache) or [HipHop Virtual Machine](roles/php-hhvm)
  - [PHP useful extensions](roles/php-extensions)
  - [PHP Maxmind](roles/php-maxmind-geoip) extension
  - [PHP New Relic](roles/php-newrelic) extension
  - [PHP Phalcon](roles/php-phalcon) extension
  - [PHP 0MQ](roles/php-zmq) extension
  - [PHP XDebug](roles/php-xdebug) extension
  - [Composer](roles/composer) tool

#### Web server
  - [Apache](roles/apache) server or [Nginx](roles/nginx) server
    * Note: If you need to configure nginx sites, read [this short instruction](roles/nginx)

#### Database
  - [MySQL](roles/mysql) server
  - [MariaDB](roles/mariadb) server
  - [Cassandra](roles/cassandra) server
  - [MongoDB](roles/mongodb)
  - [InfluxDB](roles/influxdb) server
  
#### Queue messaging
  - [0MQ](roles/zeromq) server
  - [Beanstalkd](roles/beanstalkd) server

#### Cache
  - [Memcached](roles/memcached) server
  - [Redis](roles/redis) server
  
#### Image
  - [ImageMagick](roles/imagemagick) tool
  - [GraphicsMagick](roles/graphicsmagick) tool
  - [FaceDetect](roles/facedetect) tool

#### Search
  - [Elasticsearch](roles/elasticsearch) server
  - [Sphinx](roles/sphinxsearch) server

#### Misc
  - [HAProxy](roles/haproxy) load balancer
  - [Bind](roles/bind) server
  - [Java](roles/java)
  - [Kibana](roles/kibana) tool
  - [Postfix](roles/postfix) server
  - [PredictionIO](roles/predictionio) server
  - [Sharedance](roles/sharedance) server



[1] In fact, it MAY : You have to comment some playbook lines in order to bypass the unrequested roles.
