# Diseño-de-Interfaz

Presentación guia 6: https://canva.link/l0ojnx3d23uni53

Link de diseño en figma: https://www.figma.com/design/FMwqqgMSyiTPGnHw92Af9I/kapture?node-id=0-1&t=kpHFsRGrM1TtLPb7-1

Enlace del prototipo: https://stitch.withgoogle.com/preview/9291265267811873829?node-id=cbac23920c714fe1bf1f9ff2a72126c4

Presentacion en canva: https://canva.link/vyr3v2q7x8z7b7o
## Nombre del proyecto: Kapture

## Integrantes:

  1. Edwin Alejandro Rodriguez Zubieta
  2. Duvan Camilo Obando Silva
  3. Thomas Leonardo Castillo Castro

## El Problema que se Quiere Resolver

El seguimiento pasivo de los gastos no genera consciencia financiera. Las aplicaciones tradicionales de finanzas personales se limitan a mostrar listas automatizadas de lo que el usuario ya gastó, fomentando una desconexión total con el impacto real de cada compra. Kapture resuelve esta falta de fricción introduciendo el concepto de "Consciencia Activa": obligar al usuario a procesar mental y digitalmente cada gasto antes de que este afecte su presupuesto visible.

## Los Usuarios del Sistema

El sistema está diseñado para:
* **Jóvenes profesionales y estudiantes:** Personas que buscan pasar de un control pasivo a un control estricto y activo de sus finanzas, con interés en gestionar sus gastos e historial de crédito.
* **Entusiastas del control financiero:** Usuarios que aplican la filosofía de "Zero-Based Budgeting" o "Inbox Zero", donde ninguna transacción debe quedar al aire sin ser categorizada y aprobada.

## Entrada, Proceso y Salida del Sistema

* **Entrada (Inputs):** Registro de transacciones financieras (monto, origen, fecha). Se capturarán interceptando notificaciones bancarias.
  * Decisiones del usuario (acciones de "Aprobar" o "Descartar" y asignación de etiquetas/categorías).

* **Proceso:** Recepción de la transacción y asignación estricta del estado `pending` en la base de datos.
  * Aislamiento del gasto en el "Inbox".
  * Validación de las reglas de negocio cuando el usuario procesa la transacción.
  * Recálculo en tiempo real de los balances del usuario autenticado.

* **Salida (Outputs):**
  * Bandeja de entrada limpia ("Todo al día").
  * Tablero de control (Overview) con dashboard actualizados: Balance total, ingresos, gastos procesados y distribución porcentual por categorías.
  * Historial inmutable de transacciones procesadas (Transactions View).

## El Alcance del Sistema

**Lo que el sistema SÍ hace:**
* Gestión de usuarios con autenticación segura basada en Tokens.
* Gestión de estado de transacciones mediante un flujo de aprobación manual (Inbox).
* Visualización analítica básica (Resumen financiero por estado y categoría).

**Lo que el sistema NO hace:**
* No se conecta directamente a los servidores de los bancos para extraer datos (Open Banking / Web Scraping).
* No realiza movimientos ni transferencias de dinero real; es una herramienta de registro y visualización ("Shadow Ledger").
* No proporciona asesoría de inversión algorítmica ni cálculos de retornos financieros complejos.
   
# Diseño-de-Interfaz

Presentación guia 6: https://canva.link/l0ojnx3d23uni53

Link de diseño en figma: https://www.figma.com/design/FMwqqgMSyiTPGnHw92Af9I/kapture?node-id=0-1&t=kpHFsRGrM1TtLPb7-1

Enlace del prototipo: https://stitch.withgoogle.com/preview/9291265267811873829?node-id=cbac23920c714fe1bf1f9ff2a72126c4

Presentacion en canva: https://canva.link/vyr3v2q7x8z7b7o
## Nombre del proyecto: Kapture

## Integrantes:

  1. Edwin Alejandro Rodriguez Zubieta
  2. Duvan Camilo Obando Silva
  3. Thomas Leonardo Castillo Castro

## El Problema que se Quiere Resolver

El seguimiento pasivo de los gastos no genera consciencia financiera. Las aplicaciones tradicionales de finanzas personales se limitan a mostrar listas automatizadas de lo que el usuario ya gastó, fomentando una desconexión total con el impacto real de cada compra. Kapture resuelve esta falta de fricción introduciendo el concepto de "Consciencia Activa": obligar al usuario a procesar mental y digitalmente cada gasto antes de que este afecte su presupuesto visible.

