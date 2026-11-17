# Revisión de la iteración 1

Fecha: 04/12/2026, 2:00 p. m.

Asistentes: todo el equipo, el docente y un Funcionario de Registro (usuario)

Presenta: Ana Gómez (líder de equipo)

## Objetivo de la iteración

Que un estudiante solicite un certificado sin costo, que el worker lo firme con reintentos ante fallas del proveedor y que el estudiante lo descargue.

## Resultado por ítem

| Issue | Caso de uso | Estado | Cumple criterios de aceptación |
|---|---|---|---|
| #1 | CU-01 Solicitar certificado | Terminado | Sí: los 6 escenarios de specs/001 validados |
| #7 | CU-07 Descargar certificado firmado | Terminado | Sí: los 5 escenarios de specs/007 validados |
| #3 | CU-03 Firmar digitalmente | No terminado | No: el escenario 4 (reintentos agotados y cola de errores) aún no se cumple |

## Demostración

- Un estudiante con paz y salvo solicitó un certificado de notas y recibió su código de verificación (escenario 1 de specs/001).
- Se mostró el rechazo de un estudiante con deuda en biblioteca (escenario 3).
- El worker firmó con el proveedor simulado, incluso con el proveedor lento (escenarios 1 a 3 de specs/003).
- El estudiante descargó su certificado firmado y se rechazó la descarga de un certificado ajeno (EAC-04).
- Versión publicada: release v0.1.0 en GitHub.

## Retroalimentación recibida

| Comentario | Quién | Acción |
|---|---|---|
| El estudiante debería ver el motivo cuando su solicitud se rechaza | Funcionario de Registro | Nuevo issue #9 en el backlog |
| Mostrar el código de verificación también en el PDF | Docente | Nuevo issue #10 en el backlog |

## Cambios al backlog

- Ítems nuevos: #9 y #10.
- #3 (CU-03) pasa a la iteración 2 para completar la cola de errores, junto con #2 (CU-02).

## Próximos pasos

- Retrospectiva de la iteración 1: hoy, después de esta revisión.
- Planeación de la iteración 2: lunes 07/12/2026, 8:00 a. m.
