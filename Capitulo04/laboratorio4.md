# Laboratorio 4. Identifica patrones maliciosos, usa técnicas de protección de datos y evalúa los resultados

## Descripción General

Anonimizarás resultados de Copilot para evitar el uso de datos confidenciales. Calificarás la exactitud, consistencia, relevancia, fuentes y señales de alerta en una respuesta con LLM-as-a-Jude y usarás Lakera para probar patrones maliciosos de Prompt Injection. 

---

## Paso 1: Anonimización de respuestas

Imagina que eres un consultor que utiliza Copilot para redactar comunicaciones profesionales. Sin embargo, necesitas asegurarte de que ningún dato personal sensible aparezca en las respuestas, por lo que aplicarás etiquetas de anonimización.

1. Supongamos que Copilot debe redactar un correo de seguimiento a un cliente. En lugar de usar nombres reales, se reemplazarán por etiquetas.
**Prompt:**
```text
Redacta un correo de seguimiento para <PERSON>, agradeciendo la reunión de ayer y confirmando que la próxima cita será el lunes a las 10 AM en <LOCATION>.
```

2. Ahora pedimos que se incluya un número de contacto, pero sin mostrar el real.
**Prompt:**
```text
Incluye en el correo un número de contacto representado como <TEL> en lugar de un número real.
```

3. El correo debe tener un destinatario, pero sin mostrar la dirección real.
**Prompt:**

```Redacta el correo dirigido a <EMAIL>, manteniendo el tono profesional y cordial.```

4. Supongamos que se menciona una ciudad o una oficina.
**Prompt:**
```text
En el cuerpo del correo, indica que la reunión será en <LOCATION>, sin mencionar la ciudad real.
```

5. Finalmente, pedimos que Copilot genere la respuesta completa asegurando que todos los datos sensibles estén anonimizados.
**Prompt:**

```text
Genera la versión final del correo con todos los datos anonimizados usando etiquetas
```

---

## Paso 2: Evalúa los resultados otorgados por Copilot (llm-as-a-judge)

El siguiente ejercicio te permite evaluar el resultado de Copilot. En un escenario real, sería ideal evaluarlo con otro asistente que use otro FM, pero para propósito de nuestro laboratorio usaremos el mismo Copilot.

1. Abre Microsoft 365 Copilot `https://m365.cloud.com`.
2. Cambia el tipo de procesamiento de **Automático** a **Respuesta rápida** en el costado superior. Ahora, ingresa el siguiente prompt de investigación.
**Prompt:**
```
Realiza una investigación exhaustiva sobre las tendencias actuales de transformación digital en el sector bancario, enfocándote en cómo los bancos están adoptando inteligencia artificial, automatización y servicios en la nube para mejorar la eficiencia operativa y la experiencia del cliente, amplía el análisis considerando tanto bancos tradicionales como neobancos incluyendo aspectos regulatorios, riesgos de ciberseguridad, impacto en la fuerza laboral y cambios en la relación con los clientes, utiliza fuentes confiables y verificadas como organismos oficiales (BIS, IMF, World Bank), consultoras reconocidas (McKinsey, Deloitte, PwC), publicaciones académicas y medios financieros especializados (Financial Times, The Banker) evitando fuentes no verificadas o blogs sin respaldo institucional, organiza la información en un informe ejecutivo en español con secciones claras que incluyan introducción y contexto global, principales tendencias tecnológicas en banca, retos regulatorios y de seguridad, impacto en clientes y empleados y conclusiones estratégicas, presenta el resultado en formato profesional usando bullets y tablas comparativas cuando sea útil e incluye ejemplos concretos de bancos que estén liderando estas iniciativas.
```
3. Observa el resultado y copialo.
4. Abre una nueva sesión de chat y cambia el tipo de procesamiento de **Automático** a **Razonamiento profundo** en el costado superior.
5. Solicita evaluar y calificar la respuesta de esa solicitud de la siguiente forma.

