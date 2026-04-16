# 🧠 Kapture – Conceptualización Visual & Gestión de Entrega

**Materia:** Diseño de Interfaces  

---

# 🖥️ Microinteracciones y Animación

## ¿Qué son las microinteracciones?

Las microinteracciones son pequeños momentos dentro de una interfaz donde el sistema le responde al usuario después de que este realiza una acción. Son detalles pequeños pero muy importantes porque le dicen al usuario "tu acción funcionó" o "algo está pasando". Por ejemplo, cuando deslizas una tarjeta y esta desaparece con una animación suave, eso es una microinteracción. En Kapture, estas microinteracciones son especialmente importantes porque cada acción del usuario, como aprobar o descartar un gasto, tiene un peso financiero real, por lo que el sistema debe comunicar claramente que esa acción fue registrada.

## ¿Qué es el Motion Design y por qué importa?

El motion design es el uso controlado del movimiento dentro de una interfaz. No se trata de poner animaciones bonitas por estética, sino de usar el movimiento como una herramienta de comunicación. Un buen movimiento en una app le dice al usuario hacia dónde fue un elemento, qué acaba de pasar, o que debe esperar un momento. En otras palabras, el movimiento reemplaza palabras. En Kapture, se siguen dos principios fundamentales del motion design:

El primero es el **feedback visual**, que consiste en que cada vez que el usuario realiza una acción, la interfaz debe responder de forma visible e inmediata. Si el usuario aprueba una transacción, la tarjeta debe moverse y desaparecer de forma que confirme que fue procesada. Si la descarta, el movimiento debe ser diferente para distinguir claramente entre las dos acciones.

El segundo es **ocultar tiempos de carga**, que consiste en que cuando la app necesita procesar información o conectarse a un servidor, en lugar de mostrar una pantalla estática o un mensaje de "cargando", se usan animaciones sutiles que mantienen al usuario entretenido y con la sensación de que la app está activa y respondiendo. Esto reduce la frustración y hace que los tiempos de espera se sientan más cortos.

## Principios de motion aplicados en Kapture

Dentro del proyecto Kapture se aplican los siguientes principios para que las animaciones sean coherentes con la filosofía visual del sistema, que busca ser simple, oscura y sin ruido visual:

- **El principio de duración corta** establece que las animaciones no deben ser lentas ni llamativas. Una duración entre 200 y 400 milisegundos es suficiente para que el usuario perciba el movimiento sin que la app se sienta pesada o lenta.
- **El principio de propósito claro** establece que cada animación existe por una razón específica. En Kapture no hay animaciones decorativas, todas comunican algo: una acción fue completada, un elemento llegó, o algo está cargando.
- **El principio de consistencia** establece que elementos similares deben moverse de forma similar. Si todas las tarjetas de transacción entran desde abajo, siempre deben entrar desde abajo. Esto le enseña al usuario a leer la interfaz sin esfuerzo.
- **El principio de suavidad** establece que los movimientos deben tener una curva de aceleración natural, es decir, que empiecen rápido y terminen despacio, o viceversa, imitando el movimiento físico real. Esto se logra con funciones de easing como `ease-in-out`.

# 📐 Estrategia de Recolección de Datos

Para desarrollar el proyecto Kapture, el equipo utilizó una estrategia de recolección de datos basada en fuentes secundarias y análisis de referentes existentes en el mercado, dado que el proyecto se encuentra en una fase de diseño y prototipado y no cuenta aún con usuarios reales que puedan ser encuestados o entrevistados.

1. **La primera técnica utilizada fue el benchmarking de aplicaciones financieras**, que consistió en revisar y analizar aplicaciones similares ya existentes en el mercado como YNAB (You Need A Budget), Copilot Money y Wallet by BudgetBakers. A partir de este análisis se identificaron patrones de diseño comunes, flujos de navegación frecuentes y problemas recurrentes que los usuarios reportan en reseñas públicas de estas apps. Esto permitió al equipo entender qué funciona, qué no funciona y qué oportunidad de mejora tiene Kapture frente a la competencia.

