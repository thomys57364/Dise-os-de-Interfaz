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
