# Ficha de VetCita — caso común de los labs

> Entrada dada del lab 01. **No la modifiques:** es la misma para todo el curso y la usan también los labs siguientes.
> VetCita es **ficticio**. Todos los nombres, sedes y precios de esta ficha son datos simulados.

## El caso en una línea
Un equipo adapta una web app de **reservas de clases de gimnasio** a una **red de clínicas veterinarias** con varias sedes. El producto adaptado se llama **VetCita**.

## Ficha de contexto

| Campo | Valor |
|---|---|
| Producto actual | Web app para reservar clases grupales en un gimnasio y ver el historial de asistencia. |
| Industria destino | Red de clínicas veterinarias con varias sedes. |
| Producto adaptado | **VetCita**: agenda, registro y seguimiento de citas veterinarias. |
| Tipo de producto | **Web**, usada en la computadora de recepción. La recepcionista también usa el celular cuando atiende fuera del mostrador. |
| Usuaria principal | **La recepcionista de una sede.** Agenda, confirma y reprograma citas en la computadora de recepción, con el cliente delante o al teléfono y con interrupciones constantes. Fuera del mostrador (sala de espera, consultorios) usa el celular, de pie y con poco tiempo. |
| Usuaria que supervisa | **La administradora de la red.** Desde su laptop revisa al empezar el día la ocupación y las citas sin confirmar de todas las sedes, y reasigna personal. |
| Tarea clave n.º 1 | Agendar una cita nueva. |
| Otras tareas clave | Ver la agenda del día; reprogramar una cita; supervisar la ocupación de la red. |
| Tema (3 adjetivos) | Cálido, confiable y ordenado. |
| Qué evitar visualmente | Degradados morados, tres tarjetas iguales con ícono, fotos de stock genéricas de personas en una oficina. |

## Vocabulario del caso (úsalo tal cual en los prompts)

| Elemento | Valor |
|---|---|
| Pantallas | **Agenda del día**, **Nueva cita**, **Detalle de cita**, **Dashboard de la red** (solo la administradora). |
| Navegación de la web app | Sidebar izquierda con **Agenda, Nueva cita, Clientes, Mascotas y Reportes**; encabezado con **selector de sede**. |
| Estados de una cita | **Pendiente**, **Confirmada**, **Reprogramada**. |
| Acción principal del Detalle de cita | **Reprogramar**. |

## Datos simulados (los únicos que se dan a las herramientas)

| Tipo | Datos |
|---|---|
| Sedes | Sede Centro, Sede Norte. |
| Servicios (duración y precio simulado) | Consulta general, 30 min, S/ 60 · Vacunación, 15 min, S/ 45 · Baño y corte, 60 min, S/ 50. |
| Veterinarios | Dra. Paredes, Dr. Quispe, Dra. Salinas. |
| Clientes y mascotas | Ana Torres con Luna (perra, 4 años) · Jorge Díaz con Michi (gato, 2 años). |

Si una herramienta muestra un dato que no está en esta tabla (otro precio, otra sede, testimonios con nombre), es un **dato inventado**: anótalo en la sección C de la hoja de registro.
