# Guía de mantenimiento — Wiki de microrrobótica

Este vault es una base de conocimiento incremental. La persona aporta y selecciona las fuentes; el agente mantiene la wiki.

## Capas

- `raw/`: fuentes originales. Son inmutables: **nunca edites, renombres ni elimines** sus archivos.
- `wiki/`: conocimiento elaborado. Aquí se crean y actualizan las notas Markdown.
- `AGENTS.md`: estas reglas de operación.

## Al incorporar una fuente

1. Lee la fuente de `raw/` y conserva su nombre de archivo.
2. Crea una nota breve en `wiki/fuentes/` con el título, enlace o ruta, fecha de incorporación, resumen, hallazgos, límites y enlaces internos relevantes.
3. Actualiza las notas existentes de conceptos, componentes o aplicaciones que resulten afectadas. Crea una nota nueva solo si el tema justifica reutilización futura.
4. Actualiza `wiki/indice.md` y agrega una entrada al final de `wiki/registro.md`.
5. Señala de forma explícita cualquier contradicción, incertidumbre o dato pendiente de verificar.

## Convenciones de las notas

- Escribe en español, salvo términos técnicos establecidos.
- Usa títulos claros y enlaces Obsidian: `[[Nombre de la nota]]`.
- Mantén las notas concisas y orientadas a una idea; evita duplicar texto entre ellas.
- Cuando una afirmación provenga de una fuente, enlaza la nota correspondiente en `wiki/fuentes/`.
- Para notas nuevas, usa este frontmatter mínimo:

```yaml
---
tipo: concepto
estado: borrador
actualizado: AAAA-MM-DD
fuentes: []
---
```

## Consultas y revisión

- Antes de responder una consulta, empieza por `wiki/indice.md`, después lee las notas enlazadas y cita las fuentes disponibles.
- Si una respuesta produce una comparación, síntesis o decisión reutilizable, guárdala en `wiki/analisis/` y enlázala desde el índice.
- En una revisión periódica, busca enlaces rotos, notas sin enlaces, contradicciones, conceptos citados sin nota propia y páginas desactualizadas.
