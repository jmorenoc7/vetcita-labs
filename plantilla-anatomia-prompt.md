# Plantilla — Anatomía de un prompt de diseño

> Lab 01 · Sesión 1 · Caso VetCita. Úsala para las tres interfaces (landing page, dashboard, mobile app), para corregir los 3 prompts defectuosos y para el prompt base. La práctica la reutiliza con tu proyecto final.
> Combina lo que recomiendan las guías oficiales de Google para Stitch (idea, tema, contenido, referencia) y de Anthropic para Claude Design (objetivo, layout, contenido, audiencia; contexto y el porqué; restricciones explícitas).
> Fuentes: documentación oficial de Google Stitch, páginas *Overview* y *Effective Prompting* (https://stitch.google.com/docs); Anthropic, *Prompting best practices* (https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices); Claude Help Center, *Get started with Claude Design* (https://support.claude.com/en/articles/14604416-get-started-with-claude-design).

## Cómo usarla
1. Llena cada bloque en una o dos líneas. Si un bloque queda vacío, la herramienta lo rellena con patrones genéricos.
2. Une los bloques en un solo texto, en el orden de la tabla. No hace falta poner los nombres de los bloques en el prompt final, pero ayudan a ver qué cambiaste.
3. Para comparar variantes, **cambia un solo bloque por vez** y deja el resto palabra por palabra. Así sabes qué produjo cada diferencia. (Única excepción en el lab: el par de la landing, que compara un prompt vago con la anatomía completa y mide el efecto conjunto.)

## Los 7 bloques

| # | Bloque | Pregunta que responde | De dónde sale | Error típico si falta |
|---|---|---|---|---|
| 1 | **Idea** | ¿Qué es y en qué formato? (landing page, dashboard o mobile app; Web o App) | Stitch *Overview*: "idea" | La herramienta elige el tipo de pantalla por ti |
| 2 | **Objetivo y audiencia** | ¿Quién lo usa, qué tiene que lograr y por qué importa? | Claude Design: objetivo y audiencia; Anthropic: dar contexto y el porqué | Pantalla "bonita" que no sirve a nadie en concreto |
| 3 | **Contenido** | ¿Qué secciones, datos o elementos debe tener la pantalla? | Stitch: "contenido"; Claude Design: contenido | Secciones de relleno y textos genéricos |
| 4 | **Layout** | ¿Cómo se organiza? Usa vocabulario UI estándar: *navigation bar*, *call-to-action button*, *card layout*, *hero*, *sidebar*, *bottom navigation* | Claude Design: layout; Stitch *Effective Prompting*: vocabulario UI/UX | Estructura predecible o difícil de usar |
| 5 | **Tema (vibe)** | ¿Qué sensación transmite? 2–3 adjetivos o un estado de ánimo ("cálido y confiable", "minimalista y enfocado") | Stitch: "tema"; los adjetivos influyen en colores, fuentes e imágenes | Estética genérica de "plantilla de IA" |
| 6 | **Referencia** (opcional) | ¿Hay una imagen, captura o boceto que oriente el resultado? | Stitch: imagen de referencia opcional; Claude Design: adjuntar capturas como contexto | — (opcional) |
| 7 | **Restricciones y extras** | Idioma del texto, qué evitar, qué pedir de forma explícita (estados, datos ficticios) | Anthropic: especificar formato y restricciones; pedir explícitamente lo "extra" | Texto en otro idioma, datos inventados que parecen reales |

## Reglas rápidas (de las guías oficiales)
- **Al inicio, no fijes códigos hex ni fuentes** concretas: limitan la exploración (Stitch *Overview*). Usa adjetivos en el bloque Tema.
- **Pide lo que no quieres ver:** Anthropic recomienda evitar degradados morados sobre fondo blanco y layouts predecibles; nombrar lo que se evita orienta al modelo.
- **Datos de ejemplo ficticios y marcados como tales.** Claude puede inventar precios o cifras; revísalos siempre.
- **Iterar sin destruir:** en las rondas de ajuste, una pantalla o un componente por prompt, con una o dos modificaciones, nombrando el elemento con precisión ("el botón primario del formulario de registro", no "el botón").
- **Prueba del colega:** si un colega sin contexto se confundiría al leer tu prompt, la herramienta también.

## Plantilla en blanco (copia y llena)

```text
[1 Idea]          <tipo de interfaz> para <nombre del producto>, <qué hace en una frase>.
[2 Objetivo]      Objetivo: <qué debe lograr el usuario en esta pantalla>. Audiencia: <quién, contexto de uso>. Importa porque <motivo de negocio>.
[3 Contenido]     Contenido: <sección o elemento 1>; <sección o elemento 2>; <sección o elemento 3>; <...>.
[4 Layout]        Layout: <estructura con vocabulario UI: navigation bar, hero, card layout, sidebar, bottom navigation...>.
[5 Tema]          Tema: <adjetivo 1>, <adjetivo 2> y <adjetivo 3>. Evita <lo que no quieres: p. ej. degradados morados, tres tarjetas iguales>.
[6 Referencia]    (Opcional) Usa la imagen adjunta como referencia de <qué aspecto: estructura, tono, densidad>.
[7 Restricciones] Todo el texto de la interfaz en español. Datos de ejemplo ficticios. <otra restricción>.
```

## Plantilla de prompt de iteración (para rondas de ajuste)

```text
En la pantalla <nombre de la pantalla>, cambia <elemento preciso> para que <cambio visual concreto>.
Mantén sin cambios <lo que debe conservarse: layout, contenido, navegación...>.
<Si cambias colores: indica si imágenes e íconos deben acompañar el cambio.>
```
