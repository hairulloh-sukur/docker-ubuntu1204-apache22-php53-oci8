<img src="https://www.docker.com/sites/default/files/d8/2019-07/horizontal-logo-monochromatic-white.png" width=25% height=25%/> 

# docker-ubuntu1204-apache22-php53-oci8

This is a project for create docker image with environment specification: <br><br>
Ubuntu 12.04, <br>
PHP 5.3.10, <br>
Apache 2.2.22, <br>
oracle-instantclient 12.1.0.2.0-2, <br>
oci8-2.0.12 <br>

## Pull Image

Or You can also directly pull image from https://hub.docker.com/ 
by running below command in the Terminal:

```bash
  docker pull hairullohsukur/ubuntu1204-apache22-php53-oci8
```

## Create Container

#### to create a container on the linux OS:
```bash
  docker container create --name ubuntu1204-apache22-php53-oci8 -p 80:80 -v /documentroot:/var/www hairullohsukur/ubuntu1204-apache22-php53-oci8:latest
```

#### to create a container on the Windos OS:
```bash
  docker container create --name ubuntu1204-apache22-php53-oci8 -p 80:80 -v C:\documentroot:/var/www hairullohsukur/ubuntu1204-apache22-php53-oci8:latest
```

#### to change the port, you can replace it with:
ex: -p 8081:80

#### to change the local document root:

Linux:
ex: -v /mnt/data/htdocs:/var/www

Windows:
ex: -v D:\htdocs:/var/www
