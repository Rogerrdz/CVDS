# CVDS - Laboratorio #01
# Integrantes:
 - Camilo Andres Fernandez Diaz
 - Roger Alexander Rodriguez Abril
# Respuestas:
 # Parte l
   1. Creamos una carpeta local el cual luego se va a convertir en nuestro repositorio local:


      Tambien creamos un directorio de apoyo en donde encontraremos las imagenes a usar en este laboratorio la cual llamaremos "asssets":

      

  2. Creamos un archivo tipo markdown para la Documentacion de este laboratorio este con el comando touch:


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

  a diferencia de otras version control system, el commit en Git no solo almacena las diferencias entre dos versiones sucesivas del contenido del directory, sino que guarda la instantánea (comprimida) del 
  contenido de todos los archivos que formaban parte del repository en el momento del commit.
  si un archivo no cambia de contenido entre dos commit, no se almacena una nueva versión comprimida, sino que se pone una referencia al commit anterior.
  cada commit conoce a su “padre” (parent commit), es decir, el commit inmediatamente anterior.
  El commit es la entidad básica en la que se basan los repository Git. 

  4. Enlazamos otro correo con la cuenta de github en github.com:

     Nos dirigimos al apartado de settings dentro de la cuenta:

     Luego a Emails alli encontramos  las cuentas de correo enlazadas a  la cuentas de github

     Alli añadimos una nueva cuenta de correo para mas tarde verificarla desde el mismo correo :

  5. Creamos un repositorio en blanco desde la pagina de git hub:

     añadimos el README.md y dejamos el repositorio como publico para que toda persona pueda ver:

     Ahora tenemos nuestro nuevo repositorio en blanco:

  6. Configuramos el repositorio local con el remoto :

     usamos :

     implementando tendriamos :
     
  7. Subimos los cambios con los comandos investigados en el incizo 3:

  8.Configuramos el correo electronico de manera local:

  9.Por Ultimo subimos cambios para confirmar que todo este bien con el repositorio:

  # Parte ll

  # Parte lll

  1. Hay una mejor forma de trabajar?

     

     

     

     
     
# Bibliografia
 -https://aulab.es/articulos-guias-avanzadas/70/el-comando-git-add-en-git
 
     
