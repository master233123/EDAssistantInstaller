# EDAssistant 1.2.6

## VR y Meta Quest 3

- Añadido un modo Quest 3 reversible que fuerza `EliteDangerous64.exe` por SteamVR/OpenVR.
- La app comprueba que Elite sea realmente la escena activa de SteamVR antes de declarar el HUD VR como visible.
- Si Elite se desvía al compositor Meta/Oculus, se muestra un diagnóstico claro y no un falso estado de éxito.
- El HUD normal continúa bloqueado mientras la inyección VR nativa está activa.

## Telemetría y HUD

- El casco conserva fuente, hora de actualización y valor por nave a través de `Loadout`, daño y reparaciones.
- La última telemetría válida se guarda de forma atómica para evitar perder datos al cerrar la app.
- La pausa mediante `Esc` usa detección por flanco a 20 Hz y oculta el HUD sin capturar la tecla.
- Corregido el reconocimiento de señales `Biológica` localizadas en español.
- El panel de exobiología del HUD usa las señales locales del sistema aunque no exista una ruta activa.

## Exploración y datos

- Nuevo apartado de exploración y exobiología con sistemas, cuerpos, mapeos, señales y muestras orgánicas.
- Reconstrucción incremental de todos los Journals existentes y almacenamiento persistente en AppData.
- Los datos se escriben mediante reemplazo atómico para evitar archivos parcialmente guardados.

## Buscadores

- Los filtros y resultados de módulos, comercio y exobiología se conservan al cambiar de sección.
- Hasta 100 resultados configurables y una consulta más amplia antes de aplicar filtros locales.
- Las rutas exobiológicas pueden incluir hasta 100 sistemas objetivo.
