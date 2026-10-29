# Mi Día Saludable v2.2 — Pestañas y fotografía de etiqueta nutricional

PWA de código abierto (MIT) para GitHub Pages.

## Cambios
- Apartados independientes: Inicio, Registros, Etiquetas, Planes, Ideas, Metas y Respaldo.
- Eliminado el lector de códigos de barras.
- En Etiquetas puedes subir una foto del cuadro nutricional. Tesseract.js intenta reconocer texto en el navegador; puede fallar y siempre se debe revisar/corregir manualmente.
- Las cifras se introducen según el valor de referencia de la tabla (100 g, 100 ml o porción de otro tamaño), y se calcula la cantidad a consumir.
- Estimación de impacto sobre calorías registradas hoy, sin suponer una meta calórica personal.
- Continúan las claves `mds_entries_v1`, `mds_goal_v1`, `mds_plan_v2`, `mds_food_favorites_v21`.

## Actualizar sin pérdida de datos
1. En la versión anterior, descarga **Respaldo JSON** y verifica que el archivo exista. Conserva también el CSV.
2. Haz una copia de los archivos del repositorio (puedes descargar el ZIP del repositorio en GitHub) por seguridad.
3. Sustituye `index.html`, `sw.js`, `README.md` y los otros archivos incluidos si hace falta, manteniéndolos en la raíz. Confirma los cambios en la rama `main`.
4. Espera a que GitHub Pages publique la actualización. Actualiza la página; si muestra la versión vieja, cierra/reabre la PWA o borra SOLO la caché de archivos del sitio, **no** el almacenamiento del sitio.
5. Verifica que aparezcan registros, meta, planes y favoritos anteriores.

## Privacidad y limitaciones
- Los registros se guardan en el almacenamiento local de tu navegador. No hay sincronización entre dispositivos ni cuenta de IA conectada.
- El reconocimiento OCR descarga código/modelos de Tesseract desde servicios externos cuando se usa; la imagen se procesa en el navegador. Es posible que el reconocimiento no funcione sin internet o en navegadores con poca memoria.
- El reconocimiento NO identifica automáticamente los tamaños de porción con fiabilidad, y algunas tablas muestran dos columnas. Debes comprobar nombre, energía, proteínas, carbohidratos, grasas y cantidad de referencia.
- Las calorías acumuladas solo incluyen registros de comidas con datos numéricos reconocibles, no una evaluación clínica ni un balance calórico completo.
- No guardes información de salud ni claves de API en un repositorio público.
