# Lista de matrimonio · Lis & Andrés

Prototipo de una lista de deseos personalizada. **No recibe pagos ni registra aportes reales.**

## Publicación en GitHub Pages

1. Sube todos los archivos y la carpeta `imagenes/` a la raíz del repositorio.
2. Ve a **Settings → Pages**.
3. En **Build and deployment**, selecciona **Deploy from a branch**, rama **main** y carpeta **/(root)**. Guarda.
4. La web estará en `https://asepulvedacl.github.io/lista-de-matrimonio/` después del despliegue.

## Cómo editar los deseos

Abre `regalos.json` en GitHub y presiona el ícono de lápiz. Cada objeto tiene:
- `id`: número único, no repetido.
- `nombre`: título del deseo.
- `descripcion`: historia o motivo.
- `precio`: monto en CLP, **sin puntos ni signo $**.
- `categoria`: nombre de la categoría para los filtros.
- `imagen`: URL HTTPS de una fotografía.

Para agregar otro regalo, copia un objeto, cambia su `id` y sus datos, y sepáralo del anterior con una coma. Asegúrate de mantener el JSON válido. Guarda con **Commit changes**. El sitio actualizará los deseos después del despliegue.

## Fotografías

La portada está en `imagenes/portada.jpg`. Para reemplazarla, sube otra imagen con ese mismo nombre y actualiza el archivo en GitHub. Las imágenes de regalos son **referenciales** y sus URL externas podrían dejar de funcionar; para una versión definitiva, conviene subir fotos propias a `imagenes/` y cambiar `imagen` a una ruta como `imagenes/cafetera.jpg`.

## Limitaciones

GitHub Pages es estático: no hay pagos, autenticación, almacenamiento de aportes ni control de regalos duplicados. Para la versión definitiva se integrará un sistema de backend o WordPress. Los valores de los regalos son de ejemplo y no cotizaciones.
