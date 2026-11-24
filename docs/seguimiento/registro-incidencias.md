
# Registro de incidencias – EspaiFP

Este documento establece cómo se registrarán y organizarán los errores o problemas detectados durante el desarrollo de EspaiFP.

Las incidencias se gestionarán preferentemente mediante GitHub Issues, que permitirá describir los problemas, asignarles una prioridad, consultar su estado y conservar un historial de las soluciones aplicadas.

## 1. Clasificación de las incidencias

Se utilizarán cuatro niveles de prioridad:

| Prioridad | Descripción |
|---|---|
| Crítica | Problemas graves de seguridad, pérdida de datos o fallos que comprometan el funcionamiento general. |
| Alta | Errores que impiden utilizar una funcionalidad esencial, como iniciar sesión o gestionar reservas. |
| Media | Problemas que afectan a una funcionalidad, pero permiten continuar utilizando otras partes de la aplicación. |
| Baja | Errores visuales o detalles menores que no impiden utilizar la aplicación. |

## 2. Estados de las incidencias

- **Abierta:** el problema está registrado y pendiente de solución.
- **En curso:** se está investigando o corrigiendo.
- **En revisión:** se ha aplicado una posible solución y falta comprobarla.
- **Cerrada:** el problema se ha corregido y se ha verificado su solución.

Los estados intermedios también se podrán controlar mediante el tablero de GitHub Projects.

## 3. Plantilla para registrar incidencias

Cada incidencia deberá incluir la siguiente información:

| Campo | Información que debe incluir |
|---|---|
| Identificador | Número de la incidencia en GitHub Issues. |
| Título | Nombre breve que describa el problema. |
| Descripción | Explicación de lo que ocurre y dónde sucede. |
| Pasos para reproducir | Acciones necesarias para provocar el problema. |
| Resultado esperado | Comportamiento que debería producirse. |
| Resultado obtenido | Comportamiento que se produce realmente. |
| Prioridad | Crítica, alta, media o baja. |
| Estado | Abierta, en curso, en revisión o cerrada. |
| Solución aplicada | Descripción de la corrección realizada. |
| Comprobación posterior | Prueba realizada para verificar que el problema está resuelto. |

Cuando sea posible, se adjuntarán capturas de pantalla o mensajes de error que ayuden a identificar el problema. No se incluirán contraseñas ni datos personales reales.

## 4. Ejemplo simulado de incidencia

El siguiente ejemplo es ficticio y se incluye únicamente para mostrar cómo se utilizará el registro. No representa un error real detectado en EspaiFP.

**Identificador:** INC-SIM-01

**Título:** Posibilidad de registrar dos reservas incompatibles.

**Descripción:** Se plantea un posible error por el que la aplicación permitiría registrar dos reservas para la misma aula y horario.

**Pasos para reproducir:**
1. Seleccionar un aula y un horario.
2. Registrar una primera reserva.
3. Intentar registrar otra reserva para la misma aula y horario.

**Resultado esperado:** La aplicación debe rechazar la segunda reserva e informar del conflicto.

**Resultado obtenido:** En este ejemplo simulado, se supone que la aplicación permitiría guardar la segunda reserva.

**Prioridad:** Alta.

**Estado:** Abierta (simulada).

**Solución prevista:** Incorporar una comprobación de disponibilidad en el servidor antes de guardar la reserva.

**Comprobación posterior prevista:** Repetir la prueba con dos reservas coincidentes y verificar que la segunda es rechazada.

La solución y la comprobación quedan pendientes en este ejemplo hipotético.

## 5. Actualización y cierre

Cuando se detecte una incidencia real, se creará una nueva entrada en GitHub Issues utilizando la información de la plantilla.

Durante su resolución se actualizará el estado y se documentarán los cambios realizados. Cuando se aplique una solución, se repetirá la operación que provocó el error.

La incidencia solamente se cerrará cuando se haya comprobado que el problema está resuelto y que la funcionalidad se comporta como se esperaba.

Este procedimiento permitirá mantener un historial organizado de los problemas y las correcciones realizadas durante el desarrollo de EspaiFP.
