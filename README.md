# redactor-prompts

Skill para Claude que **redacta, mejora y optimiza prompts de IA**. Convierte una idea en un prompt claro, estructurado y listo para copiar, o corrige uno que no te está dando buenos resultados.

## Qué hace

- Crea prompts desde cero a partir de lo que necesitas conseguir.
- Mejora prompts existentes, explicando qué fallaba y qué ha cambiado.
- Adapta el prompt a la herramienta: chat, generadores de imágenes, agentes, system prompts o API.
- Entrega el resultado en un bloque de código, con notas breves y variantes si las pides.
- Incluye plantillas para redacción, resumen, código, estudio, imágenes, system prompts y extracción de datos.

## Cómo estructura un prompt

Rol, contexto, tarea, restricciones, formato de salida, ejemplos, criterios de calidad y datos de entrada. Solo usa las partes que aportan valor.

## Instalación

### En Claude (claude.ai)
1. Comprime la carpeta `redactor-prompts` en un `.zip`.
2. Ve a **Configuración → Capacidades → Skills** y sube el archivo.

### En Claude Code
Copia la carpeta en el directorio de skills:

```bash
# Para todos tus proyectos
cp -r redactor-prompts ~/.claude/skills/

# Solo para un proyecto
cp -r redactor-prompts .claude/skills/
```

## Uso

Basta con pedirlo con naturalidad:

- «Hazme un prompt para que la IA me corrija trabajos de clase.»
- «Mejora este prompt, no me da respuestas útiles: ...»
- «Necesito un system prompt para un asistente de atención al cliente.»
- «Escribe un prompt para generar una imagen de un coche eléctrico al amanecer.»

## Estructura

```
redactor-prompts/
├── SKILL.md                  # Instrucciones y principios de redacción
├── references/
│   └── plantillas.md         # Plantillas por tipo de tarea
├── LICENSE
└── README.md
```

## Licencia

Distribuida bajo licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

© 2026 Alejandro Gutiérrez
