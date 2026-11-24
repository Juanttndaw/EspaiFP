
# Registro de pruebas – EspaiFP

Este documento recoge los casos de prueba previstos para comprobar el funcionamiento de las principales funcionalidades de EspaiFP.

Las pruebas se realizarán progresivamente durante el desarrollo. Cada caso incluirá los pasos necesarios, el resultado esperado, el resultado obtenido y su estado.

En el momento de preparar este registro, las pruebas todavía no se han ejecutado, ya que las funcionalidades correspondientes están pendientes de implementación.

## 1. Estados de las pruebas

Se utilizarán los siguientes estados:

- **Pendiente:** la prueba todavía no se ha ejecutado.
- **Superada:** el resultado obtenido coincide con el resultado esperado.
- **Fallida:** el resultado obtenido no coincide con el esperado y requiere una corrección.

## 2. Casos de prueba previstos

### PR-01. Creación de una reserva

| Campo | Información |
|---|---|
| Identificador | PR-01 |
| Requisito relacionado | RF-04. Gestión de reservas |
| Funcionalidad | Creación de reservas |
| Procedimiento | Iniciar sesión como profesor, seleccionar un aula disponible, indicar una fecha y un horario válidos y confirmar la reserva. |
| Resultado esperado | La aplicación registra correctamente la reserva y muestra su información. |
| Resultado obtenido | Sin ejecutar. |
| Estado | Pendiente |

### PR-02. Prevención de reservas incompatibles

| Campo | Información |
|---|---|
| Identificador | PR-02 |
| Requisito relacionado | RF-08 y RF-09. Control de disponibilidad y prevención de solapamientos |
| Funcionalidad | Comprobación de disponibilidad |
| Procedimiento | Crear una reserva para un aula y horario determinados e intentar registrar otra reserva para la misma aula en una franja horaria coincidente. |
| Resultado esperado | La aplicación rechaza la segunda reserva e informa de que el aula no está disponible en ese horario. |
| Resultado obtenido | Sin ejecutar. |
| Estado | Pendiente |

### PR-03. Modificación de una reserva

| Campo | Información |
|---|---|
| Identificador | PR-03 |
| Requisito relacionado | RF-06. Modificación y eliminación de reservas |
| Funcionalidad | Modificación de reservas |
| Procedimiento | Iniciar sesión, seleccionar una reserva existente, modificar alguno de sus datos permitidos y guardar los cambios. |
| Resultado esperado | La reserva se actualiza correctamente y muestra la nueva información sin perder los datos necesarios. |
| Resultado obtenido | Sin ejecutar. |
| Estado | Pendiente |

## 3. Registro de ejecución

Cuando se realice una prueba, se actualizará su resultado en este documento.

También se podrán añadir la fecha de ejecución, las observaciones y la ubicación de las evidencias, como capturas de pantalla o registros de funcionamiento.

| ID | Fecha de ejecución | Resultado | Estado | Observaciones |
|---|---|---|---|---|
| PR-01 | Pendiente | Sin ejecutar | Pendiente | Se realizará cuando esté implementada la gestión de reservas. |
| PR-02 | Pendiente | Sin ejecutar | Pendiente | Se realizará cuando esté implementado el control de disponibilidad. |
| PR-03 | Pendiente | Sin ejecutar | Pendiente | Se realizará cuando esté disponible la modificación de reservas. |

## 4. Gestión de pruebas fallidas

Cuando una prueba falle, se analizará la causa del problema y se registrará una incidencia en GitHub Issues si corresponde.

Después de aplicar la corrección se repetirá la prueba para comprobar que el problema ha desaparecido.

La prueba solamente cambiará a estado **Superada** cuando se obtenga el resultado esperado. Si el problema continúa, permanecerá como **Fallida** hasta que se resuelva.

Este registro se actualizará durante el desarrollo de EspaiFP y permitirá conservar un historial de las comprobaciones realizadas.
