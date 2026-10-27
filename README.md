# Portal de exámenes · Los Insurgentes · 3.º A

Versión lista para GitHub Pages. El archivo de entrada es **index.html**.
No requiere instalar Node, compilar, configurar una API ni contratar un servidor.

## Versión definitiva del primer trimestre · 26 de octubre de 2026

Este paquete sustituye todos los reportes anteriores de **Trimestre 1** por
los PDF del ZIP **chidooooooo.zip**, proporcionados por el maestro después
de su revisión final. Conserva exactamente las fotografías y las marcas
de esos archivos.

- Trimestre 1 se abre de forma predeterminada, incluso con un ID recordado.
- 25 reportes finales del primer trimestre, con sus 250 fotos revisadas.
- Vannia ya está incluida con su resultado final y su PDF.
- Dos alumnos continúan sin evaluar y sin calificación final.
- Se conservan los 24 PDF de Repaso, los mismos 27 ID, el diseño y el visor.

### Sustituir la versión anterior en EXAMENES3EROA

Extraiga este ZIP y actualice los archivos de su repositorio existente.
`index.html` debe quedar directamente en la raíz junto a `assets/`, `data/`
y `pdfjs/`. Conserve los nombres y las carpetas. No requiere compilar.

Puede subir primero los archivos de la raíz, `assets/` y `pdfjs/`, y después
`data/`, confirmando los cambios en GitHub. La página usará los resultados
definitivos al abrir de nuevo el expediente. Los reportes anteriores de
Trimestre 1 dejan de estar vinculados a los alumnos; Repaso sigue disponible.

El archivo de calificaciones para boletas se entrega por separado y se importa
en Aula Digital QR; no se incluye como lista pública dentro de la página.

## Publicar desde la página de GitHub

1. Extraiga el ZIP en su computadora.
2. Cree un repositorio para esta página, por ejemplo `EXAMENES-3A`, o abra el repositorio donde desea publicarla.
3. Entre en **Add file → Upload files**. Arrastre **todo el contenido extraído**, incluidas las carpetas. `index.html` debe quedar junto a `assets`, `data` y `pdfjs`, en la raíz del repositorio.
4. Guarde la carga con **Commit changes**.
5. Abra **Settings → Pages**. En **Build and deployment → Source**, elija **Deploy from a branch**. Seleccione la rama que contiene los archivos, normalmente **main**, y la carpeta **/(root)**. Pulse **Save**.
6. Espere a que GitHub termine la publicación. Abra el enlace que aparezca en **Settings → Pages** y compártalo con las familias.

Suba los archivos **extraídos**; GitHub Pages no abre un ZIP por sí solo. Conserve los nombres y la estructura de las carpetas. Si Windows no muestra `.nojekyll`, puede crear ese archivo vacío desde **Add file → Create new file**.

También puede subir las carpetas con GitHub Desktop y activar Pages de la misma forma. Si coloca esta página dentro de una carpeta de un sitio ya existente, conserve allí todos sus archivos juntos; las rutas están preparadas para funcionar en subcarpetas.

Documentación oficial: <https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site>

## Qué contiene

- Consulta individual mediante el ID del alumno.
- Opción **Recordar ID en este dispositivo** y botón **Olvidar ID**.
- Apartados separados: **Repaso**, **Trimestre 1**, **Trimestre 2** y **Trimestre 3**.
- 27 expedientes: Repaso conserva 24 reportes y 3 pendientes; Trimestre 1 contiene 25 reportes finales y 2 pendientes.
- Repaso: 24 PDF originales con cuatro páginas cada uno y dos fotos revisadas. Trimestre 1: 25 PDF originales definitivos con reporte, revisión detallada y diez fotos de las hojas por alumno.
- Visor incluido: **Anterior**, **Siguiente**, **Ver fotos**, **Ver reporte**, **Ampliar**, **Ajustar**, **Descargar** y **Cerrar**.
- Diseño adaptable a celular, tableta y computadora, con ajustes para orientación horizontal.
- Bibliotecas y recursos del visor incluidos en `assets` y `pdfjs`; no usa un visor de terceros ni un CDN.

## Archivos que deben permanecer juntos

| Archivo o carpeta | Uso |
| --- | --- |
| `index.html` | Página principal. |
| `assets/` | Estilos y funcionamiento de la página y del visor. |
| `data/` | Expedientes y PDF cifrados. |
| `pdfjs/` | Motor y recursos locales para mostrar los PDF. |
| `.nojekyll` | Permite publicar estos archivos como sitio estático. |
| `robots.txt` | Solicita a los buscadores que no indexen el sitio. |
| `INSTRUCCIONES.html` y `README.md` | Ayuda para publicar y mantener esta versión. |

## Cómo consultan las familias

La mamá abre el enlace, escribe el ID de su tarjeta y pulsa **Consultar exámenes**. Si activa **Recordar ID en este dispositivo**, la siguiente visita abrirá ese expediente automáticamente. Conviene usar esa opción en un dispositivo familiar.

En **Repaso**, pulse **Ver examen**. **Ver fotos** lleva directamente a las hojas fotografiadas. Para leerlas con mayor detalle, pulse **Ampliar** y deslice la hoja. **Ajustar** vuelve a mostrar el ancho completo.

## Datos y acceso

GitHub Pages publica archivos en Internet. En esta edición, los nombres, resultados y PDF se guardan cifrados; no se entrega una lista de alumnos legible ni PDF públicos sin cifrar. El navegador abre el expediente usando el ID y genera el PDF original para mostrarlo o descargarlo.

**El ID funciona como llave: cualquier persona que conozca un ID puede consultar a ese alumno.** Esta versión estática no tiene verificación de identidad en servidor ni cuentas privadas. El cifrado no convierte los ID cortos en contraseñas fuertes. Para un control de acceso mayor se necesita una plataforma con autenticación y servidor.

El ID recordado se almacena en ese navegador. **Olvidar ID** elimina el recuerdo y **Salir** cierra la consulta de la pestaña. Los archivos cifrados del sitio pueden seguir disponibles en el historial de Git del repositorio; para cambiar el acceso se debe generar y publicar una nueva versión con nuevos ID.

## Actualizaciones y uso local

Este paquete es una copia del contenido actual; no se sincroniza con la app Android, con Drive ni con la otra página publicada. Para añadir reportes o trimestres hay que generar y subir otra exportación. No cambie a mano los nombres de los archivos `.adqr`.

Use la página **publicada por HTTPS** en GitHub Pages. Abrir `index.html` con doble clic (`file://`) no permite cargar y abrir los expedientes del mismo modo. El HTML necesita sus carpetas; no es un único archivo autocontenido.

## Créditos

Visor basado en PDF.js (Mozilla), licencia Apache-2.0 incluida en `pdfjs/6.4.299/LICENSE`. Iconos Lucide, licencia ISC. React, React DOM, Noble Hashes y Noble Ciphers, licencia MIT. Los avisos se incluyen en `LICENCIAS.txt`. Las licencias de fuentes y decodificadores se incluyen junto a sus recursos.
