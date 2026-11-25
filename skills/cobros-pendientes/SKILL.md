---
name: cobros-pendientes
description: "Reservas con importe pendiente de cobro según Hostelum, ordenadas por urgencia, con el total que falta por cobrar. Úsalo cuando pregunten «qué me deben», «qué queda por cobrar», «cobros pendientes» o quieran repasar los cobros de unas fechas."
---

# Cobros pendientes

Prepara la lista de lo que falta por cobrar. Usa solo las herramientas del conector de Hostelum; no modifiques nada ni cobres nada.

## Antes de empezar

- Periodo: el que pida la persona, por fecha de llegada. Si no dice ninguno, desde hace 30 días hasta dentro de 30. El máximo por consulta son 62 días; si piden más, hazlo en tramos y súmalos.
- Alojamiento: si nombra uno, ese. Si no, deja el campo vacío. Si hay varios y no queda claro, llama a `alojamientos` y pregunta.

## Datos que hay que pedir

1. `pendiente_cobro`, con «desde» y «hasta».
2. Solo si la persona quiere el detalle de una reserva concreta: `ficha_reserva`.

## Cómo presentarlo

- **Total pendiente** y número de reservas, en la primera línea.
- **Tabla** con llegada, huésped, total, cobrado y pendiente. Ordénala así:
  1. Reservas cuya llegada ya pasó y siguen con importe pendiente.
  2. Llegadas de hoy y de los próximos 7 días.
  3. El resto, por fecha de llegada.
- **Qué mirar primero**: dos o tres reservas concretas, con el motivo (importe alto, estancia ya terminada, llegada inminente sin nada cobrado).

## Reglas

- Importes en euros, con dos decimales, tal como llegan; no los recalcules.
- No inventes datos. Si la herramienta falla o el usuario no tiene acceso a facturación y cobros, dilo y no sigas.
- Muestra los nombres de huésped tal como llegan, con sus asteriscos.
- Si la respuesta trae una nota sobre cómo se calcula lo cobrado, resúmela al final. En particular: las reservas que cobra el canal salen como pendientes si el cobro no se ha apuntado en el panel; sepáralas de las directas al ordenar.
- Si no hay nada pendiente en el periodo, dilo en una línea.
- No redactes mensajes de reclamación a huéspedes salvo que te lo pidan.
