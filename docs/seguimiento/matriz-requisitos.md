
# Matriz de requisitos – EspaiFP

Este documento recoge los requisitos funcionales y no funcionales definidos en la Fase 2 del proyecto EspaiFP.

La matriz relaciona cada requisito con su criterio de aceptación, la comprobación prevista y la evidencia necesaria para verificar su cumplimiento.

Los estados se actualizarán durante el desarrollo, una vez implementadas las funcionalidades y realizadas las pruebas correspondientes.

## 1. Requisitos funcionales

| ID | Requisito | Criterio de aceptación | Comprobación prevista | Evidencia necesaria | Estado |
|---|---|---|---|---|---|
| RF-01 | Inicio de sesión | Los usuarios pueden acceder con credenciales válidas y se rechazan las incorrectas. | Probar el acceso con credenciales correctas e incorrectas. | Capturas del acceso y de los mensajes de error. | Pendiente |
| RF-02 | Control de permisos | El profesorado y el administrador acceden únicamente a las funciones de su perfil. | Probar las operaciones disponibles con ambos perfiles. | Capturas y resultados de las pruebas de permisos. | Pendiente |
| RF-03 | Consulta de aulas | El profesorado puede consultar las aulas y sus características. | Consultar el listado de aulas registradas. | Captura del listado y de la información mostrada. | Pendiente |
| RF-04 | Gestión de reservas | El profesorado puede crear reservas indicando aula, fecha y horario. | Completar el formulario con datos válidos y confirmar la reserva. | Captura del formulario y de la reserva creada. | Pendiente |
| RF-05 | Consulta de reservas | El profesor puede consultar sus reservas y el administrador puede consultar todas. | Acceder al listado con ambos perfiles. | Capturas de los listados según el perfil. | Pendiente |
| RF-06 | Modificación y eliminación | El profesorado puede modificar o cancelar sus reservas y el administrador puede gestionar todas. | Modificar y cancelar reservas con los perfiles correspondientes. | Resultados y capturas de las operaciones. | Pendiente |
| RF-07 | Gestión de recursos | El administrador puede crear, consultar, modificar y eliminar aulas. | Realizar las operaciones de gestión sobre diferentes aulas. | Capturas y registros de las operaciones. | Pendiente |
| RF-08 | Control de disponibilidad | El sistema comprueba que el aula esté disponible antes de registrar una reserva. | Intentar reservar un aula ocupada y otra libre. | Resultados de las pruebas de disponibilidad. | Pendiente |
| RF-09 | Prevención de solapamientos | No se permiten dos reservas incompatibles para la misma aula y franja horaria. | Intentar registrar dos reservas coincidentes. | Resultado de la prueba y aviso de conflicto. | Pendiente |
| RF-10 | Validación de datos | Los campos obligatorios y las fechas y horarios se validan correctamente. | Enviar formularios vacíos o con datos no válidos. | Capturas de los mensajes de validación. | Pendiente |
| RF-11 | Persistencia de datos | La información de usuarios, aulas y reservas permanece almacenada. | Crear y modificar registros y consultarlos posteriormente en MariaDB. | Consultas y resultados de la base de datos. | Pendiente |
| RF-12 | Bloqueo de espacios | El administrador puede marcar temporalmente un aula como no disponible. | Bloquear un aula e intentar reservarla posteriormente. | Captura del estado del aula y resultado de la prueba. | Pendiente |

## 2. Requisitos no funcionales

| ID | Requisito | Criterio de aceptación | Comprobación prevista | Evidencia necesaria | Estado |
|---|---|---|---|---|---|
| RNF-01 | Usabilidad | La navegación es comprensible y permite encontrar las funciones principales. | Pedir a usuarios participantes que realicen tareas habituales. | Cuestionarios y observaciones de los participantes. | Pendiente |
| RNF-02 | Adaptabilidad | La interfaz se muestra correctamente en ordenador y dispositivos móviles. | Revisar las pantallas en diferentes tamaños de pantalla. | Capturas de distintas resoluciones. | Pendiente |
| RNF-03 | Seguridad | Las contraseñas se almacenan de forma segura y se respetan los permisos de cada usuario. | Revisar el almacenamiento de contraseñas y probar los accesos. | Revisión del código y resultados de las pruebas. | Pendiente |
| RNF-04 | Fiabilidad | Las operaciones no provocan pérdidas ni alteraciones incorrectas de información. | Crear, modificar y eliminar datos y comprobar su conservación. | Resultados de las pruebas y consultas de MariaDB. | Pendiente |
| RNF-05 | Rendimiento | Las consultas y operaciones habituales responden en un tiempo adecuado, sin esperas innecesarias. | Medir los tiempos de respuesta de las operaciones principales en el entorno de pruebas. | Registro de tiempos obtenidos. | Pendiente |
| RNF-06 | Compatibilidad | La aplicación funciona correctamente en navegadores actuales como Chrome, Firefox y Edge. | Probar las pantallas y operaciones principales en los tres navegadores. | Capturas y resultados de las pruebas. | Pendiente |
| RNF-07 | Mantenibilidad | El código está organizado para facilitar futuras modificaciones y correcciones. | Revisar la estructura de archivos y la separación entre frontend y backend. | Estructura del proyecto y revisión del código. | Pendiente |
| RNF-08 | Accesibilidad | Los formularios tienen etiquetas comprensibles y permiten una navegación clara mediante teclado. | Recorrer los formularios con el teclado y revisar sus etiquetas y controles. | Registro de comprobaciones y capturas. | Pendiente |

## 3. Actualización del estado de los requisitos

Los requisitos se revisarán durante el desarrollo y las pruebas de EspaiFP.

Se utilizarán los siguientes estados:

- **Pendiente:** el requisito todavía no ha sido comprobado.
- **En revisión:** se está realizando su comprobación.
- **Cumplido:** la prueba ha obtenido el resultado esperado.
- **No cumplido:** la comprobación ha detectado problemas que necesitan corrección.

Cuando un requisito no cumpla su criterio de aceptación, se analizará el problema y se registrará una incidencia en GitHub Issues si corresponde.

Una vez aplicada la solución, se repetirá la comprobación para verificar que el requisito se cumple.

## 4. Relación con la documentación del proyecto

Esta matriz se mantendrá relacionada con los documentos de seguimiento almacenados en esta carpeta:

- `indicadores-calidad.md`: indicadores utilizados para evaluar la calidad.
- `registro-pruebas.md`: procedimientos y resultados de las pruebas.
- `registro-incidencias.md`: problemas detectados y sus soluciones.
- `seguimiento-tareas.md`: estado de las actividades de desarrollo.

La matriz se actualizará progresivamente y permitirá consultar qué requisitos se han implementado, cuáles están pendientes y cuáles necesitan correcciones.

En el momento de preparar este documento, los requisitos permanecen pendientes de verificación. No se presentan como cumplidos aquellos que todavía no han sido probados.
