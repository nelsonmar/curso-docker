# Resolución

1. Descargar la imagen y ejecutarla

```
docker run nicopaez/pingapp:3.0.0
```

2. Pausar el contanedor (CTRL + C en la terminal)

3. Guardar el contenido del contenedor en una nueva imagen. Para eso se debe indentificar el id de contenedor:

```
docker ps -a
docker container commit <container_id> nelsonmartinez/pingapp:0.0.1
```

4. Subir la imagen al nuevo repositorio

```
docker login -u nelsonmartinez --password-stdin
docker push nelsonmartinez/pingapp:0.0.1
```

## Para descargar la imagen

```
docker pull nelsonmartinez/pingapp:0.0.1
```
