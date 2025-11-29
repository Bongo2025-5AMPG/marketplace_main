#Markdown#

# Explicación de cada comando que vimos en clase

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

  # DIAGRAMA Y EXPLICACIÓN DE ARQUITECTURA MVT


Django utiliza una arquitectura " MVT (Model- View - Template) "el cual es una variación del tradicional "MVC (Model-View-Controller) "

Este Modelo está estructurado para optimizar el flujo de trabajo en aplicaciones web modernas, el cual se conforma de las siguientes partes

Modelo ( Model ): Gestiona los datos y su estructura; representa la capa de acceso a datos y lógica asociada ( Interactúa con la base de datos ).

Vista ( View ): Actúa como la capa lógica, gestionando las solicitudes web, procesando datos y decidiendo cuales mostrar y cómo responder ( es la lógica de negocio ).

Plantilla ( Template ): Es la capa de presentación, encargada de mostrar visualmente los datos al usuario (se usa con rutas urls y es la interfaz del usuario ).

El flujo de información en este diagrama se genera de la siguiente forma

![Imagen](marketplace_main/media/item_images/Flujo de información en el patrón MVT.png)

1- El usuario realiza una petición HTML ( un caso podría ser accediendo a una URL).
2- El sistema de URLs de Django ("dispatcher") redirige la petición a la vista correspondiente.
3- La vista según la lógica programada, puede consultar o actualizar el modelo (accediendo a la base de datos).
4- La vista decide que datos enviar a la plantilla y llama a la función de renderizado.
5- La plantilla toma estos datos y los presenta en una página HTML dinámica, que es enviada como respuesta al usuario.




