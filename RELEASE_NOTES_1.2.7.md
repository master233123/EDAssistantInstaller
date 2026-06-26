# EDAssistant 1.2.7

## Cambios principales

- Manual actualizado a 1.2.7 con instrucciones completas de Quest 3, SteamVR/OpenVR, overlay VR, HUD, rutas, Galnet, ajustes, exploracion y bitacora.
- Nuevo Cuaderno de bitacora local con entradas persistentes, etiquetas, sistema asociado y notas de voz guardadas en el PC del usuario.
- Exploracion muestra vendido y pendiente estimado de exploracion/exobiologia a partir de los Journal locales.
- Rutas de exobiologia separan valor cartografico y valor biologico de Vista Genomics. Ahora se puede filtrar por planetas de 19.000.000 CR o mas cuando Spansh entrega landmarks de especies.
- Exobiologia puede evitar planetas donde ya tienes muestras registradas para crear rutas mas eficientes.
- GPS y rutas amplian la ventana de resultados consultada a Spansh para reducir casos donde solo aparecian 2 o 3 resultados.
- Vista General puede escalarse desde Configuracion sin cambiar la escala del overlay.
- HUD in-game optimizado para reducir repintados del overlay transparente y suavizar tirones de raton.
- HUD de exobiologia muestra valor biologico estimado y especies detectadas cuando estan disponibles.

## Validacion

- Compilacion del backend y frontend.
- Verificacion de rutas de exobiologia con datos reales de Spansh.
- Verificacion del manifest `latest.yml` generado por electron-builder.
