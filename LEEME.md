### Inicia un servidor en la carpeta
Este proyecto utiliza un modelo de Tensorflow.js, el cual para cargarse requiere que el acceso sea por medio de http/https.
Para eso puedes usar cualquier servidor, pero aquí hay una forma de hacerlo:
- Descarga Python en tu computadora
- Abre una línea de comandos o terminal
- Navega hasta la carpeta donde descargaste el repositorio
- Ejecuta el comando `python -m http.server 8000`
- Abre un explorador y ve a http://localhost:8000

### Utilizarlo en un celular
Si quieres abrirlo en tu celular, no se puede solo poner la IP local de tu computadora y el puerto, ya que para usar la cámara se requiere HTTPS. Puedes hacer un túnel de HTTPS siguiendo los siguientes pasos
- Descarga ngrok en tu computadora, y descomprímelo
- Abre una línea de comandos o terminal
- Navega hasta la carpeta donde descargaste ngrok
- Ejecuta el comando `ngrok http 8000`
- Es importante tener ambos activos: El servidor de python, y el túnel de ngrok
- En la línea de comandos aparecerá un enlace HTTPS. Puedes entrar ahí con tu celular, no importa si no estás en la red local.
- El túnel expira después de 1 horas, en dado caso solo reinicias ngrok
- Abre un explorador en tu celular y ve al enlace HTTPS indicado

### Uso
Puedes dar clic en el botón de "Cambiar camara" para utilizar la cámara delantera o trasera del celular. Solo apunta la cámara a una imagen de compostage o a uno real, y abajo te aparecerá la predicción. Tampoco es el clasificador del futuro entonces si no clasifica perfecto, oops.