## Los Usuarios del Sistema

El sistema está diseñado para:
* **Jóvenes profesionales y estudiantes:** Personas que buscan pasar de un control pasivo a un control estricto y activo de sus finanzas, con interés en gestionar sus gastos e historial de crédito.
* **Entusiastas del control financiero:** Usuarios que aplican la filosofía de "Zero-Based Budgeting" o "Inbox Zero", donde ninguna transacción debe quedar al aire sin ser categorizada y aprobada.

## Entrada, Proceso y Salida del Sistema

* **Entrada (Inputs):** Registro de transacciones financieras (monto, origen, fecha). Se capturarán interceptando notificaciones bancarias.
  * Decisiones del usuario (acciones de "Aprobar" o "Descartar" y asignación de etiquetas/categorías).

* **Proceso:** Recepción de la transacción y asignación estricta del estado `pending` en la base de datos.
  * Aislamiento del gasto en el "Inbox".
  * Validación de las reglas de negocio cuando el usuario procesa la transacción.
  * Recálculo en tiempo real de los balances del usuario autenticado.

* **Salida (Outputs):**
  * Bandeja de entrada limpia ("Todo al día").
  * Tablero de control (Overview) con dashboard actualizados: Balance total, ingresos, gastos procesados y distribución porcentual por categorías.
  * Historial inmutable de transacciones procesadas (Transactions View).

## El Alcance del Sistema

**Lo que el sistema SÍ hace:**
* Gestión de usuarios con autenticación segura basada en Tokens.
* Gestión de estado de transacciones mediante un flujo de aprobación manual (Inbox).
* Visualización analítica básica (Resumen financiero por estado y categoría).

**Lo que el sistema NO hace:**
* No se conecta directamente a los servidores de los bancos para extraer datos (Open Banking / Web Scraping).
* No realiza movimientos ni transferencias de dinero real; es una herramienta de registro y visualización ("Shadow Ledger").
* No proporciona asesoría de inversión algorítmica ni cálculos de retornos financieros complejos.
   
# KAPTURE Design System

Documentación del Design System del proyecto KAPTURE para la asignatura de Diseño de Interfaces.

## Arquitectura de Información

El sistema está organizado en cuatro niveles:

1. Design Tokens
2. Pattern Library
3. Design System Rules
4. Aplicaciones en el Proyecto

Esta estructura permite mantener consistencia, reutilización y escalabilidad del diseño.
# 1. Design Tokens

Los **Design Tokens** son las variables base que se utilizarán en CSS.  
En lugar de usar colores directos, se emplearán **tonos eléctricos sobre fondos gris-azulados**, lo que permite mantener consistencia visual y facilitar cambios globales en el diseño.

---

## Paleta de Colores (Colors)

| Token | Valor | Descripción |
|------|------|-------------|
| `color-bg-base` | `#0F172A` | Slate 900 – Azul noche muy oscuro para el fondo general de la aplicación. |
| `color-surface` | `#1E293B` | Slate 800 – Fondo de tarjetas y contenedores principales. |
| `color-neon-primary` | `#8B5CF6` | Violeta eléctrico – Color principal de marca y elementos de enfoque. |
| `color-neon-success` | `#10B981` | Menta neón – Usado para acciones positivas como **Aprobar**. |
| `color-neon-danger` | `#F43F5E` | Rosa/Rojo neón – Usado para acciones negativas como **Descartar**. |
| `color-text-main` | `#F8FAFC` | Blanco hueso – Color principal del texto para máxima legibilidad. |
| `color-text-muted` | `#94A3B8` | Gris claro – Usado para fechas, descripciones o información secundaria. |

---

## Espaciado (Spacing)

Sistema basado en una **escala de 4px** para mantener consistencia en toda la interfaz.

| Token | Valor | Uso |
|------|------|------|
| `space-sm` | `8px` | Separación entre íconos o elementos pequeños. |
| `space-md` | `16px` | Padding interno de botones y componentes pequeños. |
| `space-lg` | `24px` | Padding interno de tarjetas o contenedores principales. |

---


## Tipografía (Typography)

| Token | Valor | Uso |
|------|------|------|
| `font-family-sans` | `'Inter', sans-serif` | Fuente principal del sistema. Limpia, técnica y altamente legible en pantallas. |
| `font-weight-regular` | `400` | Peso estándar para texto normal. |
| `font-weight-bold` | `600` | Usado para **montos de dinero y títulos importantes**. |

