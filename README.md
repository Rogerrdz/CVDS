# CVDS - Laboratorio #01
# Integrantes:
 - Camilo Andres Fernandez Diaz
 - Roger Alexander Rodriguez Abril

 # Parte l
   1. Creamos una carpeta local el cual luego se va a convertir en nuestro repositorio local:

      ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/Crear_Carpeta_.png) 


      Tambien creamos un directorio de apoyo en donde encontraremos las imagenes a usar en este laboratorio la cual llamaremos "asssets":

      ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/assets.png) 

  2. Creamos un archivo tipo markdown para la Documentacion de este laboratorio este con el comando touch:

     ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/readme_.png) 

  3. Investigamos para que sirven los comandos "git add" y "git commit -m "mensaje" " :

  # git add

  El comando git add añade una modificación presente en la working directory al staging area. Es la forma de decirle a Git qué cambios particulares se realizarán en la próxima confirmación.

  Opciones comunes:
    
  - git add <file> - añade todos los cambios a un archivo al staging area
  - git add <file> - añade todos los cambios a una directory al staging area
  - git add -p - inicia una sesión interactiva que permite elegir que parte de los archivos modificados se agregan al staging area
  
  El modo interactivo es especialmente útil si has realizado varios cambios conceptualmente no relacionados y solo una fracción de ellos se incluye en el commit. Este modo muestra el fragmento de            cambios (chunk) y solicita que se realice la acción presionando una letra ("y" para agregar el chunk, "n" para ignorarlo, "s" para dividir aún más el fragmento, "q" para salir).
    
  P.D. Un buen flujo de trabajo espera que cada commit contenga todos y solo los cambios que hacen un cambio particular en el código base, ejemplo: agregando una feature.

  # git commit -m "mensaje"

  Un commit in Git representa un snapshot (instantánea) del repository en un momento específico. Aunque esta definición puede parecer banal, vale la pena subrayar que:

  a diferencia de otras version control system, el commit en Git no solo almacena las diferencias entre dos versiones sucesivas del contenido del directory, sino que guarda la instantánea (comprimida) 
  del 
  contenido de todos los archivos que formaban parte del repository en el momento del commit.
  si un archivo no cambia de contenido entre dos commit, no se almacena una nueva versión comprimida, sino que se pone una referencia al commit anterior.
  cada commit conoce a su “padre” (parent commit), es decir, el commit inmediatamente anterior.
  El commit es la entidad básica en la que se basan los repository Git. 

  ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/git_add_y_git_commit.png) 

  4. Enlazamos otro correo con la cuenta de github en github.com:

     ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/emails.png)

     Alli añadimos una nueva cuenta de correo para mas tarde verificarla desde el mismo correo 

  5. Creamos un repositorio en blanco desde la pagina de git hub:

     ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/create_github.png) 

     añadimos el README.md y dejamos el repositorio como publico para que toda persona pueda ver:
     
     ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/new_repository.png) 

     Ahora tenemos nuestro nuevo repositorio en blanco:

     ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/new_repository_1.png) 

  6. Configuramos el repositorio local con el remoto :

     ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/new_repository_1.png) 
    
     usamos :
     
     ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/confirmar_id_local.png)
   
     implementando tendriamos :

     ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/final.png)
     
  7. Subimos los cambios con los comandos investigados en el incizo 3:

  ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/add.png)

  8.Configuramos el correo electronico de manera local:

  ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/correo.8.png)

  9.Por Ultimo subimos cambios para confirmar que todo este bien con el repositorio:
  
  ![image](https://github.com/Rogerrdz/CVDS/tree/main/assets/punto.9.png)

# Parte II

1. Se escojieron los roles 
    - Owner : Camilo Fernandez
    - Colaborador : Roger Rodriguez

2. El owner agregara al colaborador, para realizar este paso lo primero que se debe hacer es buscar en el repositorio de github el apartado de ajustes, una vez dentro buscaremos colaboradores y dentro de este apartado ingresaremos el correo del colaborador o colaboradores que se quieran agregar al proyecto en este caso sera Roger y a el le llegara un correo para poder participar dentro del repositorio y ua vez aceptado se vera tal que asi:
![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/Colaboradores.PNG)
- El colaborador le llega la invitacion:
![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/Invitacion.png)
- El colaborador acepta la invitacion:
![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/SuccessInvitation.png)

3. Ahora el owner y el colaborador modificaran el README y se subira al mismo tiempo, al momento de hacer esto el primero que detecte que lo haya subido se subira normalmente los cambios pero al otro le generara un error como se vera acontinuación:

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/Error.png)  

4. Para resolver estos tipos de problemas primero la persona que le solto el error abrira el IDLE de su preferencia o IntelliJ en este caso se uso Visual Studio Code, usamos start README.md ya que este es el archivo que nos genera el conflicto o simplemente buscamos desde consola nuestra carpeta donde tenemos guardado el proyecto y lo abrimos y quedaria de tal manera:

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/ErrorVisual.png) 

