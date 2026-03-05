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
