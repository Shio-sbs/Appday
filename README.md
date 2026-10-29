# Mi Día Saludable — v2 (local)

PWA abierta con licencia MIT, sin cuentas ni servicios de terceros. Incluye registros v1, meta de peso, exportación CSV, **respaldo completo y restauración JSON**, plantillas generales de menús semanales, plan manual y sugerencias locales.

## Actualizar sin perder registros

1. **Desde la versión 1**, exporta CSV y anota tu meta de peso.
2. En el mismo repositorio y misma URL de GitHub Pages, reemplaza los archivos `index.html`, `sw.js` y `README.md` por los de esta versión (mantén los demás). No borres los datos de Chrome.
3. Recarga la PWA; si sigue en v1, cierra y abre o recarga la página.
4. Verifica que los registros y meta anteriores siguen visibles. La v2 **mantiene** las claves `mds_entries_v1` y `mds_goal_v1`; no borra ni transforma tus datos.
5. En v2 descarga un respaldo JSON, verifica que el archivo se guardó y consérvalo en lugar privado. Para restaurar, pulsa **Restaurar respaldo JSON**. La restauración **reemplaza** registros, meta y plan locales; nunca lo hagas sin guardar antes copia actual.

## Publicación

GitHub → tu repositorio → Add file → Upload files → arrastra los seis archivos (GitHub solicitará confirmar el reemplazo de archivos existentes) → Commit changes. Pages debe permanecer configurado en `main` y `/(root)`. En caso de conflictos en la interfaz de carga, edita archivos individualmente con el lápiz o usa la interfaz web de github.dev para reemplazarlos.

## Limitaciones

Los registros se guardan en `localStorage` del navegador actual: no se sincronizan entre dispositivos. La exportación CSV contiene solo registros; JSON incluye también meta y plan. Los planes son ideas genéricas, no prescripciones personalizadas. No hay OCR, escáner de barras, login ni conexiones de IA todavía. No subas tus archivos JSON de respaldo al repositorio público ni pegues claves de API en el frontend.
