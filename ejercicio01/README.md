# Resolución

Ejecutar el siguiente comando:

```bash
docker run --rm -v "$(pwd)":/usr/share/nginx/html/ -p 8000:80 nginx:1.22.0-alpine
```

Y luego acceder a http://localhost:8000/
