
# Registro de cambios – EspaiFP

Este documento recoge las modificaciones propuestas durante el desarrollo de EspaiFP. Su finalidad es analizar el impacto de cada cambio antes de incorporarlo al proyecto y conservar un historial de las decisiones adoptadas.

## 1. Procedimiento de gestión

Cuando se proponga una modificación, se registrará utilizando un identificador propio y se describirán sus motivos.

Antes de aprobarla se analizarán los siguientes aspectos:

- **Funcionalidades:** partes de la aplicación que pueden verse afectadas.
- **Tareas:** actividades de la planificación que será necesario modificar.
- **Recursos:** herramientas, servicios o materiales adicionales.
- **Tiempo:** esfuerzo adicional y posibles retrasos respecto al cronograma.
- **Costes:** posibles gastos adicionales.
- **Documentación:** archivos y requisitos que deberán actualizarse.

## 2. Decisiones sobre los cambios

Después de analizar la propuesta se adoptará una de estas decisiones:

| Decisión | Descripción |
|---|---|
| Aprobado | El cambio es viable y aporta una mejora al proyecto. |
| Aplazado | El cambio puede ser útil, pero se pospone para una fase posterior. |
| Rechazado | El cambio no resulta necesario o puede perjudicar los objetivos y la planificación. |

Al tratarse de un proyecto individual, el alumno será responsable de valorar las propuestas y documentar las decisiones. Si una modificación afecta de forma importante al alcance o a las condiciones académicas, se consultará con el profesor responsable.

## 3. Plantilla de registro de cambios

Cada modificación importante se documentará con los siguientes datos:

| Campo | Información |
|---|---|
| Identificador | Código único del cambio, por ejemplo CAM-01. |
| Descripción y motivo | Explicación de la modificación y por qué se propone. |
| Impacto en tareas | Actividades de la planificación que se verán afectadas. |
| Impacto en recursos | Nuevas herramientas o recursos necesarios. |
| Impacto en planificación | Tiempo adicional y posibles cambios en las fechas. |
| Impacto económico | Posibles costes adicionales. |
| Decisión adoptada | Aprobado, aplazado o rechazado. |
| Fecha y responsable | Fecha de registro y persona que toma la decisión. |
| Documentos que actualizar | Archivos, requisitos o pruebas que deberán modificarse. |

## 4. Ejemplo simulado de cambio

El siguiente ejemplo es hipotético y sirve únicamente para mostrar cómo se utilizará el registro. No representa una modificación aprobada o realizada en el proyecto.

**Identificador:** CAM-SIM-01

**Descripción:** Incorporar notificaciones por correo electrónico cuando se confirme una reserva.

**Motivo:** Facilitar que el profesorado reciba información sobre el resultado de sus solicitudes.

**Impacto en tareas:** Podrían verse afectadas T10 (gestión de reservas), T13 (integración del frontend), T14 (validaciones), T15 (pruebas) y T17 (documentación).

**Impacto en recursos:** Sería necesario utilizar y configurar un servicio de envío de correo electrónico.

**Impacto en planificación:** Se necesitarían horas adicionales para implementar y comprobar esta funcionalidad.

**Impacto económico:** Habría que comprobar si el servicio elegido tiene algún coste.

**Decisión adoptada:** Aplazado. Se dará prioridad a las funcionalidades esenciales definidas inicialmente.

**Responsable:** Juan Antonio Torregrosa Maciá.

**Documentación que habría que actualizar:** requisitos, planificación, indicadores de calidad y registro de pruebas.

Este ejemplo no supone que la funcionalidad vaya a incorporarse finalmente a EspaiFP.

## 5. Actualización y conservación

El registro se actualizará cuando aparezcan propuestas de modificación que puedan afectar al alcance, las funcionalidades, los recursos o la planificación del proyecto.

Cuando se apruebe un cambio, se actualizarán los documentos correspondientes y las tareas afectadas en GitHub Projects.

Los cambios realizados en el código y la documentación se conservarán en GitHub mediante commits descriptivos, de forma que sea posible consultar su historial.

Este procedimiento permitirá justificar las decisiones tomadas y mantener un control organizado de la evolución de EspaiFP.
