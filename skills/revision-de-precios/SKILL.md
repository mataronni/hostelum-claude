---
name: revision-de-precios
description: "Revisión de precios del hotel con los datos de Hostelum: precios propios frente a la competencia, ocupación, festivos, restricciones y riesgo de sobreventa de los próximos días. Úsalo cuando pidan «revisa los precios», «cómo voy de precio», «qué fechas debería tocar» o una revisión de un periodo concreto."
---

# Revisión de precios

Señala en qué noches conviene mirar el precio y por qué. Usa solo las herramientas del conector de Hostelum; no cambies precios ni restricciones: el cambio lo hace la persona en su panel.

## Antes de empezar

- Periodo: el que pida la persona. Si no dice ninguno, los próximos 30 días. El máximo por consulta son 62 noches.
- Alojamiento: si nombra uno, ese. Si hay varios y no dice cuál, llama a `alojamientos` y pregunta: esta revisión se hace alojamiento por alojamiento.
- Tarifa: si no dice ninguna, la de referencia.

## Datos que hay que pedir

1. `ocupacion`: ocupación y habitaciones libres por noche.
2. `precios_competencia`: precio propio, mediana de la competencia, diferencia y precio sugerido.
3. `ver_precios`: precio de cada tarifa por noche.
4. `festivos`: festivos y eventos del periodo.
5. `restricciones`: estancia mínima, cierres y venta cerrada.
6. `riesgo_overbooking`, con los días del periodo: noches con más reservas que habitaciones y avisos de canales.

## Cómo presentarlo

- **Resumen**, en dos o tres líneas: cómo está el periodo en conjunto.
- **Noches a revisar**: tabla con fecha, ocupación, precio propio, mediana de la competencia, diferencia y motivo. Incluye solo las noches que cumplan alguno de estos casos:
  - ocupación alta y precio por debajo de la competencia;
  - ocupación baja y precio por encima de la competencia;
  - festivo o evento con el precio de un día normal;
  - una restricción que puede estar frenando la venta (estancia mínima o cierre en noches con poca ocupación);
  - riesgo de sobreventa.
- **Avisos**: sobreventa y disponibilidad pendiente de enviar a los canales, si los hay.
- **Sin datos**: noches para las que no hay precios de la competencia guardados.

## Reglas

- Las noches sin datos de la competencia no se comparan; no estimes su valor.
- El precio sugerido que llega del conector se muestra como dato del panel, no como recomendación tuya.
- Explica cada motivo con las cifras que lo sostienen. No des una subida o bajada en euros que no salga de los datos.
- No inventes datos. Si una herramienta falla, dilo y sigue con el resto.
