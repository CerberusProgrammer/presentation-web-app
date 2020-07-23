- Primero necesitamos tener nuestro, Index.html.
- Despues abriremos la consola y colocaremos: npm init
- Colocar en consola: npm electron

[opcional]
- Despues crearemos un archivo package.json con este contenido:
{
    "name": "electron-quick-start",
    "version": "1.0.0",
    "description": "A minimal Electron application",
    "main": "main.js",
    "scripts": {
        "start": "electron ."
    },
    "license": "CC0-1.0",
    "devDependencies": {
        "electron": "^9.1.1",
        "electron-packager": "^15.0.0"
    }
}

- Haremos npm install
- npm start
- Listo

- Para compilar debemos hacer:

Windows:

electron-packager . nombre-app --overwrite --asar=true --platform=win32 --arch=ia32 --icon=assets/icons/win/icon.ico --prune=true --out=release-builds --version-string.CompanyName=CE --version-string.FileDescription=CE --version-string.ProductName="nombre de la app"

Linux:

electron-packager . name-app --overwrite --asar=true --platform=linux --arch=x64 --icon=assets/icons/png/1024x1024.png --prune=true --out=release-builds