# PASOS_GITHUB
SOLO TENGO ESTE ARCHIVO PARA RECORDAR LOS PASOS DE CARGA DE UN DIRECTORIO A GITHUB


# Inicializar un nuevo repositorio Git (ESTANDO EN EL DIRECTORIO QUE VAMOS A IMPORTAR)
git init

# Agregar todos los archivos al área de preparación (staging)
git add .

# Realizar el primer commit
git commit -m "Primer commit en la rama main"

# Asociar el repositorio remoto de GitHub con tu repositorio local
git remote add origin https://github.com/RichardRosero/elasticserach_richard.git

# Cambiar a la rama principal local (main)
git branch -m main

# Empujar tus cambios a la rama principal en GitHub
git push -u origin main


# En caso de que encuentres el error "refusing to merge unrelated histories", añade estos pasos después:
# Hacer pull con la opción --allow-unrelated-histories
git pull origin main --allow-unrelated-histories

# Después del pull, realiza el push nuevamente
git push origin main


