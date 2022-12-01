# EntornosExamen

## Creamos un repositorio el cual utilizaremos de para entorno de nuestro trabajo  

En este caso es este mismo repositorio  

## 1- Lo primero que haremos es clonar el repositorio

Copiamos la url del repositorio para clonarlo en nuestro entorno de desarrollo y hacemos un git clone URL, que en este caso es

~~~
git clone https://github.com/michaelgarciam1/EntornosExamen.git
~~~  
![image](https://user-images.githubusercontent.com/114613053/205109344-d40f121d-27d1-4104-93f6-10ffa8cf70a0.png)

## 2- Usando el comando git status para ver el estado del repositorio  
~~~
git status
~~~  
![image](https://user-images.githubusercontent.com/114613053/205109862-30f27b86-5177-4a12-ab89-e722a7f8b615.png)

## 3-Añadimos un archivo (Memoria.txt)

Añadimos “Memoria.txt” en el repositorio
~~~
git add Memoria.txt
~~~  
![image](https://user-images.githubusercontent.com/114613053/205110542-6ffaf348-5c98-4a8b-84f7-02d6b3e777c7.png)  

Y con el status vemos que hay cambios en nuestro repositorio

## 4-Hacemos nuestro primer commit:
Para hacerle un commit debemos usar el siguiente comando, siendo -m el mensaje que queremos añadir
~~~
git commit -m "mensaje"
~~~  
En nuestro caso usamos:
~~~
git commit -m "añadimos Memoria.txt"
~~~  
![image](https://user-images.githubusercontent.com/114613053/205112025-1c68c0f3-b68a-4233-a06a-832814b5d0da.png)  

## 5-Hacer un push al repositorio main
Debemos usar el comando:
~~~
git push origin main
~~~  
![image](https://user-images.githubusercontent.com/114613053/205112436-17bb0a7a-f88e-498e-a5d6-8308923e5762.png)

## 6- Vemos que los cambios estan en nuestro repositorio main
![image](https://user-images.githubusercontent.com/114613053/205112708-40c31e1f-a9f3-43df-a367-eb4fb5e6efc1.png)

## Añadimos un commit desde el repositorio main
Para hacer un commit desde el repositorio main añadimos un archivo desde github
![image](https://user-images.githubusercontent.com/114613053/205113179-2979fb8a-488c-48cd-a6da-9f14060ed357.png)

## Hacer un pull del main  
A pesar de tener cambios en el main no lo tenemos en nuestro repositorio,por ello debemos usar el comando:  

~~~
git pull origin main
~~~  
![image](https://user-images.githubusercontent.com/114613053/205113951-99132cc7-6d2a-458c-842d-4e0a6710f343.png)  


Vemos los cambios con el dir  :  

![image](https://user-images.githubusercontent.com/114613053/205114109-27db97af-4b04-4e81-b57d-0ac32ea5855a.png)  

# Practica 2

## 1-Vemos todos los commits hechos  

Usando el comando
~~~
git  log  --oneline --all
~~~  
![image](https://user-images.githubusercontent.com/114613053/205116600-6368a07b-008d-4ad1-bd30-b770b6706d84.png)  


## 2-Vemos como esta el readme

Ahora vemos como esta nuestro readme.md actualmente , como usamos CMD ,no
podemos usar el comando “cat” por ello usamos el comando “type”. Como hemos usado el
mismo repositorio que la practica 1 , habiamos usado el README.md de memoria.  
![image](https://user-images.githubusercontent.com/114613053/205116213-d95b677c-5366-4cf5-aa80-7703dbcf425c.png)  

## 3-Vamos al primer commit
Para ello debemos usar el comando “- Git checkout” con el hash del primer commit:
~~~
git checkout 3f97143
~~~
![image](https://user-images.githubusercontent.com/114613053/205116892-a755e9ae-27db-4d31-b3d1-be1b7f16691d.png)

## 4-Vemos como estaba el readme en ese instante

usando el comando type vemos el readme.md
~~~
type README.md
~~~
![image](https://user-images.githubusercontent.com/114613053/205117097-c700cf66-2221-4d74-ab08-1df18d5717d7.png)

## 5-Vemos en que rama estamos actualmente

Volvemos a usar el comando 
~~~
git  log  --oneline --all
~~~  
![image](https://user-images.githubusercontent.com/114613053/205117407-d5739c8d-638d-45a4-be6d-622ed8d4447a.png)  
Vemos que el head esta en la rama de initial commit es decir en el primer commit

## 6-nos queremos mover a la primera update del readme.md.
En nuestro caso movemos el head al commit con el comentario de memoria temporal
~~~
git checkout 0803006
~~~  
![image](https://user-images.githubusercontent.com/114613053/205117944-1ac2b49d-de9b-449b-8507-53102b3fd43d.png)  

y vemos como estaba el readme en ese momento.
![image](https://user-images.githubusercontent.com/114613053/205118223-158c9559-2584-4f93-8b90-62f0ac15ae6d.png)  
que es como estaba la primera parte de la practica sin acabar.


## 7-Volvemos a ver en que rama estamos
~~~
git  log  --oneline --all
~~~
![image](https://user-images.githubusercontent.com/114613053/205118549-df65d009-7de0-4c4e-9fed-94c20d776140.png)

## 8-volvemos a la rama master  
Para volver a la rama master debemos usar el comando “”git checkout master””
En mi caso he tenido que hace el checkout al origin/main para ir al main del repositorio de
github.  

![image](https://user-images.githubusercontent.com/114613053/205118786-6c14e92e-e017-44fb-9149-e15d6bcb07be.png)  

y con git checkout origin/main vemos que el head está en el main  

![image](https://user-images.githubusercontent.com/114613053/205119245-08d26bd2-a52a-4d37-af5a-9764ada26f9c.png)  


# 3- Preguntas de teoria  

## 1 -Directorio de trabajo (Working directory)  
El directorio de trabajo es el directorio donde se esta trabajando es decir , la carpeta donde esta el trabajo en cuestion por ejemplo, C:\Users\Michael\Documents\Git\EntornosExamen, donde entornosExamen es la raiz de las carpetas y los archivos donde residen las cosas necesarias para
el trabajo en cuestion  

## 2-Área de preparación (Staging area)  
Es el area donde se guardan temporalmente los datos, para luego ser enviados al repositorio  

## 3-Repositorio local (Directorio .git)  
Es el repositorio contenedor de archivos, en el cual trabajamos y podemos hacer los cambios locales necesarios

