# Registro Komplex

Aplicación de registro del Komplex Gym: inventario por áreas, proveedores, técnicos y lineamientos.

Es un solo archivo HTML con JavaScript puro. No usa librerías, ni servidor, ni conexión a internet
para funcionar. Se puede abrir desde la web o descargando `index.html` y haciendo doble clic.

## Cómo se usa

- **Modo edición** (botón rojo): convierte títulos, textos y celdas en campos editables. Guarda solo.
- **Insertar imagen**: dentro de cada bloque de texto. La imagen se reduce a 1280 px y queda dentro del registro.
- **Consulta de inventario**: se elige área, categoría, estado o una palabra y sale una sola lista con lo que coincide.
- **Respaldo / Restaurar**: baja o carga un archivo `.json` con toda la información.
- **Imprimir**: saca la sección actual sin menú ni botones.

## Dónde se guarda la información

En el almacenamiento local del navegador (`localStorage`), no dentro del archivo ni en GitHub.

Esto significa que la información **no se comparte entre dispositivos ni entre navegadores**: cada
navegador tiene su propia copia. Para pasar los datos de un equipo a otro se usa **Respaldo** en el
primero y **Restaurar** en el segundo. Conviene hacer un respaldo con regularidad, porque borrar los
datos de navegación del navegador también borra el registro.

El límite de almacenamiento del navegador ronda los 5 MB, contando las imágenes.

## Estructura

- `index.html` — la aplicación completa.
