15:06 a. m. 08/03/2021
11:58 a. m. 07/03/2021
git init

git add

git config --global user.email "you@example.com"
git config --global user.name "your Name"

git commit
git status

//entras a editor BIN para empesar a escribir digita i o y dentro de BIN digitas el nombre del commit

mi primer commit 

//te sales de BIN con QQ no le entiendo bien ?

git log

//modificas tu proyecto 

git status

//te aparecen los modificados

git checkout --<file>  // puedes descartar los cambios

git diff <file>    // te muestra las diferencias 

git add <file >    // registra los cambios en el archivo

git commit {enter} // los guarda y aparece BIN

 
//escribes la descripcion del cambio   

// presiono escape dos puntos de doble para escribir  y q para salir


git log

// (HEAD -> master) te dice la version que esta activa donde estas parado


// puedes crear el archivo  :

.gitignore

// y lo abres y digitas los nombres de las carpetas o archivos que quieres que git ignore

// pero tienes que incluir .gitignore al proyecto

git add .gitignore

git commit -m "he agregado un gitignore"

git branch // muestra los proyectos agregado y las ramas

git branch login // genera la nueva rama login 

git checkout login // cambiamos de master a la rama login

git add .  // con punto se agergan todos los archivos y carpetas del proyecto 

git commit -m "version alternativa con un login  "

// si le damos 

git log 

// nos aparecera (HEAD -> login) que es la rama donde estamos parados

// nos regresamos a master con 

git checkout master

>>>>>>>>>>>>>>>>>>>>>>GITHUB<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

Sign Up
Login
Rpositorios > New

nombre del repositorio
descripcion

publico

Create Repository

git remote add origin https://github.com/FaztTech/git-course-test.git// lo copias y lo corres en la consola donde estas ejecutando git en tu pc
                                                                        esta rarro porque hay que hacer el sigiente comando y despues volver a correr los dos 
                                                                        comandos

git push -u origin master // addiciona tus archivos en GITHUB en tu repositorio


// tepedira en la pagina de GITHUB donde estas parado que te loges y despues de logearte empezara a subir tu codigo al reporsitorio en la nue











