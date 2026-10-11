# CALMA · OPPO A5 Pro 5G

Primera versión de recursos originales para una pantalla de inicio minimalista: 62 iconos en dos variantes y seis fondos. Los iconos se entregan como PNG de 512 × 512 y SVG editables. Los fondos PNG miden 1440 × 3200; esta medida permite recorte y no afirma la resolución nativa del teléfono.

## Estado de compatibilidad

Dispositivo indicado por el usuario: OPPO A5 Pro 5G con ColorOS 16. Se incluyen dos APK de iconos para launchers compatibles, además de los recursos gráficos. No es un archivo de tema nativo de la Tienda de temas. No cambia el panel de ajustes, las notificaciones o la pantalla de bloqueo del sistema. No se ha probado en un dispositivo físico; la región y las capacidades del launcher instalado aún no se han comprobado.

## Aplicar los fondos

1. Descomprime el ZIP y copia la carpeta `wallpapers` al teléfono.
2. Abre un archivo PNG en la galería y usa la opción para establecerlo como fondo, si aparece. También puedes seleccionarlo desde los ajustes de fondos de pantalla; los nombres de menú varían por versión.
3. Ajusta el recorte y aplica a inicio, bloqueo o ambos según las opciones disponibles. Los SVG son archivos fuente: utiliza los PNG en el teléfono.

## Aplicar los iconos

### APK para un launcher compatible

1. Copia `android/calma-claro-0.4.0.apk` o `android/calma-oscuro-0.4.0.apk` al teléfono. Puedes instalar ambos: tienen identificadores diferentes.
2. Abre el APK desde el gestor de archivos. Si Android lo solicita, habilita temporalmente la instalación desde esa aplicación y deshabilítala después. Los APK están firmados con una clave local de prototipo; no son una publicación de Google Play.
3. En un launcher que admita packs de iconos Android con el formato ADW/Nova, abre sus ajustes de apariencia y selecciona CALMA Claro u Oscuro. Las rutas exactas dependen del launcher. La compatibilidad efectiva debe probarse en el teléfono.
4. Para apps que mantengan su icono anterior, usa la edición manual del icono del launcher y elige uno de CALMA. Incluimos 42 asignaciones de componentes comunes; las apps OPPO y las variantes de región pueden necesitar selección manual.
5. Aplica el fondo por separado desde la galería. Configura la cuadrícula y el reloj según las opciones del launcher.

Al abrir CALMA se muestra una explicación: el APK no cambia automáticamente el launcher predeterminado ni aplica un tema al sistema. No solicita permisos ni acceso de red. Si no aparece en la selección de packs, ese launcher puede no admitir este formato.

### Mantener el launcher de ColorOS

No hemos verificado que el launcher original de ColorOS 16 permita cargar packs Android externos. Los PNG individuales tampoco se importan automáticamente como un pack de iconos. Comprueba si permite seleccionar una imagen para cada acceso directo; si lo permite, selecciona el PNG correspondiente en `icons/claro` o `icons/oscuro`.

Si el launcher de ColorOS no permite imágenes individuales ni packs externos, utiliza un launcher compatible para este prototipo. Un tema de Tienda de temas requiere comprobar las herramientas y el canal oficial aplicables a tu región. No renombres este ZIP o los APK a un supuesto formato de tema.

## Composición sugerida

- Cuadrícula de cuatro columnas, si está disponible; pocos accesos en la primera pantalla.
- Dock: teléfono, mensajes, navegador y cámara.
- Widget de reloj existente; estilo sencillo y sin información redundante.
- Variante clara: marfil y grafito. Variante oscura: carbón y marfil.
- Fondo liso para máxima legibilidad; fondo con arco para un detalle discreto.

Incluye símbolos genéricos y reinterpretaciones monocromas de marcas para identificar aplicaciones. `chat`, `banco` y otros nombres describen categorías; las asignaciones automáticas dependen del componente exacto de la app instalada.

## Referencias y autoría

La dirección solicitada fue https://linktr.ee/heyeaslo. Durante esta sesión devolvió HTTP 403; no se ha inspeccionado su tienda ni sus repositorios. El usuario compartió después una captura, utilizada como referencia visual para la composición de la demo. La propuesta utiliza la descripción del usuario y geometría original. No contiene productos de ese creador ni está afiliada a él o a Apple/OPPO.

## Regenerar

Requiere Python y CairoSVG 2.7.1. Desde la carpeta `calma`, ejecuta `python generate.py`. El generador escribe únicamente los recursos de este paquete. `preview.html` permite inspeccionar los PNG reales; la lámina conceptual es ilustrativa y puede diferir en detalles.

Para los APK, utiliza un Android SDK oficial con Build Tools 35.0.0, `android.jar` de API 35 y Java con el módulo `jdk.compiler`. Ejecuta `python build_android.py --tools /ruta/build-tools/35.0.0 --platform /ruta/platforms/android-35/android.jar`. Los temporales y la clave local se guardan por defecto fuera del repositorio en `/workspace/calma-android-build`; puedes cambiar esa carpeta con `--build-dir`. Conserva la clave si necesitas actualizar la instalación; no está incluida en el ZIP.

## Validación

Verificados en este entorno: compilación de ambos APK, firmas Android, alineación ZIP, manifiestos y recursos. Pendiente: instalar en el OPPO, comprobar detección por el launcher y asignaciones reales. Una compilación correcta no equivale a una prueba en ColorOS 16.

## Apps añadidas en 0.3

Reddit, Canva, IMDb, JustWatch, Claude, ChatGPT, Gemini, Grok, Outlook, Teams, Copilot, Google Play Store, Mercado Pago, Mercado Libre, Cabify, YouTube Music y Kindle. Telegram continúa incluido. Los símbolos son reinterpretaciones monocromas para este pack, no archivos oficiales de las marcas. Las asignaciones a componentes deben verificarse en el teléfono; si no coinciden, utiliza la selección manual del icono.

## Apps añadidas en 0.4

Disney+, HBO Max, Itaú, Santander y Scotiabank, en claro y oscuro. Selecciona estos iconos manualmente: no se han añadido componentes supuestos para apps bancarias o variantes de streaming. Los identificadores y actividades pueden variar según el país y la versión instalada. El buscador de la demo encuentra Itaú también al escribir itau.
