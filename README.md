# Sistema de Gestión de Cobranzas — Caso de Estudio de la Metodología Kanban

Proyecto open source (licencia **GPL-3.0**) que documenta un caso de estudio donde se aplica la **metodología Kanban** para gestionar el desarrollo de un sistema web de gestión de cobranzas para clientes en mora.

## Descripción del caso

**CrediYa** es una empresa de microcréditos que registra más de 1 200 clientes y gestiona el cobro de sus créditos en hojas de cálculo sueltas. El área de cobranzas no tiene visibilidad del estado real de los clientes en mora, los pagos se registran con retraso y no existe un historial confiable por cliente.

Para resolver este problema, un equipo de 4 personas desarrollará un **sistema web de gestión de cobranzas** aplicando la metodología **Kanban**: el trabajo se visualiza en un tablero con las columnas **Inicio**, **En Proceso** y **Finalizado**, cada tarea tiene un responsable, una duración estimada y un límite de trabajo en progreso (WIP).

## Equipo y roles

| Integrante | Rol | Responsabilidad principal |
|---|---|---|
| Juan | Coach Kanban / Líder de proyecto | Gestión del tablero, métricas, límites WIP |
| Kathya | Analista de requerimientos | Análisis del negocio, documentación |
| Pierina | Desarrolladora Frontend | Interfaz web, vistas de clientes en mora |
| Darim | Desarrollador Backend / QA | Base de datos, API REST, pruebas |

## Tablero Kanban

Cada tarjeta del tablero se define con el formato: **responsable → duración → tarea**.

### Inicio
| Responsable | Duración | Tarea |
|---|---|---|
| Kathya | 1 sem | Analizar los clientes en mora y sus patrones de pago |
| Pierina | 5 d | Diseñar un ListView para mostrar clientes en mora |
| Darim | 1 sem | Diseñar la base de datos de clientes y créditos |
| Juan | 3 d | Definir políticas WIP y métricas del tablero |

### En Proceso
| Responsable | Duración | Tarea |
|---|---|---|
| Darim | 4 d | Desarrollar API REST para registro de pagos |
| Pierina | 6 d | Implementar módulo de notificaciones por correo |

### Finalizado
| Responsable | Duración | Tarea |
|---|---|---|
| Juan | 2 sem | Levantar requerimientos con el área de cobranzas |
| Kathya | 1 sem | Documentar el caso de negocio y el alcance |
| Juan | 3 d | Configurar repositorio GitHub con licencia GPL-3.0 |

## Recursos

### Recurso humano
- 4 integrantes del equipo de desarrollo (Juan, Kathya, Pierina, Darim).
- 1 usuario clave del área de cobranzas como patrocinador del proyecto.

### Recurso material
- 4 computadoras de desarrollo.
- Repositorio GitHub (open source) con licencia GPL-3.0.
- Tablero Kanban físico (pizarra) y tablero digital en GitHub Projects.
- Hoja de cálculo Excel para el seguimiento del proyecto.

### Recurso costo
- 480 horas/hombre totales estimadas (4 integrantes × 12 semanas × 10 h).
- Costo de infraestructura: 0 USD (GitHub gratuito en plan open source).

## Principios Kanban aplicados

1. **Visualizar el trabajo**: todas las tareas son visibles en el tablero (Inicio → En Proceso → Finalizado).
2. **Limitar el trabajo en progreso (WIP)**: máximo 2 tareas simultáneas por integrante.
3. **Gestionar el flujo**: las tarjetas avanzan de columna solo cuando la tarea anterior termina.
4. **Hacer explícitas las políticas del proceso**: cada tarjeta define responsable, duración y criterio de finalización.
5. **Mejorar continuamente**: reunión breve diaria (10 min) frente al tablero para detectar bloqueos.

## Contenido del repositorio

```
├── LICENSE            # Licencia GPL-3.0
├── README.md          # Este archivo
├── docs/
│   ├── caso-de-estudio.md   # Caso de estudio completo
│   └── tablero-kanban.md    # Detalle del tablero y métricas
└── .gitignore
```

## Licencia

Este proyecto está bajo la licencia **GNU General Public License v3.0** — consulte el archivo [LICENSE](LICENSE) para más detalles.
