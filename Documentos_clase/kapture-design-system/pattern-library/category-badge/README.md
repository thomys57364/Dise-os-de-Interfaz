# Transaction Card

## Propósito
Es el componente interactivo central diseñado para evitar el seguimiento pasivo de gastos; aísla la transacción en el Inbox y obliga al usuario a procesarla mentalmente antes de que afecte su presupuesto visible.

## Anatomía
- **Monto:** Elemento principal de la tarjeta que indica el valor de la transacción. Se utiliza tipografía con peso `font-weight-bold` y el mayor tamaño de fuente disponible para capturar la atención inmediata.
- **Origen:** El nombre del servicio o aplicación donde se realizó el gasto (ej. Uber, Starbucks) con una importancia visual secundaria.
- **Fecha/Hora:** Datos de solo lectura con tamaño reducido y color `color-text-muted` para no saturar al usuario.
- **Category Badge:** Etiqueta visual que muestra el tipo de gasto.
- **Botones de Acción:** Controles interactivos para aprobar (Verify/Approve) o rechazar (Dismiss/Discard) el movimiento.

## Reglas y Comportamientos
- El fondo del contenedor principal debe aplicar el token `color-surface` (`#1E293B`).
- Las acciones de validación (Aprobar) deben emplear el tono `color-neon-success`, mientras que las acciones de descarte emplearán `color-neon-danger`.
- Múltiples tarjetas en un listado (como el Inbox) deben separarse exclusivamente mediante espacio negativo y nunca utilizando líneas divisorias horizontales, con el objetivo de reducir el ruido visual.
- El relleno interno (padding) de la tarjeta debe alinearse a la escala base utilizando variables como `space-lg` (`24px`).
