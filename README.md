# Estilos2-SASS-Full-Stack-2203
Landing Page con SASS

Pasos a seguir para iniciar SASS en nuestro proyecto:

Abrimos en nuestra terminal en Visual Studio con ctrl+ñ e instalamos el archivo package.json con el comando: npm init

Instalamos carpeta de node y el archivo package-lock.json con el comando: npm install node-sass nodemon

En el archivo package.json agregamos estas lineas de código desde de "scripts": {
"build-css": "node-sass --include-path scss scss/style.scss css/style.css",
"watch-css": "nodemon -e scss -x \"npm run build-css\"",

Por lo cual desde la linea 6 hasta la 10 deberían quedar:

  "scripts": {
    "build-css": "node-sass --include-path scss scss/style.scss css/style.css",
    "watch-css": "nodemon -e scss -x \"npm run build-css\"",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  
Luego de esto, escribimos para iniciar SASS el comando: npm run watch-css
  
Si aparece esta leyenda: 
Rendering Complete, saving .css file...
Wrote CSS to C:\Users\Usuario\Desktop\SASS\css\style.css
[nodemon] clean exit - waiting for changes before restart

Felicitaciones, ya podés escribir estilos desde SASS en tu proyecto.
