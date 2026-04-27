Readme
#Trabajo individual

Mauricio Alail Cano Gutierrez

##Clase 1
###¿Que es GIT?

Es un sistema de codigo abierto el cual sirve para guardar archivos el gual sirve para desarrolladores trabajar grupalmente

###¿Como nacio git?

Fue creado por Linus Torvalds debido a la necesidad de un sistema tras salir de Bykeeper

###¿Como instalar GIT?

En la terminal con el comando:sudo apt-get install git

###Configuraciones basicas

Git config --global user.name "name"
git config --global user.email

Recien hice por que con windows no me dejo editar con nano y de ahi instale debian y trabajo de 8am a 6pm xdxd no tengo tiempo xdxd

##CLASE 2

###LOS ESTADOS DEL GIT

Directorio de Trabajo (Modificado): Es tu carpeta local donde editas los archivos. Los cambios están ahí, pero Git aún no los ha registrado formalmente.

Stage Area (Preparado): Es el área de espera. Aquí seleccionas qué cambios específicos quieres incluir en tu próxima "foto" o versión del proyecto.

Repositorio Local (Confirmado): Los cambios se guardan permanentemente en la base de datos de Git. Cada conjunto de cambios recibe un ID único (hash) y ya forma parte del historial oficial.

###DIRECTORIO DE TRABAJO(MODIFICADO)

Untracked (Sin seguimiento): Archivos nuevos que Git detecta pero que nunca han sido guardados en el historial.

Modified (Modificado): Archivos que ya existían en el historial, pero que has editado, borrado o renombrado.

Cualquier archivo que no esté explícitamente excluido en el .gitignore entrará automáticamente en uno de estos dos estados en cuanto realices un cambio.

### DIRECTORIO DE TRABAJO (MODIFICADO)

QUE PASE A SU ESTADO ORIGINAL "git restore <ARCHIVO>" borra lo que se escribio

PARA QUE EL ARCHIVO CREADO NO LO VEA GIT ES "nombre_del_archivo .gitignore

### STAGE AREA (PREPARADO)

Es el espacio donde seleccionas qué archivos modificados quieres incluir en tu próximo guardado (commit) y cuáles prefieres dejar fuera por ahora.

git add <archivo>: Agrega un archivo específico.

git add .: Agrega todos los archivos modificados o nuevos de una sola vez.

###REPOSITORIO LOCAL (CONFIRMADO)

Es donde al repositorio se cree un punto de guardado para que todos los cambios esten en el staged esten en el historial

      git commit -m "mensaje"
si se quiere deshacer el ultimo commit el comando es;
      git reset --soft HEAD~1
###BUENAS PRACTICAS

Cada commit debe representar un único cambio lógico, que sea pequeño y esté completo.

La regla de oro es que cada commit no debe dejar el proyecto sin funcionar

Dividir las tareas en pequeñas partes para guardarlas y poder revertir si algo sale mal

Add: Para archivos o funciones nuevas.

Change: Para modificar algo que ya existía.

Fix: Para correcciones de errores (bugs).

Remove: Para eliminar elementos.

EL titulo del commit no debe de ser largo max 50 caracteres

Commits Semánticos (Prefijos)

Para que el historial sea fácil de leer, usa una estructura con prefijos que indiquen qué tipo de cambio que se esta  haciendo

Prefijos:
feat: para una nueva característica para el usuario.

fix: para un bug que afecta al usuario.

perf: para cambios que mejoran el rendimiento del sitio.

build: para cambios en el sistema de build, tareas de despliegue o instalación.

ci: para cambios en la integración continua.

docs: para cambios en la documentación.

refactor: para refactorización del código como cambios de nombre de variables o funciones.

style: para cambios de formato, tabulaciones, espacios o puntos y coma, etc; no afectan al
usuario.

test: para tests o refactorización de uno ya existente.


