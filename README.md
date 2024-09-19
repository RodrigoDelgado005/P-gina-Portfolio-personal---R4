# Pagina-Portfolio-personal---R4

Para realizar los puntos debemos tener instalado node, npm y react. Para instalarlo podemos seguir lo siguiente:

Paso 1: Instala Node.js y npm Antes de instalar React, necesitas tener Node.js y npm (Node Package Manager) instalados en tu sistema. Si aún no los has instalado, sigue estos pasos:

Visita la página de descargas de Node.js en: https://nodejs.org/en/download/ Descarga el instalador para tu sistema Windows

Una vez completada la instalación, puedes comprobar que Node.js y npm están instalados abriendo un símbolo del sistema y ejecutando los siguientes comandos: node -v npm -v

Paso 2: Instala Create React App Create React App es una herramienta de línea de comandos que simplifica el proceso de configuración de un nuevo proyecto React con una estructura y configuración de proyecto recomendadas. Para instalar Create React App de forma global, abre un símbolo del sistema y ejecuta el siguiente comando:

npm install -g create-react-app

Este comando instala Create React App en tu sistema, haciendo que esté disponible para su uso en cualquier directorio.

Paso 3: Crea un nuevo proyecto React Ahora que tienes Create React App instalado, puedes utilizarlo para crear un nuevo proyecto React. Para ello, abre un símbolo del sistema, dirígete al directorio en el que quieres que se aloje el proyecto y ejecuta el siguiente comando:

create-react-app my-app Sustituye «my-app» por el nombre que desees para tu proyecto. Create React App creará un nuevo directorio con el nombre especificado y generará un nuevo proyecto React con una estructura y configuración de proyecto recomendadas.

Paso 4: Ve al directorio del proyecto e inicia el servidor de desarrollo Una vez creado el proyecto, dirígete al directorio del proyecto ejecutando el siguiente comando en el símbolo del sistema: cd my-app sustituyendo «my-app» por el nombre del directorio de tu proyecto. 

Paso 5: Debemos instalar heroicons para utilizar los iconos, esto lo haremos con el siguiente comando: 

npm install @heroicons/react

Paso 6: Debemos instalar Tailwind CSS para aplicar el diseño

npm install -D tailwindcss
npx tailwindcss init

Paso 7: En el archivo 'tailwind.config.js que se creara automaticamente al instalar Tailwind CSS debemos reemplazar su contenido por le siguiente

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}

Paso 8: Por ultimo modificaremos el archivos index.css por el siguiente contenido

@tailwind base;
@tailwind components;
@tailwind utilities;

Ahora, inicia el servidor de desarrollo ejecutando el siguiente comando: npm start

Este comando inicia el servidor de desarrollo, que vigila los cambios en los archivos de tu proyecto y recarga automáticamente el navegador cuando detecta cambios.


Problema:

Desarrollar una página web del tipo portfolio, de una sola página en la que, con diferentes componentes deberán presentar una
colección de materiales que muestre sus datos, las habilidades, logros, experiencias y los proyectos realizados. En este desarrollo se exige utilizacion de animaciones, hooks, eventos, y su correspondiente subida a un host web.

La entrega será del correspondiente link a git y al host web

Desarrollo: Debemos crear los componentes que creamos necesarios para nuestro portafolio, estos estaran en una misma pagina en diferentes seccion y al finalizar lo subiremos a un host Web a eleccion