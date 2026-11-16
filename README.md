# Sistema de Gestión de Prácticas Empresariales

Proyecto del curso Arquitectura de Soluciones de Software (9919G8F), Universidad de Caldas.

Equipo 3: Ana Gómez, Carlos Ríos, Daniela Marín, Felipe Ospina, Laura Cárdenas.

## Propósito

Aplicación web que permite a los estudiantes registrar su solicitud de práctica empresarial, a los asesores revisarla y a la coordinación hacer seguimiento al proceso.

## Estructura del repositorio

```
.
├── README.md                 Este archivo: qué es el proyecto y cómo ejecutarlo
├── docs/
│   ├── vision.md             Documento de visión
│   ├── drivers.md            Drivers arquitectónicos
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
└── src/                      Código fuente
```

## Cómo ejecutar el proyecto

1. Clonar el repositorio:
   ```
   git clone https://github.com/<organizacion>/practicas-empresariales.git
   ```
2. Instalar las dependencias (ver la sección de tecnologías).
3. Ejecutar la aplicación y abrir el navegador en la dirección indicada.

> El gerente de soporte mantiene esta sección al día cada vez que cambia el entorno.

## Tecnologías

| Capa | Tecnología | Versión |
|---|---|---|
| Frontend | Por definir en el ADR correspondiente | |
| Backend | Por definir en el ADR correspondiente | |
| Base de datos | Por definir en el ADR correspondiente | |

## Forma de trabajo

- Tablero del equipo: GitHub Projects, proyecto "Prácticas empresariales".
- Cada tarea es un issue; cada cambio llega por pull request con "Closes #n".
- Ningún pull request se integra sin la revisión de otro integrante.
- Las normas del equipo están en [docs/equipo/normas.md](docs/equipo/normas.md).
- Los roles y responsables están en [docs/equipo/roles.md](docs/equipo/roles.md).
