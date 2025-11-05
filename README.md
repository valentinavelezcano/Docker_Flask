# Docker con Flask : pagina web - Caballos

PASOS
1. Creacion del codigo de manera local
* en visual estudio code crear la una carpeta que contendra todo lo necesario para el docker y el codigo de la pagina:
  * archivo: app.py
  * archivo: Dockerfile
  * archivo: requirements.txt
  * carpeta: templates (dentro de esta carpeta ira in archivo llamado index.html con el codigo que sera la pagina que queremos crear)
  * por fuera de la carpeta se crea un archivo llamado docker-compose.yml

2. se crea un repositorio en github, publico
3. se crea el repositorio local.    con los siguientes comandos para subirlo al repositorio de github}:
   * git init
   * git commit -m "first commit" (si ya tenemos la carpeta con todas las carpetas y codigo, se hace un (git add .) y se vuelve a poner este comando)
   * git branch -M main
   * git remote add origin (y se agrega la direccion donde esta el respositorio) https://github.com/valentinavelezcano/Docker_Flask
   * gti push -u origin main (esto lo sube al repositorio)

4. se crea la maquina en aws
   * se le adiciona un el puerto donde lo se va a mostrar la pagina
  
5. se abre en la terminal la maquina que se creo
   * dentro de la maquina se instala el docker
   * se clona el repositorio de la nube donde tenemos el codigo
   * se crea la imagen:
     * sudo docker-compose build (y en este caso no quiro que este en la cache) --no-cache
     * sudo docker-compose up (para ponerlo a correr)
    
6. teniendo ya esto listo, solo es poner la Ip publica de la maquina y el puerto por donde se va a mostrar (18.232.170.182:80)....
     
