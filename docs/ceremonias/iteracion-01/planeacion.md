# Planeación de la iteración 1

Fecha: 23/11/2026, 8:00 a. m. · Duración de la iteración: 23/11/2026 a 04/12/2026 (2 semanas)

Asistentes: Ana Gómez, Carlos Ríos, Daniela Marín, Felipe Ospina, Laura Cárdenas

Modera: Daniela Marín (gerente de planeación)

## Objetivo de la iteración

Que un estudiante solicite un certificado sin costo, que el worker lo firme con reintentos ante fallas del proveedor y que el estudiante lo descargue.

## Capacidad del equipo

| Concepto | Horas |
|---|---|
| Integrantes × horas por semana × semanas | 5 × 6 × 2 = 60 |
| Reuniones del equipo | 5 |
| Margen de imprevistos (20 %) | 11 |
| **Capacidad de la iteración** | **44** |

## Ítems seleccionados

El orden sale de la matriz de priorización de docs/drivers.md: primero los casos de uso del cuadrante "atender primero" (CU-01, CU-02 y CU-03), ordenados por sus dependencias.

| Issue | Caso de uso | Especificación | Prioridad | Estimación |
|---|---|---|---|---|
| #1 | CU-01 Solicitar certificado | specs/001-solicitar-certificado | Atender primero | 16 h |
| #3 | CU-03 Firmar digitalmente | specs/003-firmar-digitalmente | Atender primero | 18 h |
| #7 | CU-07 Descargar certificado firmado | specs/007-descargar-certificado | Si sobra tiempo | 6 h |
| | **Total planeado** | | | **40 h de 44 h** |

No entra en esta iteración: #2 CU-02 Pagar el trámite (12 h), porque con él se superaría la capacidad (16 + 18 + 12 = 46 h). Pasa a la iteración 2. Mientras tanto, la iteración trabaja con tipos de certificado sin costo.

CU-07 entra aunque está en "si sobra tiempo": cabe en la capacidad, depende solo de CU-03 y permite que el usuario descargue y revise el resultado.

## Tareas

Las tareas agrupan las del `tasks.md` de cada especificación, sin pasar de 4 horas.

| Tarea | Issue | Tareas de la spec | Responsable | Estimación |
|---|---|---|---|---|
| Entidades de dominio de la solicitud | #1 | T-01 a T-05 | Carlos Ríos | 4 h |
| Puertos, DTO y errores de CU-01 | #1 | T-06 a T-14 | Daniela Marín | 3 h |
| Caso de uso SolicitarCertificado | #1 | T-15 | Ana Gómez | 4 h |
| Adaptadores en memoria y simulados de CU-01 | #1 | T-16 a T-20 | Laura Cárdenas | 3 h |
| Composición y validación de los escenarios de CU-01 | #1 | T-21 y T-22 | Felipe Ospina | 2 h |
| Entidades Certificado e IntentoFirma | #3 | T-01 a T-03 | Carlos Ríos | 3 h |
| Puertos de firma, almacenamiento, notificación y cola | #3 | T-04 a T-07 | Daniela Marín | 3 h |
| Política de reintentos y errores de firma | #3 | T-08 a T-10 | Felipe Ospina | 3 h |
| Caso de uso FirmarCertificado | #3 | T-11 | Laura Cárdenas | 4 h |
| Adaptadores simulados de firma, PDF, correo y cola | #3 | T-12 a T-15 | Ana Gómez | 3 h |
| Composición y validación de los escenarios de CU-03 | #3 | T-16 y T-17 | Felipe Ospina | 2 h |
| Puerto de lectura de PDF, DTO y errores de CU-07 | #7 | T-01 a T-05 | Daniela Marín | 2 h |
| Caso de uso DescargarCertificado | #7 | T-06 | Carlos Ríos | 2 h |
| Adaptador, composición y validación de CU-07 | #7 | T-07 a T-09 | Felipe Ospina | 2 h |

Todas las tareas tienen un responsable, duran máximo 4 horas y están en el tablero de GitHub Projects.

## Riesgos identificados

| Riesgo | Acción | Responsable |
|---|---|---|
| El proveedor de firma es lento e inestable (RT-03, R-02) | Trabajar con el proveedor simulado (éxito, lento y caído) | Laura Cárdenas |
| Semana de parciales en otras materias | Margen de imprevistos del 20 % | Daniela Marín |

## Compromiso

Todos los integrantes revisaron el plan y están de acuerdo con él.
