# PASOS_GITHUB<br>
SOLO TENGO ESTE ARCHIVO PARA RECORDAR LOS PASOS DE CARGA DE UN DIRECTORIO A GITHUB
# importante
        creas el repositoio en git antes de los demas pasos sin desmarcando el readme y el gitignore
**descargar wn windows**

        winget install --id Git.Git -e --source winget

**Inicializar un nuevo repositorio Git (ESTANDO EN EL DIRECTORIO QUE VAMOS A IMPORTAR)**

        git init

**Agregar todos los archivos al área de preparación (staging)**

        git add .
        git add README.md

**Realizar el primer commit**

        git commit -m "Primer commit en la rama main"
        
**Cambiar a la rama principal local (main)**

        git branch -M main
        
**Asociar el repositorio remoto de GitHub con tu repositorio local**

        
        git remote add origin https://github.com/RichardRosero/reposirtorio_git_nombre.git
        
**Empujar tus cambios a la rama principal en GitHub**

        git push -u origin main


**si es que quieres volver a usar el directorio local con otro repositorio de git debes cambiar la ruta por el nuevo**

        git remote -v
        
origin  https://github.com/RichardRosero/docker_api.git (fetch)
origin  https://github.com/RichardRosero/docker_api.git (push)

        git remote set-url origin https://github.com/RichardRosero/apicontact.git


        git branch -m main



# EN CASO APAREZCA UN ERROR: "refusing to merge unrelated histories", AÑADE ESTOS PASOS:<br>
**Hacer pull con la opción --allow-unrelated-histories**

        git pull origin main --allow-unrelated-histories

**Después del pull, realiza el push nuevamente**<br>

        git push origin main

# **CARGAR ACTUALIZACION**

        git add .
        git commit -m "Mensaje descriptivo para el nuevo commit"
        git push origin main
