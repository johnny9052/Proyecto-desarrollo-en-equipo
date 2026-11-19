# Planeación de la iteración 1

Fecha: 23/11/2026, 8:00 a. m. · Duración de la iteración: 23/11/2026 a 27/11/2026 (1 semana)

Asistentes: Ana Gómez, Carlos Ríos, Daniela Marín, Felipe Ospina, Laura Cárdenas

Modera: Daniela Marín (gerente de planeación)

## Objetivo de la iteración

Que un estudiante autenticado solicite y pague un certificado, que el worker lo firme con reintentos ante fallas del proveedor y que la API y el worker queden desplegados en contenedores.

## Capacidad del equipo

El proyecto dura 2 semanas y se divide en 2 iteraciones de 1 semana.

| Concepto | Proyecto (2 semanas) | Iteración 1 (1 semana) |
|---|---|---|
| Integrantes × horas por semana × semanas | 5 × 10 × 2 = 100 | 5 × 10 × 1 = 50 |
| Reuniones del equipo | 10 | 5 |
| Margen de imprevistos (20 %) | 18 | 9 |
| **Capacidad** | **72** | **36** |

## Ítems seleccionados

El orden sale de la matriz de priorización de docs/drivers.md: primero los casos de uso de "atender primero" (CU-01, CU-02 y CU-03) y después el trabajo técnico de "hacer ya" que los habilita. Las estimaciones consideran que cada caso de uso se implementa con SDD y apoyo de IA a partir de su spec, plan y tareas.

| Issue | Ítem | Origen | Prioridad | Estimación |
|---|---|---|---|---|
| #1 | CU-01 Solicitar certificado | specs/001-solicitar-certificado | Atender primero | 8 h |
| #3 | CU-03 Firmar digitalmente | specs/003-firmar-digitalmente | Atender primero | 9 h |
| #2 | CU-02 Pagar el trámite | specs/002-pagar-tramite | Atender primero | 6 h |
| #9 | PA-02 Autenticación institucional y validador de token | ADR-004 | Hacer ya | 4 h |
| #10 | PA-06 Despliegue de API y worker en Docker | ADR-008 | Hacer ya | 4 h |
| | **Total planeado** | | | **31 h de 36 h** |

No entra en esta iteración: #11 RT-02 Adaptador real de PostgreSQL (6 h), porque con él se superaría la capacidad (31 + 6 = 37 h). Pasa a la iteración 2. Mientras tanto se usan los adaptadores en memoria que definen las specs.

## Tareas

Las tareas agrupan las del `tasks.md` de cada especificación, sin pasar de 4 horas.

| Tarea | Issue | Tareas de la spec | Responsable | Estimación |
|---|---|---|---|---|
| Dominio, puertos, DTO y errores de CU-01 | #1 | T-01 a T-14 | Carlos Ríos | 3 h |
| Caso de uso SolicitarCertificado y adaptadores simulados | #1 | T-15 a T-20 | Ana Gómez | 3 h |
| Composición y validación de los escenarios de CU-01 | #1 | T-21 y T-22 | Felipe Ospina | 2 h |
| Dominio, puertos y política de reintentos de CU-03 | #3 | T-01 a T-10 | Daniela Marín | 3 h |
| Caso de uso FirmarCertificado y adaptadores simulados | #3 | T-11 a T-15 | Laura Cárdenas | 4 h |
| Composición y validación de los escenarios de CU-03 | #3 | T-16 y T-17 | Felipe Ospina | 2 h |
| Dominio, puertos, DTO y errores de CU-02 | #2 | T-01 a T-09 | Carlos Ríos | 2 h |
| Casos de uso IniciarPago y ConfirmarPago | #2 | T-10 y T-11 | Ana Gómez | 2 h |
| Adaptadores, composición y validación de CU-02 | #2 | T-12 a T-15 | Felipe Ospina | 2 h |
| Validador de token con la autenticación institucional | #9 | | Daniela Marín | 4 h |
| Imágenes Docker de la API y del worker | #10 | | Laura Cárdenas | 4 h |

Todas las tareas tienen un responsable, duran máximo 4 horas y están en el tablero de GitHub Projects.

## Riesgos identificados

| Riesgo | Acción | Responsable |
|---|---|---|
| El proveedor de firma es lento e inestable (RT-03, R-02) | Trabajar con el proveedor simulado (éxito, lento y caído) | Laura Cárdenas |
| Docker no está disponible en el servidor asignado (riesgo del ADR-008) | Confirmarlo con el Área de Sistemas el primer día | Laura Cárdenas |
| El mecanismo de autenticación institucional es un supuesto (S-03) | Validarlo con el Administrador del SIA antes de implementar | Daniela Marín |
| Evaluaciones en otras materias | Margen de imprevistos del 20 % | Daniela Marín |

## Compromiso

Todos los integrantes revisaron el plan y están de acuerdo con él.
