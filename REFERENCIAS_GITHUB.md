# REFERENCIAS GITHUB  

Acá encontrarás algunas referencias que te ayudarán con algu temas de Github. 

<br> 

## A- Cómo ir a su carpeta–repositorio local con línea de Comandos. 

Esto es para navegar con la línea de comandos, hasta y llegar a la carpeta donde tenemos el repositorio donde queremos trabajar. 

1–Abrir su consola (Terminal en Mac, CMD en Windows), dependiendo de sus sistema operativo. Algunos en Windows pueden tener la opción de Git Bash, abran esa. 

2–Ir a la carpeta del repositorio donde quieren trabajar, colocar "cd", y arrastrar la carpeta donde tienen el respositorio que les interesa trabajar. Si enla consola les aparece "cd" y la ruta a su carpeta, y dan enter, algo así:  
cd ruta/de/mi/carpeta/

3–Confirmar con pwd (Mac) o dir (Windows) si están en la carpeta de su repositorio. Si estan allí, ir al siguiente paso que les ionterese. Si no están, ir al paso anterior, hasta llegar a su carpeta. Para confirmar donde están, en su consola colocar lo siguiente, y dan enter:  
pwd o dir (debe mostrarles la ruta de la carpeta donde estan). 


<br> 
## B– Clonar repositorio.  

Si han creado un repositorio nuevo en github (online), y desean tener copia local, deben primero clonarlo en otra carpeta (no la misma donde tienen el repositorio del curso). 

1- Del punto "A- Cómo ir a su carpeta–repositorio localcon línea de Comandos." hacer los pasos 1 al 3.

2- Ir al reposotorio de Github que quieren clonar. Desde "Clone using the web URL" copiar la dirección web que aparece. 

3- En su terminal, ya estando en la carpeta nueva donde desean clonar el repositorio, colocar en Terminal "git clone ylaurlcopiadadesdegithub", y enter

4- Si todo esta ok, esto debería clonar el repositorio de github en su nueva carpeta local. verificar si la carpeta local tiene los contenidos nuevos. 

5- Ahora pueden editar el HTML local, y guardar. Para subir cambios, ver "D– Subir cambios locales a guthub con git push".  


<br>
## C- Cómo bajar el material desde el repositorio PCOMP_2024B  

Para bajar el material dsesde un repositorio de github, deben usar el comando git pull, en su consola (Terminal en Mac, CMD en Windows), estando en la carpeta del repositorio que crearon. Entonces recuerden:  

1- Del punto "A- Cómo ir a su carpeta–repositorio localcon línea de Comandos." hacer los pasos 1 al 3.

2– Estando en su carpeta deben "tirar" (pull) los cambios del repositorio, hacia a su computador local. Así podrán "descargar" las cosas que se vayan subiendo al repositorio del curso.  En su consola colocar, y dan enter:  
git pull

Y recuerden sino lo pueden hacer ahora, lo vemos con calma en la clase.  


<br> 
## D– Subir cambios locales a guthub con git push" 

Para subir cambios que haya realizado en su computador local, debe estar en su carpeta local del repositorio que quiere subir. Luego agregar el contenido nuevo, hacer un commit con mensaje y luego el push. OJO, ser MUY ordenados con las carpetas, y tener cuidado con los pesos de los archivos. 

1- Del punto "A- Cómo ir a su carpeta–repositorio localcon línea de Comandos." hacer los pasos 1 al 3.

2- Estando en su carpeta, verificar cambios locales. Colocar y luego enter: 
git status

3- Para subir, primero hay que agregar los cambios al "stage", pueden ser archivo a archivo, o todo. Por ahora subiremos todo, colocar y luego enter (ojo, va un punto que indica "subir todo"):  
git add . 

4- Una vez todo agregado al "stage", hay q e agregar un mensaje para indentificar los cambios. Primero se agrega -m y luego el mensaje entre comillas 
git commit -m "Subiento los cambios X, Y, Z."

3– Para subir material deben "empujar" (push) los cambios locales al repositorio online. Así podrán "subir" las cosas que se vayan cambiando al repositorio online. origin main" indica que es en el repositrio y rama principales. En su consola colocar, y dan enter:  
git push origin main   


<br>  
## E- Crear repositorio online para Github pages. 

