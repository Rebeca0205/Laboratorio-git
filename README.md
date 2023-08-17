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
3. Para guardar los cambios en git, solo hay que hacer clic en el + . Esto es el equivalente a git add -A
4. Luego para registrar los cambios y mandar un mensaje, escribe en el espacio de arriba para escribir el mensaje y finalmente haces clic en una palomita arriba del mensaje
5. Al final haces clic en send changes para mandarlos al repositorio de Github. Esto es el equivalente de git push -u origin main

Al igual que también aprendi a escribir y añadir imagenes usando Markdown para ver lo que hago.

## Referencias o guias
[Markdown Guide](https://www.markdownguide.org/)
