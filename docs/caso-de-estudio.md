# Caso de estudio: aplicación de la metodología Kanban

## 1. Contexto

**CrediYa** es una empresa de microcréditos con sede en Quito que atiende a más de 1 200 clientes. Su proceso de cobranza se lleva en hojas de cálculo individuales: no hay visibilidad del estado real de los clientes en mora, los pagos se registran con retraso, y el historial de cada cliente está disperso. El área de cobranzas pierde aproximadamente 6 horas semanales reconstruyendo información.

El gerente general autoriza el desarrollo de un **sistema web de gestión de cobranzas** y asigna un equipo de 4 personas durante 12 semanas.

## 2. Problema

- No existe un registro centralizado de clientes en mora.
- Los cobradores no saben qué cliente atender ni con qué prioridad.
- No hay métricas del proceso de cobranza (tiempo de respuesta, recuperaciones).

## 3. Solución propuesta

Un sistema web que centralice clientes, créditos y pagos, con un módulo de morosidad que ordene los clientes por días de atraso y monto, y un módulo de notificaciones automáticas por correo. El desarrollo del sistema se gestiona con la **metodología Kanban**.

## 4. Por qué Kanban

Kanban es ideal para este caso porque:

| Criterio | Kanban |
|---|---|
| Naturaleza del trabajo | Continuo (el flujo de tareas no se detiene en sprints) |
| Cambios de prioridad | Se aceptan en cualquier momento (la columna Inicio se reordena) |
| Equipos | Pequeños y multifuncionales (4 personas) |
| Entregas | Continuas, tan pronto una tarjeta llega a Finalizado |

## 5. Implementación del tablero

El tablero tiene tres columnas: **Inicio**, **En Proceso** y **Finalizado**.

- **Regla de entrada**: una tarjeta entra al tablero solo si tiene responsable, duración estimada y criterio de finalización.
- **Límite WIP**: máximo 2 tarjetas por persona en En Proceso.
- **Regla de avance**: una tarjeta pasa a Finalizado cuando pasa la revisión de un compañero distinto al autor.
- **Reunión diaria**: 10 minutos frente al tablero; cada integrante comenta qué avanzó, qué hará y qué le bloquea.

## 6. Tarjetas del tablero

Formato de tarjeta: **responsable → duración → tarea**.

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

## 7. Recursos

### Recurso humano
- 4 integrantes del equipo de desarrollo (Juan, Kathya, Pierina, Darim).
- 1 usuario clave del área de cobranzas como patrocinador del proyecto.

### Recurso material
- 4 computadoras de desarrollo.
- Repositorio GitHub open source con licencia GPL-3.0.
- Tablero Kanban físico (pizarra) y tablero digital en GitHub Projects.
- Hoja de cálculo Excel para el seguimiento del proyecto.

### Recurso costo
- 480 horas/hombre totales estimadas (4 integrantes × 12 semanas × 10 h).
- Costo de infraestructura: 0 USD (GitHub gratuito para proyectos open source).

## 8. Métricas de seguimiento

| Métrica | Definición | Meta |
|---|---|---|
| Lead time | Días desde que una tarjeta entra a Inicio hasta Finalizado | ≤ 10 d |
| Cycle time | Días desde que una tarjeta entra a En Proceso hasta Finalizado | ≤ 5 d |
| Throughput | Tarjetas finalizadas por semana | ≥ 3 |
| Bloqueos | Tarjetas detenidas más de 2 días | 0 |

## 9. Resultado esperado

Al finalizar las 12 semanas, CrediYa contará con un sistema web que reduce el tiempo de gestión de cobranzas de 6 horas semanales a menos de 1 hora, con información centralizada y métricas en tiempo real, entregado de forma continua gracias al flujo Kanban.
