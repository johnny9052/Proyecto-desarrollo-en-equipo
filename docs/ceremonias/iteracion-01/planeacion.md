# Planeación de la iteración 1

Fecha: 2026-11-23 · Duración de la iteración: 2026-11-23 a 2026-12-04 (2 semanas)

Asistentes: Ana Gómez, Carlos Ríos, Daniela Marín, Felipe Ospina, Laura Cárdenas

Modera: Daniela Marín (gerente de planeación)

## Objetivo de la iteración

Permitir que un estudiante registre su solicitud de práctica, que se le asigne un asesor y que el asesor reciba la notificación.

## Capacidad del equipo

| Concepto | Horas |
|---|---|
| Integrantes × horas por semana × semanas | 5 × 6 × 2 = 60 |
| Reuniones del equipo | 5 |
| Margen de imprevistos (20 %) | 11 |
| **Capacidad de la iteración** | **44** |

## Ítems seleccionados

| Issue | Ítem | Prioridad (MoSCoW) | Estimación |
|---|---|---|---|
| #3 | Registrar solicitud de práctica | Must | 8 h |
| #5 | Consultar solicitudes registradas | Must | 6 h |
| #6 | Asignar asesor | Must | 10 h |
| #8 | Notificar por correo al asesor | Should | 5 h |
| | **Total planeado** | | **29 h de 44 h** |

No entra en esta iteración: #9 Leer código QR (16 h), porque con él se superaría la capacidad (29 + 16 = 45 h).

Las 15 h restantes quedan para refinamiento de la iteración 2 y para corregir defectos.

## Tareas

| Tarea | Ítem | Responsable | Estimación |
|---|---|---|---|
| Elaborar mockup del formulario de registro | #3 | Ana Gómez | 2 h |
| Implementar la lógica de registro | #3 | Carlos Ríos | 4 h |
| Diseñar y ejecutar pruebas del registro | #3 | Felipe Ospina | 2 h |
| Elaborar el listado de solicitudes | #5 | Daniela Marín | 3 h |
| Implementar la consulta en el backend | #5 | Laura Cárdenas | 3 h |
| Implementar las reglas de asignación de asesor | #6 | Carlos Ríos | 4 h |
| Elaborar la pantalla de asignación | #6 | Daniela Marín | 3 h |
| Probar la asignación de asesor | #6 | Felipe Ospina | 3 h |
| Configurar el servicio de correo | #8 | Laura Cárdenas | 2 h |
| Implementar la notificación al asesor | #8 | Ana Gómez | 3 h |

Todas las tareas tienen un responsable, duran máximo 4 horas y están en el tablero de GitHub Projects.

## Riesgos identificados

| Riesgo | Acción | Responsable |
|---|---|---|
| Acceso al servicio de correo institucional | Usar un servicio de pruebas mientras se obtiene el acceso | Laura Cárdenas |
| Semana de parciales en otras materias | Margen de imprevistos del 20 % | Daniela Marín |

## Compromiso

Todos los integrantes revisaron el plan y están de acuerdo con él.
