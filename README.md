# Proyecto-Web-Ejemplo
Proyecto para generar certificado en GitHub en Edutin con Repremundo

Proyecto creado por Ramiro Javier Galindo Orozco

## Nota sobre ramas
Las ramas `main` y `feature-mejora-estilo` se conservan en este repositorio con fines educativos: permiten practicar flujos de trabajo de Git y GitHub (creación de ramas, merges, resolución de conflictos y limpieza de ramas).

Si en algún momento se debe decidir eliminar una rama remota y/o local, los comandos correspondientes son:

```bash
git branch -d feature-mejora-estilo
git push origin --delete feature-mejora-estilo
```

## Comandos aprendidos

**clear**: limpiar terminal

**pwd**: obtener la ruta presente de trabajo

**git clone "url del repositorio" "ruta de carpeta local para clonarlo/descargarlo"**: Código de instrucciones para descargar/clonar repositorio de manera segura con respecto a su ubicación de descarga.

```bash
pwd
#salida: /c/user/Usuario/Documents/Repositorios
git clone "https://github.com/usuario/repositorio1.git"
cd "repositorio1"
pwd
#salida: /c/user/Usuario/Documents/Repositorios/repositorio1
```

**touch "ruta local"**: sirve para crear un archivo con ruta local

**echo**: Genera una cadena de texto, se puede combinar con los caracteres ">" y ">>" para generar y dejar iniciado con una línea de texto.

```bash
echo "primera línea" > archivo.txt
echo "segunda línea" >> archivo.txt
```

**git commit -m "descripción de lo que se hizo"**: Se usa para guardar y describir el progreso o modificación que se desarrolló sobre un proyecto, generando un consecutivo de hash para esa modificación, y que será guardado de manera local.

**git push**: Se usa para subir los progresos locales a la plataforma del repositorio descrito en la configuración de "origin".

**git branch**: lista las ramas existentes a nivel local

**git branch -vv**: lista las ramas existentes a nivel local con sus respectivos mensajes de commits, referencias de hash, así como sus vínculos a ramas remotas (tracking branch)

**git branch "nombre-rama"**: Crea una nueva rama de desarrollo, pero sin cambiar la movilización del usuario hacia la edición de esa nueva rama.

**git branch -d "nombre-rama"**: Elimina una rama de desarrollo a nivel local, no la elimina en el origin, sea la plataforma de GitHub, GitLab u otros. Se usa cuando las actividades y modificaciones de esa rama ya fueron integradas, aceptadas o rechazadas en la rama principal.

**git switch "nombre-rama"**: Se usa para cambiar a otra rama de desarrollo de código sin alterar lo que se desarrolló en otras ramas.

**git checkout "nombre-rama"**: cambiar rama de trabajo del usuario.

**git checkout -b "nombre-rama"**: Crear y cambiar de rama del usuario.

**git status**: Muestra un breve resumen sobre el estado de las modificaciones realizadas en la rama/branch presentes.

**git push -u origin "nombre-rama"**: Subir la nueva rama a la plataforma del repositorio, donde:
- `origin`: es el remoto por defecto en la plataforma de repositorios, sea GitHub, GitLab u otro.
- `-u`: establece el tracking branch, configurándolo como el tracking del branch presente para que el usuario pueda usarlo en comandos posteriores.

**git push origin --delete "nombre-rama"**: Elimina una rama de desarrollo en la plataforma de GitHub, GitLab u otro, se usa cuando las actividades y modificaciones en esa rama de desarrollo ya no son necesarios para continuarse, y sus propuestas de modificaciones ya fueron integradas, aceptadas o rechazadas en la rama principal.

**git merge "nombre-rama"**: Integra los cambios de una rama especificada en la rama actual.

**git diff main..nombre-rama**: Muestra las diferencias entre dos ramas.

**git checkout --theirs archivo.txt**: Durante un merge con conflictos, acepta los cambios de la rama que se está integrando (incoming changes).

**git checkout --ours archivo.txt**: Durante un merge con conflictos, acepta los cambios de la rama actual (current changes).