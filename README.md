# Comandos git
**Es para agregar todos los archivos que se cambiaron**

`git add .`

**Es para agregar razon de actualizacion y push**

`git commit -m "<razon, descripcion del cambio>"`

**Es para agregar a github los cambios**

`git push <origin> <branch>`

**Traer todos los cambios que se hicieron de la rama actual**

`git pull <origin> <branch>`

**Es para ver que branches existen dentro de tu git y en cual estas trabajando**

`git branch`

**Actualizar todo el arbol de trabajo**

`git fetch --all`

**Traer branch creada en github a tu computadora**

`git checkout -t <origin>/<branch>`

**Cambiar de branch en tu computadora**

`git checkout <branch>`

**Para ver el status de tu commit (Que archivos se cambiaron, cuales se agregaron y cuales no con el .gitignore)**

`git status`

---

## Ejemplos

### Pasos para guardar cambios
1- `git add .`
2- `git commit -m "<razon>"`
3- `git push <origin> <branch>`

### Actualizar arbol de trabajo y crear branch en computadora que se encuentra en github
1- `git fetch <origin>`
> Este git fetch <origin> es para actualizar solo el arbol de trabajo de un repositorio, se puede utilizar git fetch --all por si se tienen más de 1 repositorio en nuestra computadora

2- `git checkout -t <origin>/<branch>`

### Cambiar cambios de una branch de mi computadora a otra
> Como ejemplo: Cuando tenemos 2 branches main y development, hicimos cambios en main cuando se necesitaban en development

1- `git stash` -> Este para guardar los cambios que se hicieron en la branch
2- `git checkout <branch>` -> Cambiamos de branch
3- `git stasth apply` -> Ya estando en la branch que necesitamos agrega los cambios guardados del stash