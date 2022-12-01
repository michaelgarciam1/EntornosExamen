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