2. **La segunda técnica fue la revisión de principios de diseño de interfaces**, que consistió en estudiar guías y estándares reconocidos en la industria como las Heurísticas de Nielsen, los principios de Material Design de Google y las Human Interface Guidelines de Apple. Esta revisión permitió tomar decisiones de diseño fundamentadas en criterios técnicos y no solo en preferencias visuales.

3. **La tercera técnica fue la definición de perfiles de usuario** basada en investigación de comportamiento financiero en jóvenes adultos. A partir de artículos y reportes sobre hábitos financieros de estudiantes y jóvenes profesionales, el equipo construyó los perfiles de usuario del sistema, identificando sus necesidades, frustraciones y motivaciones frente al manejo del dinero.

Estas tres técnicas en conjunto permitieron al equipo diseñar una aplicación con base en información real y criterios validados, asegurando que las decisiones de diseño respondan a problemas concretos y no a suposiciones.

# ❓ Preguntas orientadoras

**Pregunta 1:** Un Patrón de Diseño UI es:  
**Respuesta correcta:** Soluciones recurrentes que resuelven problemas comunes de diseño de interfaces.  
Según el marco conceptual de la guía, "Los patrones de diseño son unas técnicas para resolver problemas comunes en el desarrollo de software y otros ámbitos referentes al diseño de interacción o interfaces. Un patrón de diseño resulta ser una solución a un problema de diseño". Estos patrones evitan que reinventemos la rueda cada vez que necesitamos crear un flujo de autenticación o un panel de navegación.

**Pregunta 2:** Cuando la interfaz está orientada al usuario se debe entregarle el control de la navegación, por lo que se debe contemplar:  
**Respuesta correcta:** El usuario puede interrumpir o deshacer su acción.  
Esto responde al principio heurístico de "Control y libertad del usuario". En la navegación de la app, los usuarios a menudo eligen funciones por error y necesitan una "salida de emergencia" clara (como un botón de "Atrás" o "Cancelar") para abandonar el estado no deseado, evitando la sensación de desorientación o encierro en un flujo.

# 🎯 Moodboard

El diseño visual de la aplicación se rige bajo el **"KAPTURE Design System"**, el cual busca garantizar que la interfaz se mantenga sencilla, funcional y sin saturar cognitivamente al usuario. El Moodboard del proyecto se define por los siguientes elementos conceptuales y técnicos:

- **Palabras Clave y Filosofía:** Dark UI, simplicidad, claridad financiera, legibilidad, funcionalidad, diseño moderno.
- **Código Cromático Oficial (Design Tokens):** El sistema emplea una paleta basada en tonos eléctricos sobre fondos gris-azulados para facilitar cambios globales en el diseño.
  - **Fondos (Neutros):** Se utiliza Slate 900 (`#0F172A`), un azul noche muy oscuro, para el fondo general de la aplicación, mientras que Slate 800 (`#1E293B`) se aplica a la superficie de tarjetas y contenedores.
  - **Acentos e Interacción:** Se aplica la regla UI "El Neón indica Acción, no Decoración", reservando los colores brillantes estrictamente para elementos interactivos. El Violeta eléctrico (`#8B5CF6`) funge como color principal de marca; el Menta neón (`#10B981`) se destina a acciones positivas como "Aprobar"; y el Rosa/Rojo neón (`#F43F5E`) se utiliza para acciones negativas como "Descartar".
  - **Tipografía (Textos):** Para máxima legibilidad de lectura se emplea Blanco hueso (`#F8FAFC`), y Gris claro (`#94A3B8`) para información secundaria de solo lectura.
- **Tipografía y Jerarquía:** Se definió el uso de la familia fuente *Inter*, sans-serif, por ser limpia y técnica. En esta aplicación financiera, el número es el elemento principal, exigiendo una jerarquía donde el monto posee el tamaño más grande en peso bold (600), seguido por el servicio de origen (ej. Uber Eats), y finalizando con fechas en tamaños reducidos.
- **Estructuras y Espacio:** Bajo la norma de "Respiración por Espacio Negativo", se omite por completo el uso de líneas divisorias horizontales (`<hr>`) entre componentes (como las transacciones). La separación de elementos se logra mediante un espaciado generoso para reducir el ruido visual y mantener un aspecto limpio.
