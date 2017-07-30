Actualizar o instalar Google Chrome
-----------------------------------

Primero se debe agregar (si no está ya añadido) el repositorio de Google Chrome
en nuestro sistema usando los comandos siguientes. Durante el uso de PPA en nuestro
sistema que también recibe las últimas actualizaciones cada vez que se comprueba si hay actualizaciones del sistema.

```bash
$ wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
$ sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'

```
### Instalar o actualizar Google Chrome
```bash
$ sudo apt-get update
$ sudo apt-get install google-chrome-stable
```
### Iniciar Google Chrome
```bash
$ google-chrome &
[or]
$ google-chrome-stable &
```
