# Mi Día Saludable — Seguimiento de dieta (v3.1)

PWA de código abierto bajo licencia MIT. Esta versión muestra **únicamente funciones relacionadas con dieta y evolución del peso**.

## Funciones principales
- Resumen diario de calorías y proteínas registradas.
- Menú semanal orientativo de 7 días, editable por desayuno, almuerzo, refrigerio y cena.
- Buscador local de 35 alimentos con valores nutricionales aproximados por 100 g. La calculadora multiplica según gramos consumidos y completa el registro antes de guardarlo.
- Registro de comidas y macronutrientes, con entrada manual cuando el alimento no esté en el catálogo.
- Sumatoria diaria de calorías, proteínas, carbohidratos y grasas.
- Historial de comidas y mediciones de peso/cintura.
- Metas editables, exportación e importación JSON.

## Publicación
La aplicación está en la raíz del repositorio para GitHub Pages: https://shio-sbs.github.io/Appday/ (requiere GitHub Pages habilitado).

## Privacidad y actualización
Los datos de la nueva versión se guardan en `localStorage` con la clave `mds_dieta_v1`. No se borran las claves anteriores de la app; sus registros históricos no se muestran en esta interfaz ni se migran automáticamente. Haz respaldo JSON si deseas trasladarlos más adelante. GitHub sincroniza el **código**, no los registros personales guardados localmente en cada navegador.

Una versión independiente anterior del programa sigue en `programa-30-dias/`; no es la pantalla principal.

## Salud
Las cantidades del menú son orientativas. La app no prescribe calorías. Las cifras del catálogo son orientativas, no una base de datos nutricional verificada para marcas específicas. Registra los ingredientes de platos mixtos por separado, y revisa aceite, salsas y métodos de cocción. Antes de utilizar déficits intensivos consulta a un profesional sanitario.
