# Plantillas de prompts por tipo de tarea

Sustituye lo que aparece entre corchetes. Elimina las líneas que no necesites.

## Índice
1. Redacción y edición de texto
2. Resumen y análisis
3. Código
4. Estudio y aprendizaje
5. Generación de imágenes
6. System prompt para un asistente o agente
7. Extracción de datos en formato estructurado

## 1. Redacción y edición de texto
```
Eres [rol, p. ej. editor profesional].
Contexto: [para qué es el texto y quién lo leerá].
Tarea: [escribe / reescribe / corrige] el siguiente texto.
Tono: [formal / cercano / técnico]. Longitud: [n palabras].
Evita: [muletillas, tecnicismos, etc.].
Texto:
<texto>
[PEGA AQUÍ EL TEXTO]
</texto>
```

## 2. Resumen y análisis
```
Analiza el documento y entrega:
1. Resumen en [n] viñetas de máximo [n] palabras.
2. Ideas clave y datos relevantes.
3. Posibles dudas o puntos débiles.
Público: [quién lo leerá]. Si algo no aparece en el documento, indícalo en lugar de suponerlo.
<documento>
[PEGA AQUÍ EL DOCUMENTO]
</documento>
```

## 3. Código
```
Actúa como desarrollador [lenguaje/framework] con experiencia en [área].
Objetivo: [qué debe hacer el código].
Entorno: [versión, librerías permitidas, restricciones].
Entrega: [solo el código / código con explicación breve].
Incluye: [manejo de errores, comentarios, pruebas].
Código actual (si existe):
<codigo>
[PEGA AQUÍ EL CÓDIGO]
</codigo>
```

## 4. Estudio y aprendizaje
```
Soy estudiante de [nivel/curso] y estoy estudiando [tema].
Explícamelo con un ejemplo práctico y después hazme [n] preguntas para comprobar si lo he entendido.
No me des las respuestas hasta que conteste.
```

## 5. Generación de imágenes
```
[Sujeto principal] en [entorno], [acción o pose], estilo [fotografía / ilustración / 3D / acuarela], iluminación [tipo], composición [plano], paleta de colores [colores], formato [proporción]. Sin texto ni marcas de agua.
```

## 6. System prompt para un asistente o agente
```
# Rol
Eres [nombre/función] de [empresa o proyecto].

# Objetivo
[Qué debe lograr y para quién].

# Cómo debes comportarte
- Tono: [tono].
- Si no sabes algo: [pide aclaración / indícalo, no inventes].
- Fuera de tu ámbito: [cómo responder].

# Herramientas disponibles
[Lista y cuándo usar cada una].

# Formato de respuesta
[Estructura y longitud].
```

## 7. Extracción de datos en formato estructurado
```
Extrae del texto los siguientes campos y devuelve únicamente un JSON válido, sin explicaciones:
{ "campo1": "", "campo2": "", "campo3": "" }
Si un dato no aparece, usa null. No inventes valores.
<texto>
[PEGA AQUÍ EL TEXTO]
</texto>
```
