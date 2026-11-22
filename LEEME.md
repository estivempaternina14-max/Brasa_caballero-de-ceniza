# Brasa: caballero de ceniza (paquete PWA / Android)

Archivos: index.html, manifest.webmanifest, sw.js y la carpeta icons.
IMPORTANTE: hay que subir TODOS, incluida la carpeta icons. PWABuilder marca "falta el manifiesto"
cuando en tu sitio solo esta el index.html viejo.

## Subir a GitHub Pages
1. En github.com abre tu repositorio del juego (o crea uno llamado TU-USUARIO.github.io para que el juego
   quede en la raiz del dominio, que es lo ideal para Android).
2. Add file > Upload files. Arrastra index.html, manifest.webmanifest, sw.js y la carpeta icons completa.
   Si ya existe un index.html, se reemplaza. Pulsa Commit changes.
3. Espera 1 o 2 minutos y abre la direccion en Chrome: en el menu debe aparecer "Instalar app".

## Crear el APK
1. pwabuilder.com > pega la direccion > Start. Ya no deben salir errores de Manifest ni Service Worker.
2. Package for stores > Android. ID de paquete propio (com.tunombre.brasa). Genera una firma nueva y
   guarda el keystore y su contrasena.
3. Descarga el zip: instala el .apk en el telefono y sube el .aab a Google Play.
4. assetlinks.json debe quedar en https://TU-DOMINIO/.well-known/assetlinks.json (en la raiz del dominio).
   En un repositorio de proyecto (usuario.github.io/NombreRepo) eso no es posible; usa un repositorio
   llamado usuario.github.io o la app mostrara la barra del navegador.
