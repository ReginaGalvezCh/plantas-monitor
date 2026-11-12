# Monitor de plantas

Proyecto independiente para ayudar a detectar cuándo conviene revisar la humedad del sustrato de una planta. La primera versión observará una planta real y dará una indicación prudente; no regará automáticamente.

## Estado

Definición inicial. Sin sensor elegido, prototipo físico ni calibración completada.

## Primer alcance

- Medir humedad de forma comparable en la misma planta.
- Pedir que se revise el sustrato cuando varias lecturas coherentes indiquen sequedad.
- Mostrar estado desconocido si faltan lecturas recientes o falla el sensor.
- Considerar después el envío de un aviso a una pantalla central.

## Documentos

- [Especificación del piloto](specs/001-observar-sustrato/spec.md).
- [Método y arquitectura compartida](docs/metodologia.md).

## Próximas decisiones

Planta y maceta de prueba; ubicación de sonda; tecnología de sensor; alimentación; calibración; frecuencia de lectura; umbral tras observar datos reales; canal de aviso local.

