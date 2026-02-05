# CR-004 – Hotfix duplicación de pagos

## Descripción del problema
Durante horas pico, el sistema de matrículas duplica pagos en aproximadamente el 1% de las transacciones,
afectando la integridad financiera del sistema.

## Solución propuesta
- Implementar control de idempotencia por ID de transacción.
- Validar si un pago ya fue registrado antes de procesarlo nuevamente.

## Impacto
- No se modifica la funcionalidad del sistema.
- Cambio correctivo sobre el módulo de pagos.

## Plan de rollback
En caso de fallas, revertir a la versión estable anterior (tag v1.2.2).