---
****
# Arquitectura de la Información — KAPTURE Design System

## 1) Objetivo
Organizar y documentar el Design System para que cualquier persona pueda:
- Encontrar tokens rápidamente
- Reutilizar patrones consistentes
- Aplicar reglas de diseño
- Entender cómo las pantallas consumen el sistema

## 2) Estructura principal (niveles)

### Nivel 1: Design Tokens (`/design-tokens`)
**Qué es:** Fundaciones visuales del producto.  
**Incluye:** Colores, tipografías, espaciado, sombras, bordes, radios, etc.  
**Salida esperada:** tablas/valores + ejemplos de uso.

### Nivel 2: Pattern Library (`/pattern-library`)
**Qué es:** Componentes/patrones reutilizables.  
**Cada patrón debe tener:** propósito, anatomía, variantes, estados, reglas, accesibilidad, ejemplos.

### Nivel 3: Reglas del Sistema (`/docs/design-system-rules.md`)
**Qué es:** Principios y reglas para mantener coherencia.  
**Ejemplos:** jerarquía visual, fricción intencional, consistencia de estados.

### Nivel 4: Aplicaciones en Proyecto (`/aplicaciones-proyecto`)
**Qué es:** Pantallas del producto documentadas.  
**Debe incluir:** objetivo de la pantalla, flujo, patrones usados y decisiones clave.

## 3) Convenciones de nombres
- Carpetas en minúscula y con guiones: `detalles-transaccion`
- Patrones como “kebab-case”: `transaction-card`
- Archivos de documentación principales: `README.md` dentro de cada carpeta

## 4) Regla de oro
Si algo se repite 2 o más veces en pantallas → debe vivir en `pattern-library/`.
Si define estilo base → debe vivir en `design-tokens/`.
# Reglas del Design System (Las Leyes de UI)

Estas reglas garantizan que la aplicación se mantenga **sencilla, funcional y sin saturar cognitivamente al usuario**.

---

## Regla 1: El Neón indica Acción, no Decoración

Los **colores brillantes** (`success`, `danger`, `primary`) están estrictamente reservados para:

- Elementos interactivos (**botones, enlaces**)
- Indicadores de **estado importantes**

Todo lo que sea **solo lectura** debe mantenerse en **colores neutros**:

- `text-main`
- `text-muted`

Ejemplos de elementos solo lectura:

- Nombre de la app origen  
- Fecha y hora  
- Información secundaria  

---

## Regla 2: Respiración por Espacio Negativo (White Space)

No se usarán **líneas divisorias horizontales** (`<hr>`) para separar las transacciones en la bandeja de entrada.

La separación se logrará **exclusivamente mediante espaciado generoso**:


Esto permite:

- Reducir el **ruido visual**
- Mejorar la **legibilidad**
- Mantener una interfaz **limpia y moderna**

---

## Regla 3: Contraste Tipográfico para la Jerarquía de la Información

En aplicaciones financieras, **el número es el elemento principal**.

La jerarquía visual debe seguir este orden:

1. **Monto de la transacción**  
   - Ejemplo: **$15.50**  
   - Tamaño más grande  
   - Tipografía **bold**

2. **Aplicación o servicio de origen**  
   - Ejemplo: `Uber Eats`  
   - Importancia secundaria

3. **Fecha y hora**  
   - Tamaño más pequeño  
   - Color `text-muted`  
   - Información terciaria

Esta jerarquía permite que el usuario **identifique rápidamente la información más importante**.
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
# Category Badge

## Propósito
Ofrecer un identificador visual rápido que permita catalogar y agrupar visualmente la naturaleza de cada gasto (Transport, Food, Entertainment) dentro de los registros y tarjetas.

## Anatomía
- **Icono:** Un pictograma pequeño que refleja la temática.
- **Etiqueta:** Nombre breve de la categoría acompañando al icono.
- **Envoltorio:** Un pequeño contenedor con fondo o contorno que agrupa y delimita el componente.

## Reglas y Comportamientos
- Como es un componente puramente informativo y de solo lectura, está prohibido utilizar colores neón brillantes (reservados para interacción de estado o acción) en este elemento.
- La separación interna del componente debe ajustarse a tokens mínimos de espaciado, preferiblemente apoyándose en `space-sm` (`8px`) de la escala de 4px establecida.
