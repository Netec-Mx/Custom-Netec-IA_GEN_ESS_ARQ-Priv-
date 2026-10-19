# Laboratorio 2. Clínica de prompts: construir, probar y refinar un conjunto de prompts reutilizables para situaciones reales del trabajo, incorporando criterios de calidad y verificación

## Descripción General

Construirás y refinarás prompts reutilizables para situaciones reales de trabajo.

## Objetivos de Aprendizaje

- construir prompts estructurados;
- añadir restricciones;
- refinar respuestas;
- crear criterios de calidad.

## Prerrequisitos

### Acceso Requerido

Microsoft 365 Copilot Chat y documento de notas.

### Configuración Inicial

Abre un bloc de notas en tu equipo, copia y pega el siguiente contenido. 

```jsonl
{"prompt": "Clasifica el siguiente documento y da una recomendación de tratamiento.\n\nDocumento: 'Informe preliminar de la auditoría fiscal externa 2026, señalando posibles inconsistencias graves en la contabilidad y riesgo inminente de sanción por parte de la DIAN.'", "completion": "{\n  "clasificacion": "Crítico",\n  "recomendacion": "Restringir el acceso exclusivamente al Comité Directivo y equipo legal. Almacenar en repositorio cifrado de extremo a extremo, prohibir su reenvío por correo externo y aplicar destrucción segura tras el cierre del caso."\n}"}
{"prompt": "Clasifica el siguiente documento y da una recomendación de tratamiento.\n\nDocumento: 'Propuesta comercial detallada con tarifas preferenciales y condiciones contractuales exclusivas negociadas para el cliente clave Banco de Bogotá.'", "completion": "{\n  "clasificacion": "Confidencial",\n  "recomendacion": "Compartir únicamente con el equipo comercial asignado y los tomadores de decisiones del cliente. Asegurar el uso de acuerdos de confidencialidad (NDA) vigentes y evitar su almacenamiento en dispositivos personales."\n}"}
{"prompt": "Clasifica el siguiente documento y da una recomendación de tratamiento.\n\nDocumento: 'Cronograma y lineamientos generales para el evento de integración de fin de año de los empleados de la sucursal de Bogotá.'", "completion": "{\n  "clasificacion": "Información interna",\n  "recomendacion": "Distribuir a través de los canales de comunicación interna habituales de la compañía (intranet o correo corporativo). No requiere medidas de cifrado estrictas, pero no debe compartirse con personas ajenas a la organización."\n}"}
{"prompt": "Clasifica el siguiente documento y da una recomendación de tratamiento.\n\nDocumento: 'Nota de prensa oficial anunciando el lanzamiento de nuestra nueva línea eco-amigable de productos disponible para todo público en la web corporativa.'", "completion": "{\n  "clasificacion": "Público",\n  "recomendacion": "Apto para distribución libre y masiva en canales externos, redes sociales y medios de comunicación. No requiere restricciones de acceso ni medidas especiales de protección."\n}"}
```

Luego en el Bloc de Notas haz clic en Archivo - Guardar como... - 

* **Nombre:** ClasificadorDocumentosFewShot.jsonl
* **Tipo:** Todos los archivos (*.*)

---

## Paso 1: Usa las mejores prácticas de Ingeniería de prompt

Imagina que eres un líder de equipo que quiere usar un asistente de IA para preparar material motivacional y organizativo después de terminar un proyecto importante. Al inicio, tu prompt es muy básico, pero progresivamente lo vamos refinando.

Ingresa a Microsoft 365 Copilot en tu navegador `https://m365.cloud.microsoft`

1. Prompt sin contexto. El usuario pide algo genérico, sin dar detalles.

Prompt: `Escribe un mensaje motivador.`

Problema: La IA no sabe para quién, ni en qué situación, ni qué tono usar.

3. Añadir contexto Se especifica quién eres y en qué situación estás.

Prompt: `Soy líder de un equipo que acaba de terminar un proyecto importante. Escribe un mensaje motivador para ellos.`

Mejora: Ahora la IA entiende el rol y el escenario.

