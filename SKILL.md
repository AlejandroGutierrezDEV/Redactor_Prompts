---
name: redactor-prompts
description: Redacta, mejora y optimiza prompts para modelos de IA (Claude, ChatGPT, Gemini, generadores de imágenes, agentes y system prompts). Úsala siempre que el usuario pida escribir un prompt, mejorar o corregir uno existente, convertir una idea en instrucciones para una IA, crear un system prompt, una plantilla de prompt, o diga cosas como "hazme un prompt para...", "cómo le pido a la IA que...", "este prompt no funciona" o "prompt para generar una imagen", aunque no use la palabra "prompt".
---

# Redactor de prompts

Convierte una idea o necesidad del usuario en un prompt **claro, completo y listo para copiar y pegar**. Un buen prompt reduce la ambigüedad: la IA no puede adivinar el contexto, el objetivo ni el formato que el usuario tiene en la cabeza.

## Flujo

1. **Entiende el objetivo.** Identifica qué quiere conseguir el usuario, para quién es el resultado y en qué herramienta lo usará (chat, API, generador de imágenes, agente...). Si ya lo ha dicho o se deduce, no preguntes.
2. **Completa lo que falte.** Pregunta como máximo una vez y solo lo imprescindible (por ejemplo, el público o el formato final). Si el usuario tiene prisa o la petición es clara, asume valores razonables y señálalos en una línea.
3. **Redacta el prompt** con la estructura de abajo, adaptada al tipo de tarea. Para plantillas concretas por tipo, lee `references/plantillas.md`.
4. **Entrega el resultado** en un bloque de código para que se copie sin errores, seguido de una nota breve con las decisiones clave y cómo adaptarlo.
5. **Ofrece iterar:** una versión más corta, más estricta, con ejemplos o para otra herramienta.

## Estructura de un buen prompt

Usa solo las partes que aporten valor; un prompt sencillo no necesita las ocho.

1. **Rol** (opcional): quién debe ser la IA. Útil cuando el punto de vista cambia la respuesta.
2. **Contexto**: situación, público, material de partida y para qué se usará el resultado.
3. **Tarea**: lo que debe hacer, con verbos concretos y en positivo.
4. **Restricciones**: qué debe evitar, límites de longitud, tono, idioma, fuentes permitidas.
5. **Formato de salida**: estructura exacta (lista, tabla, JSON, número de párrafos, etc.).
6. **Ejemplos** (opcional): uno o dos de entrada y salida esperada. Son la forma más fiable de fijar estilo y formato.
7. **Criterios de calidad**: cómo saber que está bien hecho.
8. **Datos de entrada**: marca claramente dónde pegará el usuario su contenido, por ejemplo `[PEGA AQUÍ EL TEXTO]`, o delimítalo con etiquetas como `<texto>...</texto>`.

## Principios de redacción

- **Sé específico.** "Resume en 5 viñetas de máximo 15 palabras para un directivo" funciona mejor que "resume esto".
- **Explica el porqué** de las restricciones importantes; la IA las respeta mejor cuando entiende el motivo.
- **Pide lo que sí quieres** en lugar de solo lo que no. Las negaciones solas confunden.
- **Separa instrucciones y datos** con etiquetas o delimitadores para evitar que el contenido pegado se confunda con órdenes.
- **Pide razonamiento por pasos** solo en tareas de lógica, cálculo o decisiones; en tareas simples alarga sin mejorar.
- **Ajusta la longitud al problema.** Un prompt largo no es mejor por serlo; elimina lo que no cambie el resultado.
- **No inventes capacidades.** No asumas que la IA tiene internet, memoria o acceso a archivos si no sabes que los tiene.

## Cuando el usuario trae un prompt ya escrito

1. Diagnostica en pocas líneas qué falla (ambiguo, sin formato, sin contexto, contradictorio, demasiado largo...).
2. Entrega la versión mejorada completa en un bloque de código.
3. Resume los cambios en una lista corta para que el usuario aprenda qué se modificó.

## Adaptación por herramienta

- **Chat y asistentes de texto:** estructura clara con etiquetas o secciones; indica el formato de salida.
- **Generadores de imágenes:** describe sujeto, entorno, estilo, iluminación, composición y formato; sé concreto y evita nombres de personas reales o marcas protegidas.
- **System prompts y agentes:** define rol, objetivos, herramientas disponibles, reglas de comportamiento, qué hacer ante la duda y formato de las respuestas.
- **Uso por API o automatizado:** exige un formato de salida estricto (por ejemplo, solo JSON) y prevé los casos límite.

## Formato de la respuesta

```
## Prompt

<bloque de código con el prompt listo para copiar>

## Notas
- Decisión clave 1
- Cómo adaptarlo (variables que puede cambiar)
```

Si el usuario pide varias versiones, etiquétalas por objetivo (por ejemplo, «Breve», «Estricto», «Con ejemplos»).
