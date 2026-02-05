# QA – CR-004 Hotfix duplicación de pagos

## Casos de prueba

**QA-PAY-01**
Pago único válido → resultado esperado: pago registrado una sola vez.

**QA-PAY-02**
Reenvío de la misma transacción → resultado esperado: no se duplica.

**QA-PAY-03**
Múltiples solicitudes concurrentes → resultado esperado: un solo pago.

**QA-PAY-04**
Prueba de regresión del proceso de matrícula → resultado esperado: OK.

**QA-PAY-05**
Simulación de hora pico → resultado esperado: sin duplicados.
