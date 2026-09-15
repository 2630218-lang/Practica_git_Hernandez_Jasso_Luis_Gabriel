# Creación y sincronización de repositorios con Git y GitHub

> **Información del Estudiante**  
> **Nombre:** Luis Gabriel Hernandez Jasso  
> **Matrícula:** 2630218  

---

## 🎯 Objetivo
> Crear un repositorio local utilizando Git, sincronizarlo con un repositorio remoto en GitHub y comprobar el flujo de trabajo en ambos sentidos.

---

## 📋 Procedimiento
El procedimiento que realice fue mediante pasos a seguir los cuales fueron:

```
[ Paso 1 ] Crear el repositorio local
    │
    ▼
[ Paso 2 ] Registrar los primeros cambios
    │
    ▼
[ Paso 3 ] Crear el repositorio en Github
    │
    ▼
[ Paso 4 ] Realizar un cambio desde Github para verificar si se hacia el cambio en mi computadora
    │
    ▼
[ Paso 5 ] Realizar un cambio desde mi computadora para verificar si se hacia el cambio en github
```

---

## 🛠️ Comandos de Git utilizados

```bash
git init
git branch -m main
git status
git add .\README.md
git add -a
git add -A
git commit -m "Mi primer commit"
git commit -m "archivo txt modificado se me olvido agregarle lo relacionado "
git log
git remote add origin https://github.com/2630218-lang/Practica_git_Hernandez_Jasso_Luis_Gabriel.git
git remote -v
git push origin main
git pull origin main
git commit -m "Actualizacion desde el repositorio local "
git push
git -u push
```

---

## 💡 Explicación breve de la función de cada comando

| Comando | Explicación / Función |
| :--- | :--- |
| `git init` | Crea un repositorio de Git nuevo y vacío en la carpeta actual. |
| `git branch -m main` | Renombra la rama actual a main. |
| `git status` | Muestra el estado del repositorio (qué archivos cambiaron o faltan por guardar). |
| `git add .\README.md` | Agrega únicamente el archivo README.md al área de preparación (staging). |
| `git add -a` | Intentaste agregar todo, pero dio error porque la -a debe ser mayúscula. |
| `git add -A` | Prepara todos los archivos nuevos y modificados para el siguiente commit. |
| `git commit -m "..."` | Guarda una foto/snapshot en el historial con un mensaje descriptivo. |
| `git log` | Muestra la lista con el historial de commits realizados. |
| `git remote add origin <URL>` | Conecta tu repositorio local con tu proyecto en GitHub (origin). |
| `git remote -v` | Muestra las URLs remotas vinculadas a tu proyecto. |
| `git push origin main` | Sube tus commits locales a la rama main de GitHub. |
| `git push` | Intentaste subir cambios rápido, pero dio error por falta de configuración de rastreo. |
| `git pull origin main` | Descarga e integra en tu computadora los cambios que están en GitHub. |
| `git -u push` | Dio error de sintaxis porque la opción -u va después de push (`git push -u origin main`). |

---

## 🖥️ Explicaciones del Proceso

### 💻 Explicación de cómo se creó el repositorio local
> El repositorio local se creo despues de hacer una carpeta se realizo un git init y de ahi se crea el repositorio local

---

### 🔗 Explicación de cómo se vinculó el repositorio local con GitHub
> El repositorio se vinculo a github mediante su pagina web, ahi se creo un repositorio y se saco el https despues en la powersell se utilizo el comando `"git remote add origin <URL>"` y se copio el https que dio git hub

---

### ⬆️ Explicación de la sincronización Local → GitHub
> Para sincronizar los archivos de local a github primero se tienen sacar los archivos de untrack files con el comando `git add "nombre del archivo"` o `git add -A` despues se tiene que realizar un commit, para verificar que el commit se hizo bien se usa el comando `git log` suponiendo que ya tienes el repositorio vinculado se usa el comando `"git push origin main"`

---

### ⬇️ Explicación de la sincronización GitHub → Local
> Para sincronizar los archivos de github a local es mas facil solo haces el commit en la pagina de github al terminar de hacer los cambios y en la powersell pones el comando `"git pull origin main"`

---

## 📁 Descripción de los archivos contenidos en el repositorio

- 📄 **`data.txt`**: Se uso para verificar si estaba funcionando bien la sincronizacion local a github y viceversa.
- 📘 **`README.md`**: Se esta utilizando como bitacora para guardar lo aprendido.

---

## 🎓 Conclusión personal sobre lo aprendido

> Aprendi a hacer un repositorio local a github y viceversa tambien aprendi a hacer cambios desde github y realizar commits ahi y como descargar el commit a mi repositorio local