4. Definir objetivo. Se aclara qué se busca lograr con el mensaje.

Prompt: `Soy líder de un equipo que acaba de terminar un proyecto importante. Escribe un mensaje motivador para agradecerles y reforzar la confianza en futuros proyectos.`

Mejora: La IA sabe que debe incluir agradecimiento y proyección.

4. Ubicación del contenido. Se indica dónde se usará el resultado (correo, presentación, etc.).

Prompt: `Soy líder de un equipo que acaba de terminar un proyecto importante. Escribe un mensaje motivador para agradecerles y reforzar la confianza en futuros proyectos. El mensaje será enviado por correo electrónico.`

Mejora: La IA ajusta tono y extensión al canal.

5. Tipo de salida. Se define el formato esperado (párrafo, lista, tabla, etc.).

Prompt: `Soy líder de un equipo que acaba de terminar un proyecto importante. Escribe un mensaje motivador para agradecerles y reforzar la confianza en futuros proyectos. El mensaje será enviado por correo electrónico y debe estar en un solo párrafo breve.`

Mejora: La IA entrega exactamente el formato deseado.

✨ **Resultado del ejercicio**
Con este flujo, se ve cómo un prompt pasa de ser ambiguo a ser preciso y útil, gracias a la inclusión progresiva de:

📌 Contexto → quién eres y situación

🎯 Objetivo → qué quieres lograr

🗂️ Ubicación del contenido → dónde se usará

📝 Tipo de salida → formato esperado


## Paso 2: Experimenta one-shot, few-shot y CTO en un escenario empresarial

1. Usemos one-shot. Escoge un documento dentro de tu equipo y súbelo a MS365 Copilot.

2. Envía el siguiente Prompt.

```text
Clasifica el documento adjunto
```

3. Observa el resultado y anótalo.

4. Usemos few-shot. No es necesario que salgas de la sesión de chat anterior ni que vuelvas a cargar el documento

5. Sube la plantilla que creaste en el inicio de este laboratorio. **ClasificadorDocumentosFewShot.jsonl**.

6. Con la plantilla cargada envía el siguiente Prompt:

```text
Clasifica nuevamente el documento tomando como base los ejemplos adjuntos en la plantilla.
```

7. Observa los resultados, anótalos y documenta también la diferencia entre ambos. 

8. Usemos COT. Usando la misma sesión de chat, pídele el paso a paso del razonamiento para llegar a dicho resultado. Envía el siguiente Prompt:

```text
Quiero ver tu cadena de pensamiento (COT), enumera cada paso detallado para llegar a la clasificación anterior.
```

9. Observa el resultado, verifica si el razonamiento que hizo incumple con algún procedimiento o política de tu empresa. De ser así, puedes darle el feedback.

---

## Paso 3: Comprobar mantener contexto y usar refinamiento

1. Abre una nueva sesión de chat en Microsoft 365 Copilot.

2. Envía el siguiente Prompt:

```text
Quisiera contextualizarme sobre la situación geopolítica actual, busca en noticias actuales y confiables, lista los tres puntos más relevantes.
```

3. Observa el resultado, y modifica la forma de responder. Envía el siguiente Prompt:

```text
Muy bien, es justo lo que buscaba, pero quisiera que los emojis inicien por un Emoji.
```

4. Observa los resultados, seguramente ahora verás que la lista inicia con Emojis.

5. Continua tu investigación. Solicita lo siguiente:

```text
Excelente, era justo lo que quería. Ahora, genera una lista de los cinco aspectos clave que dichas noticias afectan a Colombia.  
```

6. El resultado debería estar alineado con la respuesta anterior (dichas noticias) y debería usar emojis aunque no se mencionó explícitamente en el nuevo Prompt. 

---

## Paso 4: Reforzar el concepto de Tokens, Embeddibgs y seguridad en Microsoft 365 Copilot

1. Envía la siguiente solicitud

```text
Si te hago una pregunta, te puedo pedir que la respuesta se devuelva en tokes o embeddings, es decir las representaciones numéricas?
```

