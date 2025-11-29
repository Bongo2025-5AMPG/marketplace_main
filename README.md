#Explicación de cada comando que vimos en clase.# 


- cd Documents: Con este comando se entra a la carpeta Documents del usuario.

- md nombre: Sirve para crear una carpeta con el nombre que le asignamos.

- cd nombre: Sirve para entrar a la carpeta que ya hayamos creado.

- code .: Sirve para abrir Visual Studio Code en la carpeta actual.

- dir: Este comando muestra la lista de archivos y carpetas que están dentro del directorio actual.

- pip list: Con este comando se muestran todos los paquetes de Python instalados en nuestro entorno actual, junto con sus versiones.

- python -m venv venv: Sirve para crear un entorno virtual, es como una “caja” donde se guarda todo lo que necesita nuestro proyecto sin mezclarlo con otros proyectos.

- venv\Scripts\activate: Con este comando activamos el entorno virtual, o sea la “caja” que ya creamos.

- pip install django: Sirve para instalar Django al proyecto y poder empezar a construir un sitio web.

- django-admin startproject marketplace_main: Con este comando se crea el proyecto base, se generan las carpetas y archivos necesarios para que Django pueda funcionar.

- python manage.py startapp store: Sirve para crear una aplicación dentro del proyecto. Es como abrir una sección nueva en tu sitio web.

- pip install pillow: Con este comando se instala un soporte para imágenes, permitiendo que nuestro proyecto trabaje con fotos.

- python manage.py makemigrations: Sirve para preparar los cambios en la base de datos. Django detecta las cosas nuevas que hayamos agregado y se prepara para guardarlas.

- python manage.py migrate: Con este comando se aplican los cambios a la base de datos; ahora sí, guarda todo lo nuevo que hayamos agregado en la base de datos para que funcione correctamente.

- python manage.py runserver: Con este comando se inicia el servidor web. En este punto el sitio web ya está listo para verse en el navegador. 

- python manage.py createsuperuser: Sirve para crear un usuario administrador. Este usuario administrador puede entrar al panel de control de Django y manejar todo desde ahí.

