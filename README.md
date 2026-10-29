# Mi Día Saludable — v2.1

Actualización desde v2 sin cambiar la dirección de GitHub Pages. Incluye todas las funciones de v2, búsqueda de códigos de barras mediante Open Food Facts, detección de códigos desde fotografía cuando `BarcodeDetector` está disponible, registro nutricional por porción y productos frecuentes. Alternativa manual disponible sin internet.

## Proteger datos y actualizar

1. En la app v2 pulsa **Descargar respaldo JSON** y verifica el archivo antes de actualizar. No lo subas a GitHub.
2. En tu repositorio GitHub reemplaza `index.html`, `sw.js`, `README.md` por los de v2.1; otros tres archivos siguen iguales. Conserva la misma URL GitHub Pages.
3. Reabre la aplicación, comprueba registros, meta, planes y respalda nuevamente.
4. Consulta un código conocido, revisa los nutrientes, cambia el tamaño de porción y guarda una comida de prueba.

## Privacidad y límites

El código consultado se envía a Open Food Facts cuando pulsas Buscar. La foto usada para detectar códigos no se sube ni se conserva. No hay OCR de tablas nutricionales, autenticación, sincronización o IA externa. Los valores de Open Food Facts no están garantizados; algunos productos no existen o tienen valores incompletos. Los datos siguen almacenados en `localStorage` en el dispositivo y la restauración reemplaza registros, meta, plan y, si están incluidos, productos frecuentes. Los archivos JSON de respaldo son privados.

Licencia MIT. Datos externos sujetos a las condiciones y licencias de Open Food Facts.
