# Formatos de salida (cuando no hay herramienta de quiz interactivo)

## Test en Markdown

Presenta primero **solo las preguntas**, sin soluciones, para que el usuario pueda responder. Numera las preguntas y etiqueta las opciones con A, B, C y D.

```
# Test: <tema> (<n> preguntas)

**1.** Enunciado
- A) ...
- B) ...
- C) ...
- D) ...

**2.** ...

Responde con el formato `1B, 2A, 3D...` y te lo corrijo.
```

No muestres las respuestas hasta que el usuario conteste o las pida.

## Solucionario

```
## Solucionario
| Nº | Correcta | Explicación |
|----|----------|-------------|
| 1  | B        | ...         |
```

## Entrega como archivo

Solo si el usuario pide un archivo (PDF, Word, etc.), usa la skill correspondiente. Para un PDF imprimible, pon el test en las primeras páginas y el solucionario en una página aparte al final.

## Flashcards en Markdown

```
**P:** Pregunta
**R:** Respuesta (explicación breve)
```
