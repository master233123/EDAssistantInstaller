# EDAssistant v1.2.3

## HUD in-game

- Nuevo editor de HUD para pantalla, nave, a pie y realidad virtual.
- Paneles transparentes inspirados en la instrumentación de Elite Dangerous.
- Nuevos estilos: visor, cabina, proyección mínima, ala holográfica y carril.
- Colores configurables por panel: naranja, cian, verde, rojo y blanco.
- Ajuste de posición, tamaño y opacidad mediante cuadrícula, controles numéricos y arrastre.
- Presets equilibrado, navegación, combate y mínimo.
- Menor consumo del overlay: 15 FPS en escritorio, 30 FPS en VR y menos repintados de React.

## Exobiología y GPS

- Las rutas de exobiología muestran los planetas concretos que se deben visitar.
- Cada planeta incluye señales biológicas, distancia de llegada, atmósfera, tipo y gravedad.
- Los nombres de los cuerpos aparecen también en el HUD in-game.
- Se conservan los datos planetarios al guardar y modificar una ruta.
- Reparado el copiado manual y automático de sistemas.
- Nuevo copiado nativo de Electron con confirmación visual y alternativa para navegador.
- Botón para copiar cualquier parada de la ruta.

## Materiales e ingeniería

- Inventario en tiempo real de materiales crudos, fabricados y datos codificados.
- Catálogo local de 81 planos de ingeniería con todos sus grados.
- Búsqueda por plano y módulo.
- Selección de efectos experimentales compatibles.
- Planos fijados y lista combinada de materiales disponibles y pendientes.
- Materiales, módulos y planos traducidos según el idioma de la aplicación.
- Seguimiento de recolección, descarte, intercambio, síntesis, ingeniería y broker tecnológico.

## AlicuecanAI y configuración

- AlicuecanAI es ahora el único perfil predeterminado y disponible.
- Eliminado el generador y editor de personalidades por IA.
- Migración automática de perfiles antiguos sin conservar personalidades incompatibles.
- Añadido el crédito discreto `Creado por Master_HD-ELNidoAlicuecano` en Ajustes.

## Telemetría y estabilidad

- Corregida la indicación de escudos: el Journal solo permite saber si están activos o caídos.
- Eliminado el porcentaje de escudos inventado o incorrecto.
- Mejoras de rendimiento para reducir tirones del ratón con el overlay activo.
- Validación de compilación, migración de configuración, inventario y ejecutable portable.
