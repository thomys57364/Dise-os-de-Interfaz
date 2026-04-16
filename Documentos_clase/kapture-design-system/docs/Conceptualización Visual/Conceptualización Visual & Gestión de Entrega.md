# 🧠 Kapture – Conceptualización Visual & Gestión de Entrega

**Materia:** Diseño de Interfaces  
**Responsable:** Alejandro – Conceptualización Visual y Project Manager

---

## 🎯 Moodboard

El diseño visual de Kapture se rige bajo el **KAPTURE Design System**, cuyo objetivo es mantener la interfaz sencilla, funcional y sin saturar cognitivamente al usuario.

### Palabras Clave y Filosofía
> Dark UI · Simplicidad · Claridad financiera · Legibilidad · Funcionalidad · Diseño moderno

---

### 🎨 Código Cromático Oficial (Design Tokens)

El sistema emplea una paleta de tonos eléctricos sobre fondos gris-azulados, diseñada para facilitar cambios globales y mantener consistencia visual.

#### Fondos (Neutros)

| Token | HEX | Uso |
|-------|-----|-----|
| `color-bg-base` | `#0F172A` | Slate 900 – Fondo general de la aplicación |
| `color-surface` | `#1E293B` | Slate 800 – Superficie de tarjetas y contenedores |

#### Acentos e Interacción

> 💡 Regla del sistema: **"El Neón indica Acción, no Decoración"** — los colores brillantes se reservan estrictamente para elementos interactivos.

| Token | HEX | Uso |
|-------|-----|-----|
| `color-neon-primary` | `#8B5CF6` | Violeta eléctrico – Color principal de marca |
| `color-neon-success` | `#10B981` | Menta neón – Acciones positivas como **Aprobar** |
| `color-neon-danger` | `#F43F5E` | Rosa/Rojo neón – Acciones negativas como **Descartar** |

#### Tipografía (Textos)

| Token | HEX | Uso |
|-------|-----|-----|
| `color-text-main` | `#F8FAFC` | Blanco hueso – Texto principal, máxima legibilidad |
| `color-text-muted` | `#94A3B8` | Gris claro – Información secundaria de solo lectura |

---

### 🔤 Tipografía y Jerarquía

Se definió el uso de **Inter** (`sans-serif`) como fuente principal por ser limpia y técnica.

En Kapture, el número es el elemento principal, por lo que la jerarquía visual es:
💰 Monto → tamaño grande, peso Bold (600)
🏪 Servicio de origen (ej. Uber Eats) → tamaño mediano
📅 Fecha → tamaño reducido, color muted

---

### 📐 Estructuras y Espacio

Bajo la norma de **"Respiración por Espacio Negativo"**, el sistema omite completamente el uso de líneas divisorias horizontales entre componentes. La separación de elementos se logra mediante **espaciado generoso**, reduciendo el ruido visual y manteniendo un aspecto limpio.

---

## ❓ Preguntas Orientadoras

### Pregunta 1: ¿Qué es un Patrón de Diseño UI?

**Respuesta correcta:** Soluciones recurrentes que resuelven problemas comunes de diseño de interfaces.

Los patrones de diseño son técnicas para resolver problemas comunes en el desarrollo de software y en el diseño de interacción o interfaces. Un patrón de diseño resulta ser una solución a un problema de diseño recurrente, evitando que el equipo reinvente la rueda cada vez que necesita crear un flujo de autenticación o un panel de navegación.

---

### Pregunta 2: Cuando la interfaz está orientada al usuario, ¿qué se debe contemplar respecto al control de navegación?

**Respuesta correcta:** El usuario puede interrumpir o deshacer su acción.

Esto responde al principio heurístico de **"Control y libertad del usuario"**. Los usuarios frecuentemente eligen funciones por error y necesitan una salida de emergencia clara — como un botón de *Atrás* o *Cancelar* — para abandonar el estado no deseado, evitando la sensación de desorientación o encierro dentro de un flujo.

---

## 🖥️ Fidelidad del Prototipo

Alejandro fue responsable de ensamblar el prototipo final de Kapture, asegurando los tres niveles de fidelidad:

| Dimensión | Criterio aplicado |
|-----------|------------------|
| **Fidelidad visual** | Aplicación correcta del Design System: colores, tipografía, espaciado y componentes consistentes con el UI Kit |
| **Fidelidad de contenido** | Uso de contenido real o representativo (montos, nombres de servicios, categorías) en lugar de texto placeholder |
| **Fidelidad de funcionalidad** | Flujos interactivos conectados en Figma que simulan el comportamiento real de la app |

---