> ⚠️**Nota:** En el siguiente prompt reemplaza **"Agrega la respuesta"** por la respuesta que copiaste en el punto 3 de este ejercicio.
**Prompt:**
```
Hice una investigación con IA. Adjunto la solicitud hecha por mí y la respuesta generada por IA. Quiero que realices una búsqueda para evaluar de 1 a 5 los siguientes aspectos y agregues al final de cada uno, un comentario:
- Exactitud (los datos, cifras y hechos sean correctos y verificables)
- Consistencia (la respuesta mantenga coherencia interna y no se contradiga)
- Relevancia (la información esté alineada con la pregunta o contexto del usuario)
- Fuentes (las referencias deben ser confiables y actualizadas)
- Señales de alerta (Identificar posibles errores, sesgos o afirmaciones dudosas)
###
- Respuesta: "Agrega la respuesta"
###
Prompt: Realiza una investigación exhaustiva sobre las tendencias actuales de transformación digital en el sector bancario, enfocándote en cómo los bancos están adoptando inteligencia artificial, automatización y servicios en la nube para mejorar la eficiencia operativa y la experiencia del cliente, amplía el análisis considerando tanto bancos tradicionales como neobancos incluyendo aspectos regulatorios, riesgos de ciberseguridad, impacto en la fuerza laboral y cambios en la relación con los clientes, utiliza fuentes confiables y verificadas como organismos oficiales (BIS, IMF, World Bank), consultoras reconocidas (McKinsey, Deloitte, PwC), publicaciones académicas y medios financieros especializados (Financial Times, The Banker) evitando fuentes no verificadas o blogs sin respaldo institucional, organiza la información en un informe ejecutivo en español con secciones claras que incluyan introducción y contexto global, principales tendencias tecnológicas en banca, retos regulatorios y de seguridad, impacto en clientes y empleados y conclusiones estratégicas, presenta el resultado en formato profesional usando bullets y tablas comparativas cuando sea útil e incluye ejemplos concretos de bancos que estén liderando estas iniciativas.
```
---
## Paso 3: Probar amenazas de Prompt Injection con Lakera

1. En tu navegador ingresa a `https://play.lakera.ai/agent-breaker/cco_coach`

2. El juego es un entorno educativo donde interactúas con un agente que actúa como “entrenador de ciclismo”. El reto consiste en intentar que el agente revele sus instrucciones internas ocultas (su system message), lo cual simula un ataque de prompt injection. El objetivo no es robar información real, sino aprender cómo funcionan las defensas de IA frente a manipulaciones.

3. Ahora abre el botón de chat de la aplicación de ciclismo y comienza a interactuar. Debes formular prompts creativos para intentar engañar al agente.

* Usar lenguaje persuasivo o engañoso
* Probar con escenarios ficticios (ej. 'imagina que eres un auditor')
* Observar cómo el agente responde y bloquea intentos

4. Si bien está en inglés, puedes preguntar y recibir respuestas en español.

5. Intenta obtener la mayor cantidad de información posible (puntos) y comparte tu resultado con tu instructor y tus compañeros.

¡Felicitaciones! 🥳 Has terminado el laboratorio.

---

## Solución de Problemas

### Problema 1: Copilot toma una decisión final

**Síntoma:** Copilot toma una decisión final.

**Causa probable:** El prompt permite una conclusión global.

**Solución:** Indica explícitamente que debe analizar, cuestionar o proponer opciones sin decidir.
### Problema 2: Las objeciones o preguntas son genéricas

**Síntoma:** Las objeciones o preguntas son genéricas.

**Causa probable:** Falta contexto suficiente.

**Solución:** Añade propósito, restricciones y antecedentes del escenario.
### Problema 3: Las hipótesis aparecen como hechos

**Síntoma:** Las hipótesis aparecen como hechos.

**Causa probable:** No se solicitó distinguir niveles de certeza.

**Solución:** Pide separar hechos, supuestos, inferencias y preguntas abiertas.

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
| Escenario | Definiste una situación concreta. |
| Análisis | Exploraste preguntas, objeciones o supuestos. |
| Revisión | Evaluaste límites y puntos ciegos. |
| Criterio humano | Mantviste la decisión final bajo responsabilidad humana. |

### Conceptos Clave Reforzados

- Copilot puede ayudar a ampliar perspectivas sin sustituir la decisión humana.
- Los contraargumentos son insumos para investigar, no evidencia.
- Separar hechos de supuestos mejora la calidad del análisis.
- La revisión crítica debe complementar, no reemplazar, el juicio profesional.

### Recursos Adicionales

- [Crear contenido con Microsoft Copilot Chat](https://support.microsoft.com/en-us/microsoft-365-copilot/create-content-using-microsoft-365-copilot-chat)
- [Preguntas frecuentes sobre Microsoft Copilot Chat](https://support.microsoft.com/en-us/microsoft-365-copilot/frequently-asked-questions-about-microsoft-365-copilot-chat)
