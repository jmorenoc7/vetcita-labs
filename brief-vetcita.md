# Brief de reingeniería — VetCita

> Entrada dada del lab 01 (caso común, ficticio). Lo usas en el paso 6 para escribir el prompt base de VetCita y lo vuelve a recibir el lab 02. **No lo modifiques.**
> Los datos simulados y el vocabulario del caso están en `ficha-vetcita.md`.

## Producto actual
- Qué hace hoy: web app para reservar clases grupales en un gimnasio y ver el historial de asistencia.
- Para quién se hizo: socios y recepción de un gimnasio de barrio.
- Pantallas que existen hoy: login, calendario de clases, detalle de clase, mis reservas, panel de recepción.

## Industria destino
- Red de clínicas veterinarias con varias sedes.
- Se reaprovecha: calendario, reservas con cupo, panel de recepción, historial.
- Qué cambia: la cita es individual, con un veterinario y en una sede; cada servicio tiene una duración distinta que ocupa la agenda; una cita pasa por los estados Pendiente, Confirmada y Reprogramada.

## Usuarias
- Principal: recepcionista de una sede. Agenda, confirma y reprograma citas en la computadora de recepción, con el cliente delante o al teléfono, y usa el celular cuando atiende fuera del mostrador.
- Secundaria: administradora de la red. Desde su laptop revisa la ocupación y las citas sin confirmar de todas las sedes.

## Tareas y pantallas clave

| # | Tarea (verbo + objeto) | Pantalla | ¿Existe hoy? |
|---|---|---|---|
| 1 | Registrar una cita nueva | Nueva cita | Adaptada (hoy: reservar clase) |
| 2 | Ver la agenda del día por veterinario | Agenda del día | Adaptada (hoy: calendario) |
| 3 | Reprogramar una cita | Detalle de cita (acción principal: Reprogramar) | Adaptada (hoy: detalle de clase) |
| 4 | Revisar la ocupación por sede | Dashboard de la red | Nueva |

## Restricciones
- Solo datos simulados: los de `ficha-vetcita.md`. Donde falte un precio, "precio por confirmar".
- Tipo de proyecto principal: Web, usable también en el celular.
- Interfaz en español.
- Tema: cálido, confiable y ordenado. Evitar degradados morados, tres tarjetas iguales con ícono y fotos de stock de oficina.
- No cambia: la navegación lateral del panel de recepción. En VetCita es una sidebar izquierda con Agenda, Nueva cita, Clientes, Mascotas y Reportes, con selector de sede en el encabezado. El Dashboard de la red solo lo ve la administradora.
