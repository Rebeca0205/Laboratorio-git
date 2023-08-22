# **Laboratorio-git**
Rebeca Davila Araiza

## **Cambios en repo remoto**

## Github
![Github logo](/Imagenes/GitHub-Mark.png)

- **Qué es git?**
Git es un sistema de control de versiones distribuido, en el cual un clon local de un proyecto es un repositorio de control de versiones completo. Es decir, uno puede tener un repositorio en el cual se podrá modificar los proyectos, mientras que el git estara consciente de los cambios realizados y se verán aquellos cambios que cualquier persona autorizada realizó en comparación a la version anterior. Esto es con el proposito de proteger los proyectos y siempre estar al pendiente de los cambios hechos con anterioridad.

- **Qué es GitHub**
Mientras que Github, es un portal creado para alojar proyectos de cualquier desarrollador y poder administrarlos junto con otras personas.

## Comandos de git
Durante la primera semana con git, hemos aprendido a usar los comandos basicos de git para poder actualizar y guardar cambios en github usando una Terminal. Estos comandos también puede ser realizados desde otras aplicaciones (Como en Visual Studio Code), solo que serán de distinta manera. Estos comandos escritos abajo solo se podrán realizar desde una terminal:

**cd :** change directory

**cd (Carpeta) :** sirve para poder viajar entre las carpetas de tu dispositivo
*cd Documents → cd Laboratorio_github*

**pwd :** ubicar la ruta (carpeta) en donde estemos

**ls :** el contenido de la carpeta

**git add :** revisa archivos modificados y los agrega en una área intermedia (Staging area)

**git commit :** comprometerse a los nuevos cambios y los registra en la base de datos de cambios

**git status:** se usa para checar los nuevos cambios desde el git

**git add -A:** todos los cambios que detecte los va a agregar

**git commit -m “(mensaje)”:** indicar un mensaje

**git push -u origin main :** agarrar los cambios y sincronizarlos con el repositorio remoto

**-u :** a que branch se va a subir

**history :** Te manda todo el historial de cambios y comandos escritos en el bash

**git restore --staged .DS_Store :** se escribe para no guardar datos adicionales, esto se realiza para evitar gastar espacio en la compu

### Bitacora
17/08/23: La semana pasada habia aprendido a usar los comandos de git en una terminal para actualizar y guardar cambios de mis proyectos. Hoy aprendí a hacer lo mismo, pero desde Visual Studio Code. 

1. Para eso primero solo guardo los cambios desde Visual Studio (command + S)
2. Luego ir a Source Control y ahí se verá que se acaba de realizar cambios. Si le haces clic al archivo, podrás comparar tu proyecto con su version anterior antes de los cambios
![Muestra 2](/Imagenes/Captura1.png)
3. Para guardar los cambios en git, solo hay que hacer clic en el + . Esto es el equivalente a git add -A
![Muestra 3](/Imagenes/Captura2.png)
4. Luego para registrar los cambios y mandar un mensaje, escribe en el espacio de arriba para escribir el mensaje y finalmente haces clic en una palomita arriba del mensaje
![Muestra 4](/Imagenes/Captura3.png)
5. Al final tuve que usar la terminal desde Visual Studio para mandarlo al repositorio. Solo escribí git push -u origin main

Al igual que también aprendi a escribir y añadir imagenes usando Markdown para ver lo que hago. Para tene runa referencia de como esta quedando el texto, solo hay que hacer clic derecho (en mi caso clic con 2 dedos) y hacer clic en "Markdown Preview Enhanced: Open Preview to the Side"

## Ramas y más comandos
Puedes tener distintas ramas para tener distintas personas que puedan realizar sus propios cambios y commits, para que al final todo pueda supervisarse para mandarlo a la rama principal.

***Ejemplo:***
Main: La rama principal del repositorio
Testing: rama donde se supervisa si funcionan o están correctos los cambios.
Development: rama donde se pueden hacer cambios o agregar nuevas cosas para mandarlo al main.

### Proceso
*Cuando guardas un archivo en otra rama, esta no aparecerá en otras ramas ni en el main.

1.**git branch -a :** muestra todas las ramas en el repositorio

2.**git checkout -b (Nombre de la nueva rama):** Se usa para crear una nueva rama y de una vez te cambia a esa rama

3.**git checkout (nombre de la rama):** se usa para cambiarte de rama

4.Luego realizas los cambios que deeses en los documento. Recuerda hacer add y commit

5.**git push -u origin (nombre de la rama):** Una vez que ya agregues los cambios y haces commit. Así se escribe un push perteneciente a la rama creada para que se mande a la pagina de GitHub.

6.Una vez que lo mandaste a github, te dirá que se creó una nueva rama y compare and pull request. Hace clic ahí y despues haz clic en "create pull request"

![pullrequest](/Imagenes/PullRequest.PNG)

7.Luego haz clic en "Merge pull request" para fucionarlo con la rama main. Si todo sale bien veras que se volverá morado y te dira que puedes borrar la rama. Es recomendable borrar la rama para no tener tantas al mismo tiempo.

![mergepullrequest](/Imagenes/MergePullRequest.PNG)
![pullexitoso](/Imagenes/PullExitoso.PNG)

8.Cuando le des clic en "delete branch", la rama se borrará en GitHub, pero NO en tu compu local. Para hacerlo realiza los siguientes comandos

9.**git branch -d (nombre de la rama):** borrar rama. Te dirá un error ya que no se fusionó con la rama principal desde el repositorio local

10.**git fetch --prune :** averiguar en la rama remota que cambios hay, y borra las cosas que hay que borrar (como las ramas que ya no se van a utilizar). Esto hace que ya no tengas el error al borrar la rama

11.**git pull :** descarga los cambios encontrados y los integra en la rama principal

## Trabajar en grupo en github

En github, puedes ir a settings/colaborators para agregar más personas a un repositorio. 

Cuando finalmente estés invitado y estés dentro del repositorio del lider, se debe agregar el repositorio en la computadora local.

### Proceso
1.Crea una nueva carpeta en documentos desde la terminal
**mkdir (Nombre de la carpeta):** se usa para crear una nueva carpeta

2.Luego entras a la carpeta y luego a la carpeta del repositorio
**cd (Nombre de la carpeta)**
**cd (Nombre del repositorio)**

3.Clonar el repositorio de github a nuestra computadora local
**git clone (link del SSH que se encuentra en github <>Code):** crear un nuevo repositorio y ligarlo al de github

4.Crea una nueva rama en ese repositorio
**git checkout -b (Nombre de la rama)**

5.Abres el archivo del repositorio y asi lo editas normal

6.Despues solo tienes que darle add→commit→push para mandar los cambios

7.Luego en github debes darle en pull request para mandarle los cambios al supervisor.

8.El supervisor se encargará de checar los cambios y fusionar los cambios con la rama main. 

9.Una vez que veas que el supervisor acepte todos los cambios, puede que borre tu rama. Por eso cambiate a la rama main
**git checkout main**

10.Depues actualiza los documentos con…
**git fetch --prune**

11.Descarga los cambios
**git pull**

12.Y finalmente borra tu rama desde tu computadora local
**git branch -d (nombre de la rama)**


## Referencias o guias
[Markdown Guide](https://www.markdownguide.org/)
