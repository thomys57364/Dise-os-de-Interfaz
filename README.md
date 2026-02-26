# Dise-os-de-Interfaz

Nombre del proyecto: Kapture

Integrantes:
  1. Edwin Alejandro Rodriguez Zubieta
  2. Duvan Camilo Obando Silva
  3. Thomas Leonardo Castillo Castro

## 🎯 El Problema que se Quiere Resolver

El seguimiento pasivo de los gastos no genera consciencia financiera. Las aplicaciones tradicionales de finanzas personales se limitan a mostrar listas automatizadas de lo que el usuario ya gastó, fomentando una desconexión total con el impacto real de cada compra. Kapture resuelve esta falta de fricción introduciendo el concepto de "Consciencia Activa": obligar al usuario a procesar mental y digitalmente cada gasto antes de que este afecte su presupuesto visible.

## 👥 Los Usuarios del Sistema

El sistema está diseñado para:
* **Jóvenes profesionales y estudiantes:** Personas que buscan pasar de un control pasivo a un control estricto y activo de sus finanzas, con interés en gestionar sus gastos e historial de crédito.
* **Entusiastas del control financiero:** Usuarios que aplican la filosofía de "Zero-Based Budgeting" o "Inbox Zero", donde ninguna transacción debe quedar al aire sin ser categorizada y aprobada.

## ⚙️ Entrada, Proceso y Salida del Sistema

* **📥 Entrada (Inputs):** * Registro de transacciones financieras (monto, origen, fecha). En la fase actual, se ingresan vía cliente Web; en la futura versión móvil, se capturarán interceptando notificaciones bancarias.
  * Decisiones del usuario (acciones de "Aprobar" o "Descartar" y asignación de etiquetas/categorías).
  * Credenciales de acceso para la autenticación basada en tokens.

* **🔄 Proceso:** * Recepción de la transacción y asignación estricta del estado `pending` en la base de datos.
  * Aislamiento del gasto en el "Inbox" (no afecta los KPIs financieros globales todavía).
  * Validación de las reglas de negocio cuando el usuario procesa la transacción (cambio de estado a `approved` o `rejected` y actualización de llaves foráneas para las categorías).
  * Recálculo en tiempo real de los balances del usuario autenticado.

* **📤 Salida (Outputs):**
  * Bandeja de entrada limpia ("Todo al día").
  * Tablero de control (Overview) con KPIs actualizados: Balance total, ingresos, gastos procesados y distribución porcentual por categorías.
  * Historial inmutable de transacciones procesadas (Transactions View).

## 🚀 El Alcance del Sistema

**Lo que el sistema SÍ hace (In Scope):**
* Gestión de usuarios con autenticación segura basada en Tokens (Soporte Multi-plataforma Web/Móvil).
* Gestión de estado de transacciones mediante un flujo de aprobación manual (Inbox).
* Visualización analítica básica (Resumen financiero por estado y categoría).
* API RESTful desacoplada lista para ser consumida por diferentes interfaces de cliente.

**Lo que el sistema NO hace (Out of Scope):**
* No se conecta directamente a los servidores de los bancos para extraer datos (Open Banking / Web Scraping).
* No realiza movimientos ni transferencias de dinero real; es una herramienta de registro y visualización ("Shadow Ledger").
* No proporciona asesoría de inversión algorítmica ni cálculos de retornos financieros complejos.
   
Link de diseño en figma: https://www.figma.com/design/FMwqqgMSyiTPGnHw92Af9I/kapture?node-id=0-1&t=kpHFsRGrM1TtLPb7-1
