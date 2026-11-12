# Especificación 001: observar el sustrato

**Estado:** propuesta para validar.

## Propósito

Ayudar a decidir cuándo revisar una planta concreta sin presentar una lectura aislada como certeza de que necesita riego.

## Comportamiento esperado

1. El sistema registra lecturas de humedad de una planta identificada y permite compararlas en el tiempo.
2. Una indicación de revisión aparece únicamente tras lecturas consistentes con el criterio calibrado para esa planta.
3. Cuando los datos son antiguos, ausentes o incoherentes, informa «estado desconocido».
4. El aviso puede descartarse o restablecerse después de revisar la planta; la regla exacta queda pendiente de la prueba.

## Criterios de aceptación del piloto

- Se puede distinguir un estado normal, «revisar sustrato» y «desconocido».
- Una lectura única anómala no dispara el aviso.
- La desconexión del sensor no se interpreta como sequedad.
- El umbral se documenta con observaciones de la planta de prueba, sin afirmar que sirva para todas.

## Fuera de alcance por ahora

Riego automático, diagnóstico de salud de la planta y sincronización con la pantalla central.

## Preguntas abiertas

¿Qué planta y maceta? ¿Qué tecnología de sonda resiste el uso previsto? ¿Qué intervalo de lectura y antigüedad máxima son adecuados? ¿Cómo se confirma que el aviso fue atendido?

