# NoticiasResumidas.com - Concepto y Misión

> **El periodismo del futuro respeta tu tiempo. Esa es nuestra premisa.**

Este repositorio contiene la documentación conceptual y la filosofía detrás de [NoticiasResumidas.com](https://noticiasresumidas.com), un medio de comunicación diseñado para la era de la sobrecarga informativa. El proyecto ha evolucionado desde un prototipo inicial hasta convertirse en un ecosistema tecnológico robusto centrado en la automatización y la eficiencia.

---

### 🎯 El Problema: La "Infoxicación"

Vivimos en un ciclo de noticias 24/7. La información es abundante, pero el tiempo es limitado. Los medios tradicionales a menudo presentan artículos extensos, llenos de repeticiones y con titulares diseñados más para el clic que para informar. El resultado es la "infoxicación": una sensación de estar saturado de información pero carente de conocimiento real.

### 💡 Nuestra Solución: Un Ecosistema Tecnológico

En NoticiasResumidas.com, aplicamos la Inteligencia Artificial no como un fin, sino como una herramienta para solucionar este problema. La solución es un ecosistema completo que incluye:

1.  **Pipeline de Procesamiento Automatizado:** Un flujo de trabajo que se encarga de todo el proceso informativo:
    *   **Scraping Inteligente:** Extracción del contenido relevante de las noticias, con mecanismos para manejar errores y bloqueos.
    *   **Sistema de Caché Multi-capa:** Todo (artículos, inferencias de LLM, imágenes) se almacena en caché para garantizar una velocidad de carga casi instantánea y minimizar costes.
    *   **Inferencia del LLM:** El texto limpio se envía a un modelo de lenguaje para su resumen y análisis.

2.  **"El Comentarista":** Más allá del resumen, hemos creado un agente de IA que aporta una primera capa de análisis y contexto, con una personalidad y biografía definidas para humanizar la interacción.

3.  **Enfoque Multiplataforma:** La información debe ser accesible donde el usuario la necesite. Por ello, el ecosistema se extiende a:
    *   **Aplicación Web Progresiva (PWA):** Para una experiencia nativa en dispositivos móviles.
    *   **Extensión para Navegadores:** Permite resumir cualquier noticia de la web directamente desde Chrome (y con planes para otros navegadores).

### 🛠️ Arquitectura y Evolución del Proyecto

El proyecto se ha construido de forma iterativa, añadiendo complejidad y robustez en cada fase. La arquitectura actual se basa en:

*   **Core del Backend (PHP):** Un backend a medida que gestiona la lógica de negocio, incluyendo un sistema de **rutas limpias** (`.htaccess`), una profunda **integración con la base de datos** para el logging de peticiones y la gestión de prompts, y un robusto **sistema de caché basado en ficheros (JSON)** para maximizar el rendimiento.

*   **Inteligencia Artificial y LLMs:**
    *   **Abstracción de Modelos:** El sistema ha sido diseñado para ser agnóstico al proveedor de LLM, habiendo integrado y balanceado cargas entre diferentes modelos (como los de Groq y Together) para optimizar costes y velocidad.
    *   **Prompt Engineering Avanzado:** Los prompts no son estáticos. Se gestionan desde la base de datos y han sido refinados continuamente para mejorar la calidad de los resúmenes, extraer categorías, generar títulos y asegurar la coherencia.
    *   **Generación de Imágenes:** El sistema puede generar automáticamente imágenes contextuales para las noticias, incluyendo una marca de agua para reforzar la identidad de la marca.

*   **Frontend y Experiencia de Usuario (UX):** Se ha puesto un gran énfasis en la interfaz, con mejoras constantes en la navegación por categorías, la presentación de artículos relacionados, los metatags para compartir en redes sociales y la creación de un panel de estadísticas y debug interno.

*   **Automatización e Infraestructura:**
    *   **Contenerización:** Se utiliza Docker para aislar y gestionar servicios clave como el scrapper, garantizando su estabilidad.
    *   **Tareas Programadas (Cron Jobs):** Múltiples procesos automáticos se encargan del relleno de contenido a través de fuentes RSS, asegurando que la plataforma esté siempre actualizada.

### 🚀 Hoja de Ruta Futura (Roadmap)

El proyecto sigue en constante evolución. Las próximas grandes líneas de trabajo se centran en:

*   **Apertura a la Comunidad:** Habilitar comentarios de usuarios y explorar interacciones entre las aportaciones humanas y las respuestas generadas por IA.
*   **Búsqueda Semántica con Vectores:** Implementar un sistema de búsqueda y artículos relacionados basado en vectores para ofrecer resultados mucho más precisos y contextuales.
*   **Soporte Multilingüe:** Expandir el alcance del proyecto mediante la traducción de contenidos y de la interfaz.
*   **Personalización y Experiencia de Usuario:** Mejorar los mensajes de carga, la interfaz de las páginas de noticias y ofrecer una experiencia más interactiva.

---

**Visita el proyecto en vivo en [www.noticiasresumidas.com](https://noticiasresumidas.com).**