2. Analiza la respuesta, debería decirte que sí puede generar respuestas codificadas pero no darte los valores numéricos reales. Esto es por temas de seguridad.

3. Ahora enviemos una prueba.

```text
Cómo se vería la representación tokenizada de la frase: "Mi perro es blanco y mi gato es negro". Muéstralos como IDs numéricos.
```

4. Observa cómo se ven representados los Tokens.

5. Ahora, pídele que te muestre dichos tokens como embeddings.

```text
Ahora muestrame estos IDs numéricos cómo se verían ubicados en un índice vectorial, además genera los embeddings.
```

6. Observa la explicación y el resultado.

7. Finalmente, vas a comparar dos frases para comprender mejor los conceptos de Tokens y embeddings.

```text
Genera tokens y embeddings para la frase: "El banco negó el préstamo por error". Y genera una gráfica bidimensional donde se vea la diferencia de las ubicaciones semánticas en el índice de las dos frases. Finamente, en un párrafo sintetiza el concepto de tokens y embeddings y su impacto en mi trabajo diario.
```

8. Observa el resultado. Seguramente, en el párrafo final, Microsoft 365 Copilot personaliza su respuesta alineado a tu perfil, rol o puesto, verifica que sea así.

> ⚠️**Nota:** Si el último párrafo de la respuesta no menciona tu rol, cargo o perfil y de acuerdo a esto genera el resultado puede deberse a la varianza del modelo o restricciones de tu empresa para que Copilot acceda a tu perfil.

¡Felicitaciones! 🥳 Terminaste el laboratorio correctamente.

---

## Solución de Problemas

### Problema 1: La respuesta no sigue el formato solicitado

**Síntoma:** La respuesta no sigue el formato solicitado.

**Causa probable:** El formato se expresó de manera ambigua.

**Solución:** Enumera explícitamente las secciones, columnas o elementos que debe contener.
### Problema 2: La respuesta cambia demasiado entre intentos

**Síntoma:** La respuesta cambia demasiado entre intentos.

**Causa probable:** El prompt deja abiertas demasiadas decisiones.

**Solución:** Añade restricciones, prioridades y criterios de salida.
### Problema 3: Los ejemplos contaminan la respuesta

**Síntoma:** Los ejemplos contaminan la respuesta.

**Causa probable:** No quedó claro que son solo un patrón.

**Solución:** Indica que Copilot debe imitar la estructura o el tono, pero no copiar hechos de los ejemplos.

---

## Limpieza

1. Cierra la conversación de práctica si ya no la necesitas.
2. Elimina o evita conservar datos de práctica que no deban reutilizarse.
3. Conserva únicamente prompts, tablas o patrones que puedan reutilizarse de forma segura.
4. Si trabajaste con un archivo proporcionado, sigue las políticas de tu organización para su almacenamiento o eliminación.

> **Nota:** estas actividades no requieren desinstalar software ni eliminar configuraciones del equipo. La limpieza se enfoca en conversaciones, archivos y datos utilizados durante la práctica.

---

## Resumen

| Fase | Logro |
|---|---|
| Solicitud | Partiste de una necesidad de trabajo. |
| Estructura | Añadiste objetivo, contexto, expectativas y fuente. |
| Experimentación | Probaste variantes y refinamientos. |
| Reutilización | Construiste un prompt más consistente. |

### Conceptos Clave Reforzados

- Un prompt útil puede combinar objetivo, contexto, expectativas y fuente.
- Formato y restricciones ayudan a reducir ambigüedad.
- Los ejemplos orientan, pero no siempre son necesarios.
- Un prompt reutilizable debe poder entenderse fuera de la conversación original.

### Recursos Adicionales

- [Introducción a la escritura de prompts en Microsoft Copilot](https://support.microsoft.com/en-us/microsoft-365-copilot/get-started-writing-prompts-in-microsoft-365-copilot)
- [Cómo escribir mejores prompts en Microsoft Copilot](https://support.microsoft.com/en-us/microsoft-365-copilot/write-a-great-prompt-in-microsoft-365-copilot)
