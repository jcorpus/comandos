Comandos básicos Linux
-----------------------
##### Actualizar ubuntu
`sudo do-release-upgrade -d`

##### mkdir (crea un directorio)
```bash
$ mkdir micarpeta
```
##### rm (borra un archivo o directorio)
```bash
$ rm miarchivo.txt
```
`rm -r descargas`
##### 


##### wc (Cuenta las lineas, palabras y caracteres que contiene un archivo)
```bash
$ wc archivo.txt
```

##### tail (Muestra las últimas lineas de un archivo, por defecto las últimas 10)
```bash
$ tail archivo.txt
```

##### more (muestra el contenido de un documento)
```bash
$ more archivo.txt
```

##### ls -lh (lista lo que hay en un directorio con información legible para el humano xd)

```bash
$ ls -lh
```
-Alguas banderas para ls

`ls -l`: lista los archivos con datos de cada nodo, ordenados alfabéticamente

`ls -lS`: lista los contenidos ordenados por tamaño

`ls -lh`: lista los contenidos mostrando los datos legibles fácilmente (tamaño)

`ls -r`: lista los archivos ordenados de forma inversa (sirve con las banderas S y t)

`ls -a`: lista los contenidos de un directorio incluyendo los archivos ocultos

##### chmod cambiar permisos
`$ chmod +x` + para agregar permiso y x para permiso de ejecución
`$ chmod -x` quitamos el permiso de ejecución

##### ps procesos activos de un programa
`$ ps aux`
`$ ps aux | grep postgres` muestra procesos de postgres
`$ kill #de proceso` elimina el proceso

#### tar/zip comprimir y descomprimir archivos
`$ tar czvf nombrefichero.gz nombre de directorio a comprimir` c = comprimido
`$ tar xzvf nombrefichero` x= descomprimir 
`$ zip -r nombre.zip lib archivo`
`$ unzip nombrearchivo.zip` 

##### pw (Donde nos encontramos)
```bash
$ pwd
```

##### mv (mover archivos en el directorio)
```bash
$ mv micarpeta ../
```

##### cp (copiar archivos)
```bash
$ cp origen ./destino
```
copiar directorios `cp -r`

##### cat (parecido al more)
```bash
$ cat archivo.txt
```

##### touch (tocar archivos)
```bash
$ touch nuevoarchivo
```

##### nano (editor de texto en la terminal)
```bash
$ nano archivo.php
```

##### man (manual de los comandos)
```bash
$ man ls
```

##### bc (calculadora en la terminal)
```bash
$ bc
```
##### top (Muestra los procesos en Linux)
```bash
$ top
```
##### kill (matar un proceso por el ID del proceso PID)
```bash
$ kill -9 id del proceso
```
##### grep (buscar dentro de archivos)
```bash
$ grep palabra miarchivo
```
##### grep (otra forma de buscar seria combinando comados)
```bash
$ cat archivo.py |grep palabra 
```
##### grep (con la bandera -n nos dice en que linea se encuentra)
```bash
$ grep palabra archivo.php -n
```
##### Descargar archivos
`wget https://www.ejemplos.com/video.mp4` 


cURL peticiones GET, POST
-------------------------
##### curl (peticiones HTTP/S)
```bash
$ curl https://jcorpus.github.io
```
**copiar contenido de una pagina en un archivo**
```bash
$ curl -o contenido.html https://jcorpus.github.io
```
##### curl (descargar archivo original con curl -O)
```bash
$ curl -O https://i.makeagif.com/media/2-07-2017/XJtC1y.gif
```
##### curl (peticiones get)
```bash
$ curl "https://httpbin.org/get?variable=hola"
```
**otro ejemplo de envio de datos por get**
```bash
$ curl --data "nombre=julio&apellido=corpus" http://httpbin.org/post
```