Estos pasos permiten crear un repositorio online que se pueda ser visto en una web. Inicializaremos el reposotirio online, luego lo clonamos local, trabajamos allí, y luego se suben los cambios con push. Ojo que a veces los cambios se demoran un poco en aparecer.  

**1- CREAR repositorio**. 

– Ir a su cuenta github.  
– Crear nuevo reposotirio: "+", "New repository".   
– El nombre del repositorio debe tener esta estructura: PCOMP24B_p02_apellido_titulo.   
– En descripción colocar PCOMP 2024B, P02, Titulo_del_Proyecto, Integrantes (orden alfabético porfa): Apellido Nombre, Apellido Nombre, Apellido Nombre...  
– Public: debe ser público.   
– Add README file. Poner que agregue un archivo Readme (es en Markdown). Sirve como registro general de lo que trata el repositorio.   
– "Crear repositorio". Esto lleva al repositorio creado.   

**2- CREAR ARCHIVO HTML (Después localmente lo podemos modificar)**   

– En el repositorio, crear un archivo HTML: "Add file / Creare new file".  
– Luego del nombre del repositorio, colocar el nombre del archivo, debe ser este: index.html  
– En el cuerpo colocar un texto html cuaquiera, por ejemplo (con los braquets): 
`
<h1>Este es un titulo de github pages. </h1>
`  
– "Commit Changes"   

**3- SETTINGS DE GITHUB PAGES**  
– Ir a "Settings" (arriba derecha).  
– Ir a "Pages" (abajo izquierda).  
– En Source seleccinar "Deploy from a branch" 
– En Branch, seleccionar "Main"   
– Hacer "Save"  
– Listo! pero hay q esperar un poco, se demora en hacer "deploy"   
– La url es: https://nombredesucuenta.github.io/elrepositorioweb/  

Pueden ver estos pasos acá:  
– Programación Accesible: https://www.youtube.com/watch?v=8IdBAysf-U4   


<br>  
## F- Authentication Token    

El soporte para autenticación terminó el 2021 ("Support for password authentication was removed on August 13, 2021") lo que implica que a veces hay que sacar un "token" (un código) de autenticación, a continuación algunos de los pasos para obtenerlo.  


1- Ir a User / Settings (abajo) Developer Settings / Personal access token / Tokens (classic)
2- Generate New Token / Tokens (classic)
3- Poner nombre descriptivo corto. No expiration date. Seleccionar todas la cajitas. 
4- Guardar token con la vida. No se ve otra vez. No prestar y no mostrar a nadie, es una clave secreta unica. 

Ahora hacer el push origin main
colocar user
pegat token
	
Más info acá:  
-Simple: Support for password authentication was removed on August 13, 2021 
https://youtu.be/dNy7GTah9IU?si=7EPbouoZoAZ_Fmgr

Video:  
-  How To Fix Support For Password Authentication Was Removed On GitHub   
https://www.youtube.com/watch?v=ePCBuIQJAUc


-Opción setear origen.
-Ahora setear el origen:  
-copiar nombre del usuario y repositorio de la url: https://github.com/ricardovv/PCOMP_2024B
https://github.com/usuario/repo
git remote set-url origin new.git.url/here




<br><br>
## Otros comandos útiles: 
Recuerden que deben estar en su carpeta del repositorio para que funcionen.  
**git status**:  Les dice si hay cambios que se hayan realizado en sus archivos locales.  
**pwd** (en Mac) dir (en Windows): Siempre es bueno confirmar en que carpeta nos encontramos.  
**git --version**:  Para ver la versión de git que tenemos.


Les dejo este link si queren saber algo más:  
**Git pull explicado** 
https://www.freecodecamp.org/espanol/news/git-pull-explicado/


**No dar seguimiento a un archivo**. 
Esto para que no aparezca en el github (online) pero si puede estar en el local. Hacer lo siguiente en el repositorio local y luego subir (git push origin main): 
- Colocar el nombre de archivo en el archivo .gitignore
- Subir el archivo al repositorio de git hub (git add, git commit, got push orogon main...)
– remover del repo online (github) con: git rm --cached nombredearchivo.xxx
- hacer un git commit: git commit -m "removeiendo nombredearchivo.xxx"
- subir el cambio con git push origin main
- ir al repo de github y confirmar el cambio. 

**Cambiar nombre de archivo**
Para cambiar nombre de archoivo desde git local.
git mv old_file_name.txt new_file_name.txt
