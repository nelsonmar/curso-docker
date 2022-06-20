# Resolución

## HEALTHCHECK

La instrucción `HEALTHCHECK` sirve para chequear que el contenedor esté en un estado deseado luego de iniciar.

## ONBUILD

La instrucción `ONBUILD` se ejecutará eventualmente cuando la imagen sea utilizada como base para otra imagen. Acepta como argumento otra instrucción, que es la que se disparará finalmente en la imagen hija.

## VOLUME

La instrucción `VOLUME` define un directorio que se expone al host. Tal como la instrucción `EXPOSE` no modifica el comportamiento de la imagen en sí, solamente añade la metadata.

