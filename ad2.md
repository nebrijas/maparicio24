# Actividad dirigida 2


# En este espacio se explica como ha sido el desarrollo de la actividad 2 

1. El primer paso fue descargar e instalar la terminal **Git Bash* que permite conectar con el repositorio **Git Hub**

2. Tras instalada la aplicación se dio inicio la construcción de *la web*

3. Dando continuidad al trabajo lo que se hizo fue cambiar el **README.md** a la *ad1.md* para esto usamos el **Git Bash**

4. Luego convertimos los archivos **Markdonw** a **HTML**

5. Entramos a Https://github.com/maparicio24/settings/pages y desde ahí se hizo el proceso para convertirlo en **HTML**
 
6. En el **Git Bash** se escribió el comando `pwd` el cual permite saber en cual directorio estamos

7. Luego clonamos a través de `git clone https://github.com/nebrijas/maparicio24 que permite copiar el directorio de nuestro repositorio

8. Pusimos un `ls` para ver la carpeta creada en el directorio

9. Accedimos a la misma con el `cd` y el nombre de la carpeta, es decir así `cd maparicio24` y con *enter* seguimos escribiendo

10.Dentro de la carpeta, pusimos `ls` para ver el contenido que hay en su interior.

11. Después puse `git config user.name` con mi usuario `maparicio24`y le di *enter* luego `git config user.email` seguido del correo que  utilizé en  **GitHub**

12. Generamos un token en la *web* https://github.com/settings/tokens por 60 días 

13. Luego copiamos el *token* que se ha creado 

14. Seguimos con `echo "(aquí dentro el token copiado previamente)"> ../.token` 

15. Escribi`README.md ad1.md` que copia el contenido de **README.md** a la nueva carpeta **ad1.md**.

16. Después puse el editor de texto `nano README.md` y se puso el título y dos enlaces, uno a **ad1.md** y otro a este directorio (**ad2.md**)

17. Con `git status` vimos las modificaciones que se hizo

18. Luego escribi  `git add` seguido del nombre del archivo

19. Después con `git commit -m "modifico README.md y añado ad1.md"` se escribió para los pasos que se hizo.

20. Con `git push` guardamos el contenido en **GitHub**.


21. Con el código `git pull` puedo ver los cambios en la web a través del archivo local.
