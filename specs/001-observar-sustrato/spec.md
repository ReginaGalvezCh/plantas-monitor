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

## Primera prueba propuesta

**Condición previa:** elegir y registrar una planta, maceta, sustrato, lugar de uso y sonda. La prueba no se declara realizada hasta disponer de mediciones físicas.

1. Marcar una posición y profundidad de inserción para poder repetir las lecturas sin cambiar deliberadamente la geometría.
2. Registrar varias lecturas seguidas antes de un riego habitual, con hora, valor bruto, observación manual del sustrato y posición de la sonda.
3. Registrar varias lecturas después del riego y durante el secado normal, manteniendo la posición. Anotar también cambios de maceta, sustrato o ubicación.
4. Comparar la variación entre lecturas cercanas con la variación observada a lo largo del secado. Si no se distinguen, revisar sensor y método antes de proponer una regla.
5. Probar por separado una lectura anómala, la falta de lectura y una lectura antigua. Deben producir un estado prudente, nunca una orden de riego.
6. Documentar los datos, observaciones, regla candidata y excepciones. El intervalo de lectura, la vigencia y el criterio de «lecturas consistentes» se fijarán a partir de esta evidencia.

## Límite de interpretación

El sensor observa una zona del sustrato; no diagnostica la salud de toda la planta. «Revisar sustrato» pide una comprobación humana. No se usará «regar ahora» como conclusión automática de una lectura aislada.

## Fuera de alcance por ahora

Riego automático, diagnóstico de salud de la planta y sincronización con la pantalla central.

## Preguntas abiertas

¿Qué planta y maceta? ¿Qué tecnología de sonda resiste el uso previsto? ¿Qué intervalo de lectura y antigüedad máxima son adecuados? ¿Cómo se confirma que el aviso fue atendido?
