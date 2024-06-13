# PASOS_GITHUB<br>
SOLO TENGO ESTE ARCHIVO PARA RECORDAR LOS PASOS DE CARGA DE UN DIRECTORIO A GITHUB<br>

**descargar wn windows
    winget install --id Git.Git -e --source winget

**Inicializar un nuevo repositorio Git (ESTANDO EN EL DIRECTORIO QUE VAMOS A IMPORTAR)**<br>
    git init<br>

**Agregar todos los archivos al área de preparación (staging)**<br>
    git add .<br>

**Realizar el primer commit**<br>
    git commit -m "Primer commit en la rama main"<br>

**Asociar el repositorio remoto de GitHub con tu repositorio local**<br>
    git remote add origin https://github.com/RichardRosero/elasticserach_richard.git<br>

**Cambiar a la rama principal local (main)**<br>
    git branch -m main<br>

**Empujar tus cambios a la rama principal en GitHub**<br>
    git push -u origin main<br>


# EN CASO APAREZCA UN ERROR: "refusing to merge unrelated histories", AÑADE ESTOS PASOS:<br>
**Hacer pull con la opción --allow-unrelated-histories**<br>
git pull origin main --allow-unrelated-histories<br>

**Después del pull, realiza el push nuevamente**<br>
git push origin main<br>

# **CARGAR ACTUALIZACION**<br>
<br>git add .<br>
<br>git commit -m "Mensaje descriptivo para el nuevo commit"<br>
<br>git push origin main<br>

