# Plan de ejecución — EspaiFP (F3)

## Datos del proyecto

- **Proyecto:** EspaiFP — Sistema de reserva y gestión de aulas.
- **Módulo:** 2CFSS · Projecte intermodular 2.
- **Ciclo:** Desarrollo de Aplicaciones Web (DAW).
- **Curso:** 2026-2027.
- **Responsable:** Juan Antonio Torregrosa Macia.

## Objetivo de la planificación

Organizar las tareas necesarias para desarrollar EspaiFP, establecer su secuencia y dependencias, estimar tiempos y recursos, y definir procedimientos para controlar el progreso y los riesgos.

## Descomposición de tareas y dependencias

| ID | Tarea | Dependencia principal | Duración estimada |
|---|---|---|---:|
| T01 | Análisis de requisitos | — | 4 h |
| T02 | Preparación del entorno | T01 | 3 h |
| T03 | Creación del repositorio GitHub | T01 | 2 h |
| T04 | Diseño de la base de datos | T01 | 5 h |
| T05 | Diseño de la interfaz | T01 | 5 h |
| T06 | Estructura del proyecto | T02, T03, T04 y T05 | 5 h |
| T07 | Autenticación y permisos | T06 | 8 h |
| T08 | Gestión de aulas | T06 | 8 h |
| T09 | Consulta de disponibilidad | T08 | 5 h |
| T10 | Gestión de reservas | T07, T08 y T09 | 12 h |
| T11 | Control de solapamientos | T10 | 6 h |
| T12 | Gestión administrativa | T07, T08 y T10 | 12 h |
| T13 | Desarrollo e integración del frontend | T05, T07, T09, T10 y T12 | 15 h |
| T14 | Validaciones y adaptación | T13 | 6 h |
| T15 | Pruebas y corrección de errores | T13 y T14 | 10 h |
| T16 | Despliegue | T15 | 4 h |
| T17 | Documentación y entrega | T15 y T16 | 6 h |

**Esfuerzo estimado total: 116 horas.**

## Cronograma inicial

| Tarea | Inicio | Fin |
|---|---|---|
| T01 | 16/11/2026 | 22/11/2026 |
| T02–T03 | 23/11/2026 | 29/11/2026 |
| T04–T05 | 30/11/2026 | 13/12/2026 |
| T06 | 14/12/2026 | 20/12/2026 |
| Periodo sin tareas programadas | 21/12/2026 | 03/01/2027 |
| T07 | 04/01/2027 | 17/01/2027 |
| T08 | 18/01/2027 | 31/01/2027 |
| T09 | 01/02/2027 | 07/02/2027 |
| T10 | 08/02/2027 | 21/02/2027 |
| T11 | 22/02/2027 | 28/02/2027 |
| T12 | 01/03/2027 | 14/03/2027 |
| T13 | 15/03/2027 | 04/04/2027 |
| T14 | 05/04/2027 | 11/04/2027 |
| T15 | 12/04/2027 | 25/04/2027 |
| T16 | 26/04/2027 | 02/05/2027 |
| T17 | 03/05/2027 | 09/05/2027 |

Las fechas constituyen una previsión inicial y deberán revisarse de acuerdo con el calendario académico, la carga de los demás módulos y el progreso real.

## Hitos

- **H1 — 20/12/2026:** análisis, diseño y estructura inicial preparados.
- **H2 — 14/03/2027:** funcionalidades principales del servidor completadas.
- **H3 — 11/04/2027:** frontend integrado y adaptado.
- **H4 — 09/05/2027:** pruebas, despliegue y documentación completados.

## Recursos principales

Ordenador personal, Windows, Visual Studio Code, XAMPP, PHP, Apache, MariaDB, phpMyAdmin, Git, GitHub, diagrams.net, navegadores web y LibreOffice. El desarrollo inicial se realizará en local; el alojamiento externo solo se necesitará para el despliegue previsto.

## Diagramas

- [Diagrama de Gantt](diagramas/Gantt_EspaiFP_F3.png)

## Responsabilidad

El proyecto es individual. El alumno asumirá las funciones de análisis, diseño, desarrollo frontend y backend, gestión de datos, pruebas, despliegue y documentación.
