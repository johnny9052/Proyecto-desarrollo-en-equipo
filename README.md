# Sistema de certificados en línea

Proyecto del curso Arquitectura de Soluciones de Software (9919G8F), Universidad de Caldas.

Equipo 3: Ana Gómez, Carlos Ríos, Daniela Marín, Felipe Ospina, Laura Cárdenas.

## Propósito

Aplicación web en la que el estudiante o egresado solicita un certificado académico, paga el trámite y descarga un PDF firmado digitalmente por un proveedor externo, sin desplazarse a la Universidad. El Funcionario de Registro solo revisa las solicitudes con novedades.

Este repositorio muestra cómo se organiza el trabajo en equipo del proyecto: normas, roles y actas de las ceremonias. La arquitectura del caso (visión, drivers, ADR, vistas) y las especificaciones de SDD viven en las carpetas `docs/` y `specs/`.

## Estructura del repositorio

```
.
├── README.md                 Este archivo: qué es el proyecto y cómo trabajar en él
├── AGENTS.md                 Reglas permanentes para el agente de IA (SDD)
├── docs/
│   ├── vision.md             Documento de visión
│   ├── drivers.md            Drivers: catálogo de casos de uso (CU-01 a CU-08) y matriz de priorización
│   ├── arquitectura.md       Documento de arquitectura
│   ├── adr/                  Registros de decisión arquitectónica
│   ├── vistas/               Vistas arquitectónicas (4+1)
│   ├── equipo/
│   │   ├── normas.md         Normas de comportamiento y comunicación
│   │   └── roles.md          Roles TSPi y responsables
│   └── ceremonias/
│       └── iteracion-01/
│           ├── planeacion.md     Acta de planeación
│           ├── revision.md       Acta de revisión
│           └── retrospectiva.md  Acta de retrospectiva
├── specs/                    Una carpeta por caso de uso (001 a 008): spec, plan, tareas y validación
└── src/                      Código fuente
```

## Del caso de uso al tablero

| Caso de uso (drivers.md) | Issue | Especificación |
|---|---|---|
| CU-01 Solicitar certificado | #1 | specs/001-solicitar-certificado |
| CU-02 Pagar el trámite | #2 | specs/002-pagar-tramite |
| CU-03 Firmar digitalmente | #3 | specs/003-firmar-digitalmente |
| CU-04 Consultar estado de la solicitud | #4 | specs/004-consultar-estado |
| CU-05 Actualizar perfil | #5 | specs/005-actualizar-perfil |
| CU-06 Generar reporte mensual | #6 | specs/006-generar-reporte-mensual |
| CU-07 Descargar certificado firmado | #7 | specs/007-descargar-certificado |
| CU-08 Revisar solicitudes con novedades | #8 | specs/008-revisar-novedades |

Cada issue tiene el mismo número de su caso de uso. Las tareas de cada issue salen del `tasks.md` de su especificación.

## Cómo ejecutar el proyecto

1. Clonar el repositorio:
   ```
   git clone https://github.com/<organizacion>/certificados.git
   ```
2. Instalar Python 3.12.
3. Ejecutar `python src/main.py`: en esta etapa se usan adaptadores en memoria y simulados.

> El gerente de soporte mantiene esta sección al día cada vez que cambia el entorno.

## Forma de trabajo

- Tablero del equipo: GitHub Projects, proyecto "Certificados en línea".
- Cada tarea es un issue o sub-issue; cada cambio llega por pull request con "Closes #n".
- Ningún pull request se integra sin la revisión de otro integrante.
- Las normas del equipo están en [docs/equipo/normas.md](docs/equipo/normas.md).
- Los roles y responsables están en [docs/equipo/roles.md](docs/equipo/roles.md).
