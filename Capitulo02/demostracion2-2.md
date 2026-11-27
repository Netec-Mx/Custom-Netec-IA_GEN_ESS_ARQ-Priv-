# Demostración guiada 2.2. Construir un prompt template para reutilizar y para prompting few-shot

El propósito de este documento es sugerir la demostración que el instructor puede realizar durante la entrega del segundo capitulo del curso Fundamentos IA Gen Priv. Los siguientes pasos son generales, se entiende que el instructor tiene las habilidades para comprenderlo. Están organizados en orden de los slides de Power Point adjuntos.

## Instrucciones

**Prompt template reutilizable**

* Ingresa a microsoft 365 copilot
* Solicita la creación en formato jsonl de un template para que sea reutilizado en distintos escenarios
* copia el resultado en un bloc de notas
* realiza las modificaciones pertinentes.
* pregunta a los estudiantes qué otros cambios creen que requiere
* guardalo en formato json
* compartelo en el chat de la sesión

**prompt template para few-shot**

* experimenta con un objetivo para zero-shot, one-shot y few-shot
* por ejemplo, análisis de sentimientos.
* crea un prompt template para adjuntarlo como ejemplos para few-shot para que obtenga los ejemplos del documento.
* por ejemplo para el análisis de los sentimientos quedaría algo así. (el sentimiento no se menciona explicito, sino se codifica en un número.

```json
{"text": "¡Me encantó este producto! Superó todas mis expectativas y el servicio fue excelente.", "sentiment": "positivo", "code": 777}
{"text": "Pésimo servicio, el artículo llegó roto y nadie se hizo responsable. No lo recomiendo.", "sentiment": "negativo", "code": 666}
{"text": "El paquete llegó hoy a las 3:00 PM. Es una caja de cartón estándar.", "sentiment": "neutro", "code": 6767}
{"text": "La atención al cliente fue rapida y muy amable. Volvería a comprar sin duda.", "sentiment": "positivo", "code": 777}
{"text": "La calidad del material es terrible y la app falla constantemente.", "sentiment": "negativo", "code": 666}
{"text": "El dispositivo incluye cable de carga y manual de instrucciones.", "sentiment": "neutro", "code": 6767}
```

* explica el formato a los estudiantes y pídeles escenarios que podrían usarlos.
