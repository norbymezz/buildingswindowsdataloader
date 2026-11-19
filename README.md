# Carga de ventanas

Aplicación web adaptable a celulares para registrar ventanas por piso, departamento, ID, alto y ancho, y descargar los datos como CSV compatible con Excel.

## Probar desde el celular

### Abrir la aplicación

**[Toca aquí para usar Carga de ventanas](https://norbymezz.github.io/buildingswindowsdataloader/?v=20261119-id25)**

> Ábrela en el navegador del celular. El enlace de abajo lleva a los archivos de GitHub y no es la aplicación.

[Ver el código en GitHub](https://github.com/norbymezz/buildingswindowsdataloader)

La aplicación se adapta a la pantalla del celular y muestra el botón **Vista para celular** para ampliar los controles. Abre el enlace desde Chrome o usa **⋮ → Abrir en Chrome** si estás viendo el README dentro de GitHub. Si no ves cambios, recarga la página; el parámetro de versión del enlace ayuda a evitar una copia guardada. Si Pages no abre, revisa [Settings → Pages](https://github.com/norbymezz/buildingswindowsdataloader/settings/pages), con la rama **main** y la carpeta **/(root)**.

## Uso

Completa los campos y selecciona **Agregar ventana**. Los registros se conservan en el almacenamiento local del navegador de ese dispositivo. Usa **Descargar CSV** para guardar `ventanas.csv` o **Vaciar registros** para borrar la lista.

La descarga usa UTF-8 con BOM y separador punto y coma para facilitar la apertura en Excel con configuración regional en español. Las medidas se exportan con punto decimal y dos posiciones.

En navegadores compatibles, selecciona **Cargar por voz** y dicta los datos de una ventana, por ejemplo: “piso 3, departamento A, ventana V-01, alto 1,20, ancho 0,90”. Chrome usa sesiones de voz de hasta **25 segundos por sesión** y muestra una cuenta regresiva; la página intenta reabrir la sesión si Chrome la corta. Toca **Detener dictado** al terminar. Los campos reconocidos se completan automáticamente. En Chrome, permite el micrófono para este sitio desde el icono junto a la dirección → **Permisos del sitio → Micrófono → Permitir**, y recarga. Si el audio se corta, cierra otras apps que usen el micrófono y prueba sin ahorro de batería. Revisa los valores antes de agregar la ventana.

## Privacidad

Los datos permanecen en el almacenamiento local del dispositivo. No se envían a un servidor. El CSV solo se genera cuando seleccionas descargar. Cada dispositivo mantiene sus propios registros.

## Relación con Uizador

No se copiaron componentes de `Uizador-`: la revisión del README y la búsqueda del código no mostraron una función de reconocimiento de voz para reutilizar. La captura por voz usa la API de reconocimiento del navegador como mejora opcional.

