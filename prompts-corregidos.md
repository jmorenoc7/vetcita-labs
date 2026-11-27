# Prompts corregidos — Lab 01 · VetCita — <tu nombre>

> Paso 5 del lab (15 min). **No generes nada:** se corrige por escrito, con la plantilla de anatomía y la plantilla de iteración (`plantilla-anatomia-prompt.md`).
> Los tres prompts los escribió el equipo de VetCita. Cada uno tiene fallos distintos. Contexto y datos simulados: `ficha-vetcita.md`.
> Los prompts corregidos forman parte de la salida del lab 01 y de la evidencia de tus reglas (sección D de la hoja de registro). El lab 02 parte del prompt base y del brief.

---

## A · Un prompt sin audiencia ni contenido produce una app genérica (4 min)

Primer prompt para Stitch:

```text
Hazme una app moderna y bonita para una veterinaria.
```

**A1. Diagnóstico (1 min).** Marca los bloques que faltan o están mal resueltos y di qué produce cada hueco.

| Bloque | ¿Falta o débil? | Qué produce |
|---|---|---|
| 1 Idea | | |
| 2 Objetivo y audiencia | | |
| 3 Contenido | | |
| 4 Layout | | |
| 5 Tema | | |
| 7 Restricciones y extras | | |

**A2. Prompt corregido (3 min).** Reescríbelo para **una sola pantalla**: **"Detalle de cita"**, la que abre la recepcionista desde la agenda para revisar una cita y reprogramarla cuando el cliente llama. Usa el vocabulario de la ficha (estados de cita, acción principal).

```text

```

---

## B · Cinco cambios en un prompt destruyen el diseño (5 min)

**Contexto:** en Stitch ya existe un **Dashboard** web aceptable para la administradora de la red. Lo generó un compañero: tiene navigation bar superior, cuatro tarjetas de KPI, una tabla de citas del día y un botón "Nueva cita" en el encabezado. La administradora pide:

```text
Está bien pero cámbialo todo a modo oscuro, pasa el menú a la izquierda,
agrega gráficos de citas por sede, pon el botón en verde y que se vea
más profesional.
```

**B1. Diagnóstico (1 min).** En dos líneas: por qué pone en riesgo el diseño existente y cuáles son los **dos** tipos de error que contiene.

-
-

**B2. Secuencia corregida (4 min).** Reescríbelo como una **secuencia numerada de 3 a 5 prompts** con la plantilla de iteración: cada uno nombra la pantalla y el elemento con precisión, hace uno o dos cambios y dice qué se mantiene. Decide qué haces con "que se vea más profesional" y justifícalo en una línea.

```text
1.
2.
3.
```

Qué hice con "más profesional":

---

## C · Sin estados ni datos dados, el prototipo engaña (6 min)

**Contexto:** el equipo usa Claude Design **dentro de Claude** para prototipar el flujo con el que la recepcionista registra una cita nueva. Este es el primer prompt:

```text
Diseña el flujo para registrar una cita en VetCita: elegir servicio con
sus precios, elegir horario y confirmar. Usa un degradado morado sobre
fondo blanco y la fuente Inter, que se vea moderno.
```

**C1. Diagnóstico (2 min).** Encuentra **tres** fallos distintos de los de A y B. Pistas: qué verá quien lo implemente cuando algo salga mal; qué datos aparecerán en pantalla (mira tu sección C de la hoja de registro); qué dice la plantilla sobre el tema en un primer prompt.

| Fallo | Por qué es un problema | Bloque que lo corrige |
|---|---|---|
| | | |
| | | |
| | | |

**C2. Prompt corregido (4 min).** Reescríbelo con los bloques de la plantilla. Usa los datos simulados de `ficha-vetcita.md`.

```text

```
