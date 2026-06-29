# Notas de la Versión - EDAssistant v1.3.0

Esta versión centra los cambios en exobiología y búsqueda cercana.

## Exobiología
* Se eliminan los filtros antiguos de valor geológico/cartográfico y valor biológico mínimo.
* Se añade filtro por una o varias familias de plantas: Aleoida, Bacterium, Cactoida, Clypeus, Concha, Electricae, Fonticulua, Frutexa, Fungoida, Osseus, Recepta, Stratum, Tubus y Tussock.
* Cada planta muestra su valor aproximado de Vista Genomics en la interfaz.
* La ruta filtra realmente los cuerpos por las plantas elegidas en backend, no solo en pantalla.
* El filtro para evitar planetas ya muestreados ahora normaliza nombres y también tiene en cuenta cuerpos con biología guardados en el registro local.
* Los planetas del sistema actual que vienen del Journal ya no se reinsertan si el usuario ha pedido evitar repetidos o filtrar plantas concretas.

## Buscar Cercano
* La antigua pestaña de búsqueda de piezas se reemplaza por un buscador cercano más amplio.
* Nuevas categorías: estaciones, comerciantes de materiales, módulos, naves, mercancías, facciones menores, sistemas, cuerpos y señales.
* Se añaden controles de resultados, distancia máxima, llegada máxima, ordenación y exclusión de portanaves/asentamientos.
* Los resultados se pueden copiar directamente desde la tabla.
* La app usa fuentes públicas compatibles con la base de datos galáctica de EDAssistant. La API pública documentada de Inara requiere clave y no expone los mismos endpoints web de búsqueda avanzada, por lo que queda preparada la estructura para conectar un proveedor Inara si se aporta un endpoint/evento compatible.

## Actualización
* Versión interna, backend, Electron y auto-update actualizados a `1.3.0`.
* Publica `EDAssistant-Setup-1.3.0.exe`, su `.blockmap` y `latest.yml` en el repositorio oficial de instaladores para que el actualizador automático detecte esta versión.
