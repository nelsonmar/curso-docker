# Resolución

#### ¿Cuántos contenedores se están ejecutando?

Se están ejecutando dos contenedores: la aplicación web y la base de datos.

Puede observarse en dentro del archivo `docker-compose-jobvacancy.yml`, son los dos items dentro del diccionario `services`.

#### ¿Cuales son las imágenes en las que están basados los mencionados contenedores?

La aplicación web está basada en la imagen `nicopaez/jobvacancy-ruby:1.3.0` y la bbdd está basada en la imagen `postgres`.

Se puede observar en el campo `image` de cada servicio.

#### ¿Puedes leer el docker-compose-jobvacancy.yml y describir lo que hace cada una de sus lineas?

- `version` indica la versión de Docker Compose a utilizar.
- `services` indica los servicios incluidos en el archivo docker-compose, que se iniciarán al ejecutar `docker-compose up`.
- `web` y `db` son los nombres de los dos servicios.
- `image`: es la imagen que se utilizará para iniciar el contenedor.
- `ports` son los puertos que se mapean al host para poder acceder al contenedor.
- `environment`: son las variables de entorno que se le definen al contenedor que va a iniciar.
- `depends_on`: es la precedencia que tienen los contenedores al momento de iniciar. Si un contenedor depende de otro, Docker Compose espera a que uno inicie para levantar el otro.

#### ¿Cómo es posible que esos contenedores se vean entre sí?

Por defecto Docker Compose crea, de manera implícita, una red de Docker propia donde incluye a todos contenedores definidos en el docker-compse.

Por eso no es necesario definir explícitamente que los contenedores deben iniciar en la mismar red.
