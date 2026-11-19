# Carga de ventanas

Aplicación web sencilla para registrar ventanas por piso, departamento, identificador, alto y ancho, y descargar los registros como CSV compatible con Excel.

## Probar desde el celular

**[Abrir Carga de ventanas](https://norbymezz.github.io/buildingswindowsdataloader/)**

La primera publicación puede tardar unos minutos en estar disponible. Si el enlace todavía no abre, habilita GitHub Pages en **Settings → Pages** seleccionando la rama **main** y la carpeta **/(root)**. Luego vuelve a abrir el enlace.

## Uso

Completa los campos y selecciona **Agregar ventana**. Los registros se conservan en el almacenamiento local del navegador de ese dispositivo. Usa **Descargar CSV** para guardar `ventanas.csv` o **Vaciar registros** para borrar la lista.

La descarga usa UTF-8 con BOM y separador punto y coma para facilitar la apertura en Excel con configuración regional en español. Las medidas se exportan con punto decimal y dos posiciones.

En navegadores compatibles se puede usar **Cargar por voz** y dictar, por ejemplo: “piso 3, departamento A, ventana V-01, alto 1,20, ancho 0,90”. Revisa los campos reconocidos antes de agregarlos. El reconocimiento depende del navegador y puede requerir permiso de micrófono; la carga manual siempre está disponible.

## Privacidad

Los datos permanecen en el almacenamiento local del dispositivo. No se envían a un servidor. El CSV solo se genera cuando seleccionas descargar. Cada dispositivo mantiene sus propios registros.

## Relación con Uizador

No se copiaron componentes de `Uizador-`: la revisión del README y la búsqueda del código no mostraron una función de reconocimiento de voz para reutilizar. La captura por voz usa la API de reconocimiento del navegador como mejora opcional.
