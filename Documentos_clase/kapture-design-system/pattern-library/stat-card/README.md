# Stat Card

## Propósito
Desplegar resúmenes financieros fundamentales en el Dashboard para mantener al usuario informado del recalculado en tiempo real de sus ingresos, gastos y transacciones pendientes.

## Anatomía
- **Título del Indicador:** Identifica la métrica (ej. "Total Expenses", "Pending Items").
- **Icono de Tendencia/Estado:** Un apoyo visual en la esquina superior que denota dirección o alertas.
- **Valor Monetario:** La cifra total calculada, presentada en peso `font-weight-bold`.
- **Contexto Temporal:** Subtítulo de apoyo (ej. "Last 30 days" o "Action Required").

## Reglas y Comportamientos
- El número de la estadística debe ser siempre el primer elemento en captar la jerarquía visual de la tarjeta.
- Toda la información secundaria (título de la estadística y contexto de tiempo) debe permanecer como texto de solo lectura usando el color `color-text-muted` para no distraer la atención de los datos críticos.
