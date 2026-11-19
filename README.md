# Carga de ventanas

Aplicación web adaptable a celulares para registrar ventanas por piso, departamento, identificador, alto y ancho, y descargar los datos como CSV compatible con Excel.

## Probar desde el celular

**[Abrir Carga de ventanas](https://norbymezz.github.io/buildingswindowsdataloader/)**

Los controles están optimizados para pantalla táctil y el formulario se acomoda en una columna en pantallas angostas. Si Pages aún no está activo, habilítalo en **Settings → Pages** seleccionando la rama **main** y la carpeta **/(root)**.

## Uso

Completa los campos y selecciona **Agregar ventana**. Los registros se conservan en el almacenamiento local del navegador de ese dispositivo. Usa **Descargar CSV** para guardar `ventanas.csv` o **Vaciar registros** para borrar la lista.

La descarga usa UTF-8 con BOM y separador punto y coma para facilitar la apertura en Excel con configuración regional en español. Las medidas se exportan con punto decimal y dos posiciones.

En navegadores compatibles, selecciona **Cargar por voz** y dicta los datos, por ejemplo: “piso 3, departamento A, ventana V-01, alto 1,20, ancho 0,90”. Los campos reconocidos se completan automáticamente y se resaltan; si falta alguno, puedes completarlo manualmente. Revisa los valores antes de agregar la ventana. El dictado requiere permiso de micrófono y puede depender del navegador; la carga manual siempre está disponible.

## Privacidad

Los datos permanecen en el almacenamiento local del dispositivo. No se envían a un servidor. El CSV solo se genera cuando seleccionas descargar. Cada dispositivo mantiene sus propios registros.

## Relación con Uizador

No se copiaron componentes de `Uizador-`: la revisión del README y la búsqueda del código no mostraron una función de reconocimiento de voz para reutilizar. La captura por voz usa la API de reconocimiento del navegador como mejora opcional.

