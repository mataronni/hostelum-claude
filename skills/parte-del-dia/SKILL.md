---
name: parte-del-dia
description: "Parte del día del hotel con los datos de Hostelum: llegadas, salidas, ocupación, check-in online pendiente, mantenimiento abierto y servicios de cocina. Úsalo cuando pidan «el parte de hoy», «qué tenemos hoy», «cómo está el día» o el parte de otra fecha."
---

# Parte del día

Prepara un parte breve para quien abre la recepción. Usa solo las herramientas del conector de Hostelum; no modifiques nada.

## Antes de empezar

- Fecha: la que pida la persona. Si no dice ninguna, hoy.
- Alojamiento: si nombra uno, ese. Si no, deja el campo vacío: el conector usa el único que tenga o el conjunto del grupo. Si hay varios y no queda claro cuál quiere, llama a `alojamientos` y pregunta.

## Datos que hay que pedir

Para la fecha elegida:

1. `llegadas`: reservas que entran.
2. `salidas`: reservas que se van.
3. `ocupacion`, con «desde» y «hasta» en esa misma fecha: ocupación y habitaciones libres por tipo.
4. `checkin_online_pendiente`: qué llegadas tienen el check-in online hecho y cuáles no.
5. `mantenimiento`: tareas abiertas, las urgentes primero.
6. `cocina_servicios`, con «desde» en esa fecha: desayunos, comidas, cenas y extras.

## Cómo presentarlo

Una página, en este orden:

- **Resumen**, en una línea: llegadas, salidas, ocupación y habitaciones libres.
- **Llegadas**: tabla con huésped, tipo de habitación, salida y estado del check-in online. Señala las que no lo tienen hecho.
- **Salidas**: lista corta.
- **Cocina y extras**: cantidades del día.
- **Mantenimiento**: solo las tareas urgentes y las que afectan a una habitación con llegada hoy; del resto, el número.
- **A vigilar**: como mucho tres puntos concretos, sacados de los datos.

## Reglas

- Escribe en el idioma en que te hablen; por defecto, en castellano.
- No inventes datos. Si una herramienta falla o un bloque no está disponible para ese usuario, dilo en una línea y sigue con el resto.
- Muestra los nombres de huésped tal como llegan, con sus asteriscos; no intentes completarlos.
- Si un apartado no tiene nada, ponlo en una línea («Sin salidas hoy») en lugar de omitirlo.
