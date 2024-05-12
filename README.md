# SCESI-GIT
APUNTES DE CLASE 
GIT  1ra clase
 

GIT es un sistema de control de versiones que registra cada cambio realizado en el código fuente. Es esencial para verificar cambios y solo guarda lo necesario.

    El primero en su categoría fue CVS en 1990.
    En 2005 nace GIT, creado por la comunidad de Linux.
    2008 marca la creación de GitHub.
    En 2018, Microsoft adquiere GitHub. Aunque hubo temor de que se vuelva privativo, no ocurrió un cambio radical.
    Actualmente, GIT domina el mercado en 2024.

REPOSITORIO

Un repositorio es el pilar de GIT. Se considera un almacén que guarda los archivos de un proyecto y los cambios realizados, siendo accesible para todos como un estante.
Los Tres Estados de GIT

Cualquier archivo inicializado en GIT pasa por tres estados:

    MODIFIED
    STAGED
    COMMITTED

COMMIT

Un commit registra cambios y es fundamental en GIT, equivalente a guardar la partida en un videojuego.
HEAD

Es un puntero en GIT que indica la última confirmación realizada.

COMANDOS REALIZADOS EN CLASE


**git add <archivo>:** Agrega cambios en un archivo al área de preparación.

**git status:** Muestra el estado actual del repositorio.

**git commit -m "mensaje":** Crea un nuevo commit con un mensaje descriptivo.

**git restore <archivo>:** Deshace cambios en un archivo y lo restaura.

**git log:** Muestra un registro de todos los commits.

**git commit -am -m "mensaje":** Agrega y hace commit de archivos modificados en un paso.

**git checkout <rama>:** Cambia a una rama específica del repositorio.

# **APUNTES DE CLASE GIT - 2da Clase**

Las ramas en Git no son propias de este sistema, más bien funcionan como nuevos apuntadores que permiten tener un punto de partida con un commit inicial. Es importante entender que las ramas no se fusionan nuevamente después de ser creadas.

Cuando creamos un commit inicial en una rama, esto nos ayuda a rastrear desde dónde se generan más copias y bifurcaciones. Esto resulta fundamental para trabajar en equipo, ya que permite un desarrollo no lineal y colaborativo.

Es fundamental que cada rama tenga un nombre que especifique claramente su propósito y lo que se está trabajando en ella.

Para trabajar con ramas en Git, utilizamos los siguientes comandos:
- `git branch`: para crear una nueva rama.
- `git switch`: para cambiar de una rama a otra.
- `git merge`: para fusionar ramas.
- `git branch -a`: para visualizar todas las ramas, lo que nos ayuda a decidir cuáles eliminar.

**ELIMINAR RAMAS**
¿Por qué? Para mantener limpio el espacio de trabajo.
- `git branch -d nombreDeRama`: para eliminar una rama específica.

# **APUNTES DE CLASE GIT - 3ra Clase**

## `Git remote origin`
El comando `git remote origin <url>` permite crear y eliminar conexiones con otros repositorios.

## `Git remote prune origin`
Nos permite eliminar ramas que ya no existen en el repositorio remoto y que también podemos eliminar en el repositorio local.

## `Git branch`
Nos permite crear ramas desde nuestro código y también visualizarlas.

## `Git push origin <rama>`
Nos permite sincronizar los cambios del repositorio local con el remoto.


# **APUNTES DE CLASE GIT - 4ta Clase**

# GitHub y Comandos Relevantes de Git

GitHub es una plataforma de desarrollo colaborativo basada en Git que facilita el trabajo en equipo en proyectos de software. Permite gestionar repositorios de código, hacer seguimiento de problemas, revisar código y alojar documentación. Es ampliamente utilizado en la comunidad de desarrolladores, especialmente en proyectos de código abierto.

## Comandos Relevantes de Git:

- `git clone`: Clona un repositorio remoto en la máquina local.
- `git pull`: Recupera y fusiona cambios desde un repositorio remoto a la rama local.
- `git push`: Envía cambios locales al repositorio remoto.
- `git add`: Agrega archivos modificados al área de preparación.
- `git commit`: Guarda cambios permanentemente en la historia del proyecto.
- `git branch`: Crea y gestiona ramas en el repositorio Git.


# APUNTES DE CLASE GIT - 5ta Clase

## Git Flow

### Ramas Principales

- **Main:** Destinada al código en producción.
- **Develop:** Contiene características en fase de prueba.

### Desarrollo Basado en Trunk

La integración continua mediante commits frecuentes facilita la integración de cambios. También se emplean redes de seguridad para revertir despliegues en caso de problemas.

### Estrategias de Fusionado

- **Ship:** Fusiona directamente en la rama principal sin revisión.
- **Show:** Muestra los cambios para su revisión mediante CI.
- **Ask:** Abre un PR para discutir los cambios antes de la fusión.




# APUNTES DE CLASE GIT - 6ta Clase
## Buenas prácticas en Git

- Utilizar verbos imperativos:
  - `add`: Añadir un nuevo archivo.
  - `bash`: ...
  - `git commit -m "añadimos un nuevo archivo."`: Incorrecto debido al punto final.
  - `git commit -m "para arreglar un problema..."`: Incorrecto por el uso de puntos suspensivos.
  - `git commit -m "cambiamos por defecto el sistema del color"`: Correcto, sin errores de sintaxis.

- Limitar los mensajes de commit a un máximo de 50 caracteres.
- Emplear prefijos para los commits:
  - `feat`: Nueva característica para el usuario.
  - `fix`: Corrección de un bug que afecta al usuario.
  - `perf`: Cambios que mejoran el rendimiento.
  - `build`: Cambios relacionados con el sistema.
  - `ci`: Cambios de integración.
  - `refactor`: Refactorización de código.
  - `test`: Refactorización de código existente.









