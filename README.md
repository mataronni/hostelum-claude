# Hostelum para Claude

Consulta tu hotel desde Claude con los datos de tu panel de Hostelum. Solo consulta: no cambia reservas, precios ni cobros.

## Qué incluye

| Orden | Qué hace |
|---|---|
| `/hostelum:parte-del-dia` | Llegadas, salidas, ocupación, check-in online pendiente, mantenimiento y cocina del día. |
| `/hostelum:cobros-pendientes` | Reservas con importe pendiente de cobro, ordenadas por urgencia. |
| `/hostelum:revision-de-precios` | Noches en las que conviene mirar el precio: competencia, ocupación, festivos y riesgo de sobreventa. |
| `/hostelum:informe-del-mes` | Cifras del mes comparadas con el mes anterior y con el año pasado. |

También puedes pedirlo con tus palabras: «dame el parte de hoy», «qué me queda por cobrar», «revisa los precios de diciembre».

Incluye la conexión con Hostelum (`https://panel.hostelum.com/mcp`). La primera vez, Claude te pedirá entrar con tu usuario del panel y autorizar el acceso. Verás lo mismo que ese usuario puede ver en el panel.

## Requisitos

- Un usuario del panel de Hostelum.
- El acceso desde IA activado en tu alojamiento.

## Instalación

En Claude Code:

```
/plugin marketplace add mataronni/hostelum-claude
/plugin install hostelum@hostelum
```

En Claude (web y escritorio): Personalizar › Plugins › Añadir, y después conecta «Hostelum» en Conectores.

## Ayuda

- Documentación de la conexión: https://panel.hostelum.com/mcp/ayuda
- Soporte: hola@hostelum.com

© WOWTECH SL
