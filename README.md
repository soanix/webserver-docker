[![GitHub license](https://img.shields.io/badge/license-Apache-green.svg)](http://git.kaido.ovh/Kido/Deskofus/raw/master/license)


### Instalación

```bash
git clone https://github.com/soanix/webserver-docker.git webserver
cd webserver
# Editamos los datos del archivo .env
# Luego ejecutamos
docker-compose build
docker-compose up -d

```

Si todo va bien, deberíamos poder acceder a http://localhost desde nuestra máquina o a la ip publica del servidor donde este alojado docker.
En caso contrario, verificar si nginx da algun error

docker logs nginx --tail 100 -f

* Si es un problema de certificados borrar el bloque de ssl de etc/nginx/conf.d/default.template y recargar nginx docker exec -it nginx nginx -s reload

---

### Crear virualhost (Servidor virtual)

```bash
mkdir web/domain.tld
```

### Componentes

- Apache2
  - PHP 8.0 (Image: apache80)
  - PHP 7.4 (Image: apache74)
  - PHP 7.3 (Image: apache73)
  - PHP 7.2 (Image: apache72)
  - PHP 7.1 (Image: apache71)
- Nginx
- MariaDB
- Mysql
- Redis
- Postfix
- proftpd
- letsEncrypt / certbot
- Portainer
