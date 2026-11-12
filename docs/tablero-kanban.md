# Tablero Kanban del proyecto

Tablero digital espejo del tablero físico. Columnas: **Inicio**, **En Proceso**, **Finalizado**.

## Formato de tarjeta

```
┌─────────────────────────────┐
│ Responsable: [Nombre]       │
│ Duración:    [Xd / X sem]   │
│ Tarea:       [Descripción]  │
└─────────────────────────────┘
```

## Estado actual del tablero

### Inicio
- [Kathya] · 1 sem · Analizar los clientes en mora y sus patrones de pago
- [Pierina] · 5 d · Diseñar un ListView para mostrar clientes en mora
- [Darim] · 1 sem · Diseñar la base de datos de clientes y créditos
- [Juan] · 3 d · Definir políticas WIP y métricas del tablero

### En Proceso
- [Darim] · 4 d · Desarrollar API REST para registro de pagos
- [Pierina] · 6 d · Implementar módulo de notificaciones por correo

### Finalizado
- [Juan] · 2 sem · Levantar requerimientos con el área de cobranzas
- [Kathya] · 1 sem · Documentar el caso de negocio y el alcance
- [Juan] · 3 d · Configurar repositorio GitHub con licencia GPL-3.0

## Políticas del tablero

| Política | Regla |
|---|---|
| WIP | Máximo 2 tarjetas por persona en En Proceso |
| Avance | Revisión de un compañero distinto al autor para pasar a Finalizado |
| Bloqueo | Una tarjeta detenida 2 días se marca con etiqueta roja y se trata en la reunión diaria |
| Reunión | Diaria, 10 minutos, frente al tablero |

## Métricas

| Métrica | Definición | Meta |
|---|---|---|
| Lead time | Días desde Inicio hasta Finalizado | ≤ 10 d |
| Cycle time | Días desde En Proceso hasta Finalizado | ≤ 5 d |
| Throughput | Tarjetas finalizadas por semana | ≥ 3 |
| Bloqueos | Tarjetas detenidas más de 2 días | 0 |
