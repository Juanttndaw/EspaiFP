
# Indicadores de calidad – EspaiFP

Este documento recoge los indicadores que se utilizarán para comprobar la calidad de la aplicación EspaiFP durante su desarrollo.

Los indicadores se revisarán progresivamente a medida que se implementen las funcionalidades. Los resultados se actualizarán cuando se realicen las comprobaciones correspondientes.

## Registro de indicadores

| ID | Indicador | Aspecto que controla | Cómo se comprobará | Resultado aceptable | Cuándo se comprobará | Estado |
|---|---|---|---|---|---|---|
| IC01 | Cumplimiento de requisitos funcionales | Que las funcionalidades previstas estén implementadas. | Revisar cada requisito y realizar su prueba correspondiente. | El 100 % de los requisitos esenciales supera su comprobación antes de la entrega final. | Durante el desarrollo y al finalizar el proyecto. | Pendiente |
| IC02 | Prevención de reservas incompatibles | Que no existan dos reservas incompatibles para la misma aula y horario. | Intentar crear dos reservas para el mismo espacio y franja horaria. | El sistema rechaza la segunda reserva e informa del conflicto. | Al implementar las reservas y durante las pruebas generales. | Pendiente |
| IC03 | Validación de formularios | Que los campos obligatorios y los datos introducidos sean correctos. | Enviar formularios vacíos, incompletos o con datos no válidos. | Los datos incorrectos son rechazados y se muestran mensajes de error claros. | Durante el desarrollo de cada formulario. | Pendiente |
| IC04 | Autenticación y permisos | Que los usuarios accedan únicamente a las funciones que les corresponden. | Probar el acceso con usuarios de distintos roles y sin iniciar sesión. | Las operaciones restringidas no pueden realizarse sin los permisos correspondientes. | Al implementar el inicio de sesión y los permisos. | Pendiente |
| IC05 | Integridad de los datos | Que las reservas, usuarios y aulas se almacenen correctamente. | Crear, modificar y eliminar registros y comprobar los datos guardados en MariaDB. | Los datos se conservan correctamente y no aparecen registros duplicados o relaciones incorrectas. | Durante el desarrollo de la base de datos y las pruebas de integración. | Pendiente |
| IC06 | Adaptación a diferentes dispositivos | Que la interfaz pueda utilizarse en distintos tamaños de pantalla. | Revisar las pantallas principales en ordenador, tableta y móvil. | Los elementos principales se muestran correctamente, sin cortes ni desplazamientos horizontales innecesarios. | Durante el desarrollo del frontend y antes de la entrega. | Pendiente |
| IC07 | Usabilidad y accesibilidad básica | Que los usuarios puedan comprender y utilizar la aplicación. | Revisar textos, etiquetas, navegación, formularios y contraste. | Los controles tienen etiquetas comprensibles y la información es legible. | Durante el diseño de la interfaz y la evaluación con usuarios. | Pendiente |
| IC08 | Ausencia de errores críticos | Que las funciones principales no presenten fallos que impidan su utilización. | Ejecutar las pruebas previstas y revisar los errores detectados. | No quedan errores críticos conocidos que impidan iniciar sesión, consultar disponibilidad o gestionar reservas. | En las revisiones importantes y antes de la entrega final. | Pendiente |

## Actualización de los indicadores

Los indicadores se revisarán durante el desarrollo y en las comprobaciones generales del proyecto.

Cuando se realice una prueba, se anotará el resultado obtenido y se actualizará el estado correspondiente.

Se utilizarán los siguientes estados:

- **Pendiente:** todavía no se ha realizado la comprobación.
- **En revisión:** se está comprobando el indicador.
- **Cumplido:** se ha obtenido el resultado esperado.
- **No cumplido:** la comprobación ha detectado problemas que necesitan corrección.

Cuando un indicador no alcance el resultado esperado, se analizará el problema y, si corresponde, se registrará una incidencia en GitHub Issues.

Los resultados y las evidencias se conservarán en el repositorio para poder consultar la evolución de la calidad de EspaiFP.
