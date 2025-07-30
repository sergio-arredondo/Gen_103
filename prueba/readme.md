#introducción de git y github
##comandos básicos

'ls': Lista todas las carpetas y archivos del directorio
'ls -a': Lista todas las carpetas y archivos incluyendo los ocultos
'cd': Navega al directorio principal
'cd ruta': Navega al directorio indicado
'cd..': Navega un directorio para atrás
'pwd': Muestra la ruta completa del directorio
'mkdir nombre_carpeta': Crea una carpeta nueva
'touch nombre_del_archivo': Crea un nuevo archivo

##Configurar Git por primera vez

1. Configurar su nombre de usuario

bash
git config --global user.name "Nombre_de_usuario_de_github"

2. Configurar su email de Github

bash
git config --global user.email "email_de_github"

Para verificar que todo este correcto:

bash
git config user.name

> [!NOTE]
> Este comando verifica y devuelve su nombre de usuario

bash
git config --list

> [!NOTE]
> Este comando verifica y devuelve una lista completa de sus datos

##Inicializar un repositorio con comando que tira github
bash

1. 'echo "# Gen_103" >> README.md' : Crea un archivo readme.md (opcional)

2. 'git init' : Inicializa un nuevo repositorio de git en el directorio actual (se usa una sola vez, obligatorio)

3. 'git add README.md' o 'git add .' Agrega el archivo readme.md o cualquier otro archivo que se indique al area de preparación.
   Con 'git add .' agregamos todos los archivos y carpetas del directorio

4. 'git commit -m "first commit"' (se va utilizar en mas de una ocación) Registra todos los cambios que se agregaron anteriormente al area de preparación con un
   comentario específico, haciendo referencia el cambio hecho. En este caso "first commit"

5. 'git branch -M main' se usa una sola vez obligatorio

-Crea y cambia a la rama "main", que será la rama principal

6. 'git remote add origin https://github.com/sergio-arredondo/Gen_103.git'

- Enlaza su repositorio local con el repositorio remoto de GitHub

7. 'git push -u origin main' (se usa en más de una ocasión sin el -u)

sube todos los cambios subidos y comentados al repositorio

##Inicializar un repositorio con comandos propios

> [!caution] >**Se usa una sola vez de manera obligatoria**

1. Inicializamos el repositorio
   bash

git init

2. Creamos y cambiamos a la rama "main"

git branch -M main

3. Enlazamos nuestro repositorio local con el remoto

git remote add origin https://github.com/sergio-arredondo/Gen_103.git

##Comandos a realizar cada vez que hay un cambio a subir

> [!Important]
> **se usan en mas de una ocasión**

1. Subimos los cambios al area de preparación

git add .

2. comentamos / registramos los cambios subidos al área de preparación

git commit -m "comentario relacionado"

3. Subimos todos los cambios al repositorio remoto

git push origin main

##Otros cambios útiles de git

-ver en que estado está el repositorio

git status

-ver el historial de commits

git log

-Clonar un repositorio

git clone https://github.com/abigail-salas/Gen_103.git
