# Cuándo pasar de skill a agente

No queremos convertir una skill en agente demasiado pronto.

Primero debe demostrar que el proceso está suficientemente claro.

## Una skill está preparada cuando

- resuelve correctamente la mayoría de los casos habituales;
- sabemos qué información necesita para trabajar;
- sus decisiones siguen criterios claros;
- conocemos las excepciones importantes;
- los errores más frecuentes ya están controlados;
- el resultado esperado puede definirse con claridad;
- sabemos qué herramientas o conectores necesitará fuera de ChatGPT.

## Señales de que todavía no está preparada

- cambia mucho de comportamiento entre casos similares;
- necesita demasiadas instrucciones manuales cada vez;
- seguimos modificando continuamente el objetivo del proceso;
- no sabemos qué hacer ante errores o datos incompletos;
- todavía no hemos probado suficientes casos reales.

## Cuándo merece la pena crear el agente

La conversión tiene sentido cuando necesitamos una o varias de estas capacidades:

- ejecución automática;
- trabajo programado;
- reaccionar ante eventos;
- acceso continuo a servicios externos;
- memoria o almacenamiento persistente;
- logs y trazabilidad;
- ejecución para clientes o usuarios externos;
- integración con otros sistemas.

## Regla de decisión

**Primero validamos el proceso. Después automatizamos su ejecución.**

El agente no debería utilizarse para descubrir cómo funciona el proceso. Esa parte debe resolverse principalmente durante la fase de skill y pruebas.
