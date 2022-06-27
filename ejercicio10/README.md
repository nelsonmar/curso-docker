# Resolución

1. Crear el bot en Telegram

2. Crear el archivo `deployment.yml` y configurar el token obtenido del BotFather como variable de entorno `TELEGRAM_TOKEN`

3. Aplicar los cambios con `kubectl apply -f deployment.yml`

4. Ir al chat del boy en Telegram y enviarle un mensaje: `/version`