Como se podra ver al abrir el archivo se veran las modificaciones hechas por los 2 y el conflicto que hay, para solucionar este problema podemos borrar la parte que no nos interese ya sea del owner o del colaborador, o tambien podemos mezclar dichas partes. En este caso uniremos las partes pero antes de ello debemos borrar estos caracteres para que funcione <<< === y >>> ya que esto señala los archivos que entran en conflicto al hacer pull y quedaria de esta manera:

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/CorreccionErrores.png)

Una vez hecho los cambios el IDLE nos mostrara que cambiamos, que borramos o que hicimos para corregir los errores dentro del codigo, como se podra ver en el ejemplo mostrara la version del owner y del colaborador y abajo como se corregio el error que en este caso fue fusionando los 2 cambios hechos por cada uno:

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/MuestraCambios.png)

5. Una vez hecho los cambios y corrigiendo los errores le daremos a git status para ver el estado del archivo que entraba en onflicto y se vera de esta manera:

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/Archivomodif.png)

Ya para finalizar subiremos este nuevo archivo con las modificaciones de manera normal, usando add, commit y pull o push para subirlo al repositorio y antes de darle en este ultimo comando le daremos a git status una vez mas para asegurar que no hayan errores y que si haya funcionado el comando add:

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/ArchivoListo.png)

Y ya con esto solucionamos el problema y podremos trabajar normalmente en el repositorio creado.

# Parte III
1. Cada uno crea una rama esto para facilitar las modificaciones de cada uno de los usuarios y luego unir las versiones o poder ver los errores si es necesario y corregirlos y esto se vera de tal manera:

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/crear_rama.png)

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/Branch.PNG)

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/feature_camilo.png)

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/feature_roger.png)


2. Cada persona hace cambios y realiza el pull request a la rama main/master para que con cada modificacion hecha se pueda subir al repositorio correctamente

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/pull.png)

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/pull2.png)

3. Se eliminan las ramas como se pide en el laboratorio esto para facilitar y dejar una rama en concreto:

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/borrar_r1.png)

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/borrar_r2.png)

Ahora veremos como se debe ver una aprobacion de un pull request hecho por un usuario y como al aceptar esta afecta el repositorio y rama principal y se guardan los cambios despues de la confirmacion del usuario 

![image](https://github.com/CamiloFdez/Cvds_lab1/blob/master/assets/apr_2.png)


# Respuestas
- Parte I: 
    * ¿Para qué sirve y como se usan estos comandos git add y git commit -m “mensaje”?
        - Git add: Este comando de git sirve para mover los cambios que se realizaron en el directorio del trabajo al área del entorno de ensayo, tambien al utilizar este comando se puede empezar a rastrear archivos nuevos, preparar archivos, y hacer otras cosas como marcar archivos en conflicto por combinación.
        - Git commit -m "mensaje": Este comando confirma la instantánea preparada en el historial del proyecto, es decir, una vez al usar el anterior comando y añadir todos los archivos que se quieran añadir al repositorio este comando permite confirmar los cambios y adicional a esto añadir un mensaje de que se hizo para asi servir de guía del paso a paso o de lo que se este haciendo y subiendo mediante el proceso.   
- Parte II:
    * ¿Que sucedió al momento de que los dos editaran el README.md al mismo tiempo?
        - Al momento de modificar los dos poniendo cualquier cosa en el README y intentar subir los cambios al mismo tiempo a uno le subira correctamente los cambios al repositorio, pero al otro no le subira y sucedera un error en ese caso debido a que como guardo los datos del repositorio del primero que lo subio, este no tiene dichos cambios y generara asi un error de actualizacion al momento de subirlo, una solucion como se vera en el apartado de la parte 2 es hacer un merge o abrir IntelliJ, Visual Studio Code o el de su preferencia para corregir, eliminar o unir estos cambios propuestos por los 2 usuarios y asi arreglar el error.
- Parte III:
    * ¿Hay una mejor forma de trabajar con git para no tener conflictos? 
        - Si, hay mejores formas para trabajar y no tener conflictos, una de ellas pueden ser las ramas que estas sirven cuando los usuarios estan interactuando con varios archivos pues crean estas ramas para que las modificaciones que cada uno hace queden dentro del repositorio y ya cuando se terminen todos los cambios el usuario hace un Pull Request para que dichos cambios sean aceptados al final o cuando terminen cada cambio realizado para subirlo al repositorio.
    * ¿Qué es y como funciona el Pull Request?
        - Un pull request es una peticion que un usuario le hace al otro para que este último incorpore los commits que están en el repositorio, al crear estas ramas tambien ayudan para fusionar los cambios hechos por los usuarios despues de utilizar este comando, permitiendo asi que os demas revisen dichos cambios y puedan determinar si aprueban o no dichos cambios para solicionar conflictos y errores.
     

     

     

     
     
# Bibliografia
 -https://aulab.es/articulos-guias-avanzadas/70/el-comando-git-add-en-git
 
     
