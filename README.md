[![GitHub license](https://img.shields.io/badge/license-Apache-green.svg)](http://git.kaido.ovh/Kido/Deskofus/raw/master/license)


### Instalación

```bash
git clone https://github.com/soanix/webserver-docker.git webserver
cd webserver
# Editamos los datos del archivo .env
# Luego ejecutamos
docker-compose up -d

```

Si todo va bien, deberíamos poder acceder a http://localhost desde nuestra máquina o a la ip publica del servidor donde este alojado docker.

---

### Crear virualhost (Servidor virtual)

```bash
cd web
mkdir domain.tld
```

### Componentes

- apache2
 - libapache2-mod-php7.4  
- curl  
- php7.4
  - php-mysql  
  - php-intl
  - php-imagick
  - php-mbstring
  - php-dev  
  - php-curl  
  - php-intl  
  - php-json
  - php-simplexml
  - php-xml
  - php-dev
  - php-pear
- nginx
- MariaDB
- Mysql
- Redis
- Postfix
- proftpd
- letsEncrypt / certbot
- Portainer
