# EDAssistant 1.2.5

## VR y overlays

- Corregido el orden de inicialización: el puente VR se conecta antes de cargar el HUD para no perder el primer fotograma.
- SteamVR/OpenVR utiliza texturas GPU compartidas y confirma que el compositor acepta el fotograma.
- La aplicación ya no muestra “VR activo” hasta recibir un fotograma real del HUD.
- Activada la detección OpenXR en Windows y corregida la apertura automática cuando Elite usa un runtime OpenXR compatible.
- Añadido diagnóstico de fotogramas y errores del compositor al registro de inicio.
- Los controles de escala y visibilidad del overlay ahora se aplican realmente.
- Evitado el falso positivo que indicaba “VR activo” cuando Meta OpenXR terminaba abriendo SteamVR en segundo plano.
- En Meta OpenXR directo se abre el HUD transparente de escritorio para capturarlo con OpenKneeboard/Meta Dash.
- El HUD se oculta al abrir paneles, servicios, mapas, FSS/SAA, Codex, menú principal o pausa, y reaparece al volver al vuelo.
- El HUD normal se cierra y queda bloqueado mientras está activo el overlay VR nativo.

## AlicuecanAI

- Las rutas de neutrones y comercio calculadas por la IA pasan a ser rutas activas del GPS.
- Las rutas manuales creadas por la IA validan los sistemas contra EDSM.
- Nueva orden para preparar el siguiente salto: copia el sistema y abre el mapa galáctico.
- AlicuecanAI puede reproducir, pausar, continuar y detener noticias Galnet mediante el TTS local.
- Restaurada la carga de la voz y personalidad configuradas para la consola y las órdenes de Galnet.

## Exobiología

- El sistema actual tiene prioridad cuando contiene señales biológicas.
- Se muestran por separado los planetas con biología conocidos en el sistema actual.
- Se combinan los datos comunitarios de Spansh con señales detectadas localmente por el Journal.
- Compatibilidad con eventos `FSSBodySignals` y `SAASignalsFound`.

## Telemetría y estabilidad

- El casco se actualiza después de `Repair`, `RepairAll` y reparaciones con drones.
- Corregidos combustible tras salto/repostaje, destino, posición planetaria, salud/oxígeno a pie y estados de `Flags2`.
- El panel térmico deja de mostrar un porcentaje inexistente y usa las alertas reales del Journal.
- Los escaneos actualizan tipo, atmósfera y gravedad de los cuerpos biológicos detectados.
- Corregidos controles obsoletos del HUD y dependencias de estado del planificador de ingeniería.
- Añadidas pruebas de diagnóstico VR y validaciones de backend.

## Compatibilidad OpenXR

OpenXR no define overlays externos universales. La inyección nativa requiere que el runtime exponga
`XR_EXTX_overlay` y `XR_KHR_D3D11_enable`. SteamVR/OpenVR funciona mediante `IVROverlay`; runtimes
OpenXR directos sin esa extensión necesitan una capa compatible como OpenKneeboard.
