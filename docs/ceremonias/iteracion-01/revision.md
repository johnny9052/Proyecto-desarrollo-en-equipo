# Revisión de la iteración 1

Fecha: 27/11/2026, 2:00 p. m.

Asistentes: todo el equipo, el docente y un Funcionario de Registro (usuario)

Presenta: Ana Gómez (líder de equipo)

## Objetivo de la iteración

Que un estudiante autenticado solicite y pague un certificado, que el worker lo firme con reintentos ante fallas del proveedor y que la API y el worker queden desplegados en contenedores.

## Resultado por ítem

| Issue | Ítem | Estado | Cumple criterios de aceptación |
|---|---|---|---|
| #1 | CU-01 Solicitar certificado | Terminado | Sí: los 6 escenarios de specs/001 validados |
| #2 | CU-02 Pagar el trámite | Terminado | Sí: los 6 escenarios de specs/002 validados |
| #9 | PA-02 Autenticación institucional | Terminado | Sí: la API rechaza peticiones sin token válido |
| #10 | PA-06 Despliegue en Docker | Terminado | Sí: API y worker corren en sus contenedores |
| #3 | CU-03 Firmar digitalmente | No terminado | No: el escenario 4 (reintentos agotados y cola de errores) aún no se cumple |

## Demostración

- Un estudiante con paz y salvo pagó y solicitó un certificado de notas, y recibió su código de verificación (escenario 1 de specs/001).
- Se mostró el rechazo de un estudiante con deuda en biblioteca (escenario 3 de specs/001).
- Se mostró un pago rechazado y el reintento del pago (escenario 3 de specs/002).
- El worker firmó con el proveedor simulado, incluso con el proveedor lento (escenarios 1 a 3 de specs/003).
- La API y el worker se levantaron con sus imágenes Docker.
- Versión publicada: release v0.1.0 en GitHub.

## Retroalimentación recibida

| Comentario | Quién | Acción |
|---|---|---|
| El estudiante debería ver el motivo cuando su solicitud se rechaza | Funcionario de Registro | Nuevo issue #17 en el backlog |
| Mostrar el código de verificación también en el PDF | Docente | Nuevo issue #18 en el backlog |

## Cambios al backlog

- Ítems nuevos: #17 y #18.
- #3 (CU-03) pasa a la iteración 2 para completar la cola de errores, junto con #11 (RT-02), que no cupo en la iteración 1.

## Próximos pasos

- Retrospectiva de la iteración 1: hoy, después de esta revisión.
- Planeación de la iteración 2: lunes 30/11/2026, 8:00 a. m.
