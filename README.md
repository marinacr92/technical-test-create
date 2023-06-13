# Prueba técnica de CREATE

Proyecto para valorar el nivel en HTML/CSS. Consiste en una página web maquetada a partir de dos archivos `.png` proporcionados (versión _Mobile_ y versión _Desktop_). Su diseño es **Responsive**, es decir, enfocado a que la web pueda verse correctamente en distintos dispositivos y pantallas. Para ello se ha hecho uso de _mediaqueries_ y de unidades “flexibles” como porcentajes (`%`), _Root EM_ (`rem`) o _viewport width_ (`vw`). De esta forma es posible su visualización tanto en versión _Mobile_ (menor a 500px), versión _Tablet_ (de 500px a 1024px) y versión _Desktop_ (mayor a 1024px).

Como base para el proyecto se ha utilizado el _Adalab Web Starter Kit_ (WSK), una plantilla de proyectos con funcionalidades preinstaladas y preconfiguradas. Éste ha sido creado en **Node** y **Gulp** e incluye un motor de plantillas **HTML**, el preprocesador **SASS** y un servidor local, que han permitido la automatización de tareas.

En el proyecto hay 3 tipos de ficheros y carpetas:

- Ficheros que se encuentran en la raíz del repositorio y constituyen la configuración del WSK.
- La carpeta `src/` con los ficheros de la página web como **HTML**, **CSS** e imágenes.
- Las carpetas `public/` y `docs/`, generadas de forma automática por el kit al arrancar el proyecto y leer los ficheros contenidos en la carpeta `src/`.

Gracias al kit ha sido posible, además, dividir el proyecto en varios _partials_, incluidos en la carpeta `src/`. Al procesar dicha carpeta, como se ha comentado anteriormente, se genera un solo archivo `index.html` y `main.css` en la carpeta `public/`. Los _partials_ del HTML son:

- _header_
- _main_
- _aside_
- _footer_

Los _partials_ de estilo (SCSS) poseen los mismos nombres que los archivos ya comentados. Además, existe un archivo creado para guardar las variables (`_variables.scss`) que se han usado con frecuencia en el proyecto, una hoja de reset (`_reset.scss`) y un archivo `_nav.scss` con las clases comunes de varios _partials_.

En resumen, para la realización de la página web se ha utilizado:

- **HTML** y **CSS** para la maquetación
- **SASS** como preprocesador de CSS
- **NPM** como gestor de paquetes y dependencias (WSK)
- **Gulp**, herramienta de automatización de tareas (WSK)

### _Scripts_ disponibles

#### `npm start`

Ejecuta la aplicación en el **modo de desarrollo**.
Abre [http://localhost:3000](http://localhost:3000) en el navegador.
La página volverá a cargar cada vez que se realicen cambios.
También es posible ver los errores en la consola.

#### `npm run docs`

Prepara la aplicación para **producción**.
Genera la carpeta `docs/` con los ficheros finales.

¡Muchas gracias!
