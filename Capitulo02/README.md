# Laboratorio 2. Clínica de prompts en Copilot Chat: mejorar solicitudes reales mediante iteración, estructura, zero-shot y few-shot

## Metadatos

| Campo | Detalle |
|---|---|
| **Duración** | 75 minutos |
| **Complejidad** | Media |
| **Nivel Bloom** | Aplicar |

## Descripción General

En este laboratorio transformarás necesidades laborales vagas en prompts estructurados y efectivos para Microsoft 365 Copilot Chat, aplicando el marco **Objetivo-Contexto-Expectativas-Fuente** junto con técnicas zero-shot, one-shot y few-shot. Partiendo de las tareas identificadas en tu mapa de oportunidades del Laboratorio 1, ejecutarás ciclos completos de diagnóstico, reestructuración, refinamiento conversacional y generación de múltiples formatos de salida. Al finalizar, consolidarás una biblioteca personal de prompts reutilizables en un documento `.docx` que servirá como referencia para el Laboratorio 3.

## Objetivos de Aprendizaje

Al completar este laboratorio serás capaz de:

- [ ] Transformar necesidades laborales vagas en prompts estructurados aplicando el marco Objetivo-Contexto-Expectativas-Fuente, complementado con rol, formato, restricciones y tono.
- [ ] Aplicar la técnica zero-shot para tareas directas y las técnicas one-shot y few-shot para tareas que requieren orientar el estilo, formato o nivel de detalle de la respuesta.
- [ ] Ejecutar al menos dos ciclos completos de refinamiento conversacional sobre un mismo objetivo, mejorando iterativamente la respuesta mediante correcciones, profundizaciones y ajustes de formato.
- [ ] Generar al menos tres formatos de salida distintos (lista, tabla, resumen ejecutivo) a partir del mismo contenido fuente, utilizando restricciones de formato en el prompt.
- [ ] Construir una biblioteca personal de prompts reutilizables para al menos tres tareas recurrentes identificadas en el Laboratorio 1.

## Prerrequisitos

### Conocimientos previos

| Requisito | Descripción |
|---|---|
| Laboratorio 1 completado | Contar con el mapa de oportunidades y riesgos (`LAB01_plantilla_mapa_oportunidades_v1.docx`) con al menos cinco tareas identificadas y clasificadas por nivel de riesgo. |
| Demo 01-00-02 observada | Haber actualizado el mapa con aprendizajes de buenas prácticas de la demostración del instructor. |
| Conceptos de la Lección 2.1 | Comprender los cuatro pasos para transformar una necesidad en un prompt efectivo: identificar la necesidad real, añadir contexto relevante, especificar el resultado esperado y revisar antes de enviar. |
| Elementos clave de un prompt | Conocer los cinco elementos: Qué, Para quién, Por qué, Cómo y Restricciones. |

### Acceso y recursos

| Recurso | Detalle |
|---|---|
| Cuenta Microsoft 365 | Cuenta corporativa con licencia de Microsoft 365 Copilot Chat habilitada (verificada al menos 24 horas antes). |
| Copilot Chat | Acceso funcional a [https://copilot.microsoft.com](https://copilot.microsoft.com) en modo **Trabajo (Work)**. |
| Plantilla de biblioteca | Archivo `LAB02_plantilla_biblioteca_prompts_v1.docx` proporcionado por el instructor. |
| Mapa del Laboratorio 1 | Archivo `LAB01_plantilla_mapa_oportunidades_v1.docx` completado con al menos cinco tareas. |
| Navegador compatible | Microsoft Edge 124+ o Google Chrome 124+. |
| Microsoft Word | Microsoft 365 Apps for Enterprise, versión 2404 o superior. |

## Entorno de Laboratorio

### Hardware mínimo

| Componente | Especificación |
|---|---|
| Procesador | 64 bits, Intel Core i5 / AMD Ryzen 5 o superior |
| RAM | 8 GB mínimo (16 GB recomendado) |
| Pantalla | Resolución mínima 1366×768 (1920×1080 recomendado) |
| Conexión a Internet | 5 Mbps de bajada por participante (10 Mbps recomendado) |
| Periféricos | Teclado y ratón funcionales |

### Software requerido

| Software | Versión | Propósito |
|---|---|---|
| Microsoft Edge o Google Chrome | Edge 124.0.2478.97+ / Chrome 124.0.6367.119+ | Navegador para acceder a Copilot Chat |
| Microsoft 365 Copilot Chat (Web) | Servicio activo a mayo 2025 | Plataforma principal del laboratorio |
| Microsoft Word | Microsoft 365 Apps, versión 2404 (Build 17531.20152)+ | Editar la plantilla de biblioteca de prompts |
| Editor de texto plano | Notepad (Windows) o TextEdit (macOS) | Notas auxiliares durante el laboratorio |

### Configuración inicial

1. Abre el navegador (Edge o Chrome) y navega a [https://copilot.microsoft.com](https://copilot.microsoft.com).
2. Inicia sesión con tu cuenta corporativa de Microsoft 365.
3. Verifica que el selector de modo en la parte superior de la interfaz muestre **Trabajo** (Work). Si muestra **Web**, haz clic en el selector y cambia a **Trabajo**.
4. Abre en Microsoft Word el archivo `LAB01_plantilla_mapa_oportunidades_v1.docx` (tu mapa completado del Laboratorio 1).
5. Abre en Microsoft Word el archivo `LAB02_plantilla_biblioteca_prompts_v1.docx` (plantilla vacía proporcionada por el instructor).
6. Organiza tu pantalla con Copilot Chat en una mitad y Word en la otra (usa la función de ajuste de ventanas con `Win + ←` / `Win + →` en Windows, o arrastra a los bordes en macOS).

> **Nota para el instructor:** Antes de iniciar, confirme que todos los participantes ven el modo **Trabajo** disponible en Copilot Chat. Si algún participante no lo ve, verifique el estado de la licencia con el administrador de TI.

## Instrucciones Paso a Paso

### Paso 1: Seleccionar tareas del mapa de oportunidades (8 minutos)

**Objetivo:** Identificar de tres a cinco tareas de bajo o medio riesgo del Laboratorio 1 que servirán como base para toda la práctica de prompting de este laboratorio.

**Instrucciones:**

1. Abre tu archivo `LAB01_plantilla_mapa_oportunidades_v1.docx` en Microsoft Word.
2. Revisa la lista completa de tareas que identificaste en el Laboratorio 1. Localiza la columna o sección donde clasificaste cada tarea por nivel de riesgo (bajo, medio, alto).
3. Selecciona **entre tres y cinco tareas** que cumplan estos criterios:
   - Clasificadas como **riesgo bajo o medio**.
   - Representan actividades que realizas con frecuencia en tu rol profesional.
   - Son lo suficientemente variadas para explorar diferentes tipos de prompt (por ejemplo: redactar un correo, resumir información, generar una lista de ideas, crear una agenda, elaborar un reporte).
4. En tu archivo `LAB02_plantilla_biblioteca_prompts_v1.docx`, localiza la sección **"Tareas seleccionadas"** y registra cada tarea seleccionada con el siguiente formato:

   | # | Tarea | Tipo de actividad | Nivel de riesgo | Frecuencia |
   |---|---|---|---|---|
   | 1 | Redactar correo de seguimiento a cliente después de reunión | Comunicación escrita | Bajo | Semanal |
   | 2 | Resumir los puntos clave de un informe de avance de proyecto | Síntesis de información | Bajo | Quincenal |
   | 3 | Generar una agenda estructurada para reunión de equipo | Planificación | Medio | Semanal |

5. Si tienes menos de tres tareas de bajo o medio riesgo, consulta con el instructor para redefinir alguna tarea de riesgo alto como una versión simplificada de menor riesgo.

**Resultado esperado:** Una tabla con tres a cinco tareas concretas documentadas en la plantilla, cada una con su tipo de actividad, nivel de riesgo y frecuencia.

**Verificación:**
- [ ] La tabla contiene entre 3 y 5 tareas.
- [ ] Todas las tareas están clasificadas como riesgo bajo o medio.
- [ ] Cada tarea describe una actividad concreta (no genérica como "usar IA para trabajar mejor").
- [ ] Las tareas representan al menos dos tipos diferentes de actividad.

---

### Paso 2: Escribir prompts vagos y diagnosticar respuestas débiles (12 minutos)

**Objetivo:** Experimentar de primera mano cómo un prompt vago produce respuestas genéricas o inútiles, y documentar las deficiencias específicas de cada respuesta para crear una línea base de comparación.

**Instrucciones:**

1. En Copilot Chat (modo **Trabajo**), inicia una **nueva conversación** haciendo clic en el botón **"Nuevo chat"** (icono de lápiz o `+` en la esquina superior).
2. Para la **primera tarea** de tu tabla, escribe deliberadamente un prompt vago, breve y sin contexto. El objetivo es simular cómo escribiríamos si no conociéramos técnicas de prompting. Ejemplos de prompts vagos según tipo de tarea:

   - Para redactar un correo: `Escribe un correo sobre la reunión.`
   - Para resumir un informe: `Resume el informe.`
   - Para generar una agenda: `Haz una agenda.`
   - Para crear un reporte: `Necesito un reporte de avance.`

3. Envía el prompt y **espera la respuesta completa** de Copilot Chat.
4. Lee la respuesta detenidamente y evalúa su calidad utilizando los siguientes criterios de diagnóstico:

   | Criterio de diagnóstico | Pregunta de evaluación | Calificación (Sí/No/Parcial) |
   |---|---|---|
   | **Relevancia** | ¿La respuesta aborda exactamente mi necesidad laboral real? | |
   | **Especificidad** | ¿Contiene detalles concretos de mi situación o es genérica? | |
   | **Formato útil** | ¿El formato de la respuesta es el que necesito para usarla directamente? | |
   | **Tono adecuado** | ¿El tono es apropiado para mi audiencia y contexto? | |
   | **Listo para usar** | ¿Podría usar esta respuesta tal cual, sin ediciones significativas? | |

5. En tu plantilla `LAB02_plantilla_biblioteca_prompts_v1.docx`, localiza la sección **"Diagnóstico de prompts"** y registra para esta primera tarea:
   - El prompt vago exacto que escribiste.
   - Un resumen de la respuesta obtenida (2-3 líneas).
   - La evaluación con los cinco criterios de diagnóstico.
   - Una nota breve sobre **qué falta** en el prompt (ejemplo: "No especifiqué quién es el destinatario ni el motivo del correo").

6. Repite los sub-pasos 1 a 5 para **al menos dos tareas más** de tu tabla (inicia un nuevo chat para cada tarea).
7. Al finalizar las tres evaluaciones, identifica el **patrón común** de las deficiencias. Escribe una oración que resuma qué elementos suelen faltar en tus prompts iniciales.

**Resultado esperado:** Para cada tarea evaluada, un registro completo en la plantilla que incluye: el prompt vago, el resumen de la respuesta, la evaluación con cinco criterios y la identificación de lo que falta. Además, una oración resumen del patrón de deficiencias.

**Verificación:**
- [ ] Se probaron al menos 3 prompts vagos, uno por tarea seleccionada.
- [ ] Cada prompt vago tiene su evaluación de cinco criterios documentada.
- [ ] Se identificó al menos una deficiencia concreta por cada prompt.
- [ ] Se escribió una oración resumen del patrón común de deficiencias.

---

### Paso 3: Reescribir prompts con el marco Objetivo-Contexto-Expectativas-Fuente (15 minutos)

**Objetivo:** Aplicar el marco estructurado **Objetivo-Contexto-Expectativas-Fuente (OCEF)**, complementado con rol, formato, restricciones y tono, para transformar cada prompt vago en una instrucción precisa y accionable, y comparar cualitativamente la mejora.

**Instrucciones:**

1. Antes de reescribir, revisa el marco OCEF ampliado que utilizarás:

   | Componente | Descripción | Ejemplo |
   |---|---|---|
   | **Objetivo** | ¿Qué tarea concreta debe realizar Copilot? | "Redacta un correo de seguimiento" |
   | **Contexto** | ¿Cuál es la situación, quién eres, para quién es? | "Soy coordinador de proyectos. El correo es para el cliente Acme después de la reunión del martes donde se acordaron tres compromisos." |
   | **Expectativas** | ¿Qué formato, extensión, tono y nivel de detalle esperas? | "Tono profesional y cordial. Máximo 4 párrafos. Incluir los tres compromisos como lista numerada." |
   | **Fuente** | ¿Hay información específica que Copilot debe usar? | "Los compromisos son: (1) enviar propuesta revisada el viernes, (2) confirmar presupuesto antes del 20 de junio, (3) agendar siguiente reunión para la semana del 24 de junio." |
   | **Rol** *(complemento)* | ¿Qué rol debe asumir Copilot al responder? | "Actúa como un redactor de comunicaciones corporativas." |
   | **Restricciones** *(complemento)* | ¿Qué debe evitar o no incluir? | "No menciones problemas internos del equipo ni uses jerga técnica." |

2. Toma la **primera tarea** de tu diagnóstico del Paso 2. Inicia una **nueva conversación** en Copilot Chat (modo Trabajo).
3. Reescribe el prompt vago aplicando el marco OCEF completo. Asegúrate de incluir al menos los cuatro componentes principales (Objetivo, Contexto, Expectativas, Fuente) y al menos uno de los complementos (Rol, Restricciones o Tono).

   **Ejemplo de transformación:**

   *Prompt vago original:*
   ```
   Escribe un correo sobre la reunión.
   ```

   *Prompt estructurado con OCEF:*
   ```
   Actúa como un redactor de comunicaciones corporativas.

   Objetivo: Redacta un correo de seguimiento post-reunión.

   Contexto: Soy coordinadora de proyectos en una empresa de consultoría.
   Ayer tuve una reunión con el cliente Acme Corp para revisar el avance
   del Proyecto Atlas. En la reunión se acordaron tres compromisos clave.

   Fuente — Los compromisos acordados son:
   1. Nuestro equipo enviará la propuesta revisada el viernes 13 de junio.
   2. Acme confirmará el presupuesto aprobado antes del 20 de junio.
   3. Se agendará la siguiente reunión de seguimiento para la semana del
      24 de junio.

   Expectativas:
   - Tono profesional y cordial.
   - Máximo 4 párrafos.
   - Incluir los tres compromisos como lista numerada dentro del cuerpo
     del correo.
   - Cerrar con una línea de disponibilidad para consultas.

   Restricciones: No mencionar problemas internos del equipo ni usar
   jerga técnica.
   ```

4. Envía el prompt estructurado y espera la respuesta completa.
5. Evalúa la nueva respuesta con los **mismos cinco criterios** del Paso 2 (Relevancia, Especificidad, Formato útil, Tono adecuado, Listo para usar).
6. En tu plantilla, documenta en la sección **"Comparación de prompts"**:
   - El prompt estructurado completo.
   - Un resumen de la nueva respuesta (2-3 líneas).
   - La evaluación con los cinco criterios.
   - Una nota de **comparación directa**: ¿en qué mejoró respecto al prompt vago?

7. Repite los sub-pasos 2 a 6 para **al menos dos tareas más**.
8. Al finalizar las tres comparaciones, escribe una reflexión breve (2-3 oraciones) sobre cuál de los componentes del marco OCEF tuvo el mayor impacto en la mejora de las respuestas para tus tareas específicas.

**Resultado esperado:** Tres o más prompts estructurados documentados con su evaluación comparativa, mostrando mejora cualitativa respecto a los prompts vagos. Una reflexión sobre el componente de mayor impacto.

**Verificación:**
- [ ] Se reescribieron al menos 3 prompts usando el marco OCEF.
- [ ] Cada prompt estructurado incluye al menos los 4 componentes principales (O, C, E, F).
- [ ] La evaluación comparativa muestra mejora en al menos 3 de los 5 criterios por cada prompt.
- [ ] Se documentó la reflexión sobre el componente de mayor impacto.

---

### Paso 4: Explorar técnicas zero-shot, one-shot y few-shot (15 minutos)

**Objetivo:** Aplicar las tres técnicas de prompting basadas en ejemplos (zero-shot, one-shot, few-shot) a tareas diferentes, documentando cuándo cada técnica produce mejores resultados según el tipo de tarea.

**Instrucciones:**

1. Revisa las definiciones de cada técnica antes de comenzar:

   | Técnica | Definición | Cuándo usarla |
   |---|---|---|
   | **Zero-shot** | Se da la instrucción sin ningún ejemplo. Copilot genera la respuesta basándose solo en la descripción de la tarea. | Tareas directas y bien definidas donde el formato o estilo esperado es estándar (ej.: resumir un texto, responder una pregunta factual). |
   | **One-shot** | Se incluye **un ejemplo** del resultado esperado antes de pedir la tarea. | Cuando necesitas que Copilot siga un formato, estilo o estructura específica que no es obvio solo con la instrucción. |
   | **Few-shot** | Se incluyen **dos o más ejemplos** del resultado esperado antes de pedir la tarea. | Cuando el patrón es complejo, el formato tiene reglas específicas o necesitas consistencia alta entre múltiples resultados. |

2. **Ejercicio Zero-shot:** Selecciona una tarea de tu tabla que sea directa y bien definida (por ejemplo: resumir información, generar una lista de ideas o redactar un mensaje breve). Inicia un **nuevo chat** en Copilot Chat y escribe un prompt estructurado (usando OCEF) **sin incluir ningún ejemplo** del resultado esperado.

   *Ejemplo de prompt zero-shot:*
   ```
   Objetivo: Genera una lista de 5 riesgos potenciales para un proyecto
   de migración de datos en una empresa de servicios financieros.

   Contexto: Soy gerente de proyectos y necesito presentar esta lista
   en la reunión de comité de riesgos del próximo jueves.

   Expectativas: Cada riesgo debe incluir una descripción de una línea
   y una categoría (técnico, operativo, regulatorio o de recursos).
   Formato de tabla con columnas: #, Riesgo, Descripción, Categoría.

   Restricciones: No incluir riesgos financieros de mercado, solo
   riesgos operativos del proyecto.
   ```

3. Envía el prompt, revisa la respuesta y cópiala en tu plantilla bajo la sección **"Técnicas Shot — Zero-shot"**.

4. **Ejercicio One-shot:** Selecciona una tarea diferente donde el formato o estilo sea importante (por ejemplo: redactar descripciones de producto, crear entradas de un glosario, o escribir retroalimentación para un colaborador). Inicia un **nuevo chat** y escribe un prompt que incluya **un ejemplo concreto** del resultado que esperas.

   *Ejemplo de prompt one-shot:*
   ```
   Objetivo: Redacta descripciones breves para tres cursos de
   capacitación interna.

   Contexto: Soy coordinadora de desarrollo organizacional. Las
   descripciones se publicarán en la intranet corporativa para que
   los empleados se inscriban.

   Ejemplo del formato y estilo que necesito:
   ---
   **Excel Avanzado para Analistas**
   Duración: 8 horas | Modalidad: Virtual sincrónica
   Aprende a crear tablas dinámicas, macros básicas y dashboards
   interactivos para transformar datos en decisiones. Dirigido a
   analistas y coordinadores que usan Excel diariamente.
   ---

   Ahora genera descripciones con el mismo formato y estilo para
   estos tres cursos:
   1. Gestión del Tiempo con Outlook
   2. Presentaciones Ejecutivas con PowerPoint
   3. Fundamentos de Ciberseguridad para No Técnicos

   Restricciones: Máximo 3 líneas de descripción por curso. Tono
   profesional pero accesible.
   ```

5. Envía el prompt, revisa la respuesta y cópiala en tu plantilla bajo **"Técnicas Shot — One-shot"**.

6. **Ejercicio Few-shot:** Usando la **misma tarea** del ejercicio one-shot (o una tarea similar que requiera consistencia), inicia un **nuevo chat** y ahora incluye **dos o tres ejemplos** antes de la solicitud.

   *Ejemplo de prompt few-shot (fragmento de los ejemplos):*
   ```
   Objetivo: Redacta descripciones breves para dos cursos adicionales
   de capacitación interna.

   Contexto: Soy coordinadora de desarrollo organizacional. Las
   descripciones se publicarán en la intranet corporativa.

   Aquí tienes tres ejemplos del formato y estilo exacto que necesito:

   Ejemplo 1:
   **Excel Avanzado para Analistas**
   Duración: 8 horas | Modalidad: Virtual sincrónica
   Aprende a crear tablas dinámicas, macros básicas y dashboards
   interactivos para transformar datos en decisiones. Dirigido a
   analistas y coordinadores que usan Excel diariamente.

   Ejemplo 2:
   **Gestión del Tiempo con Outlook**
   Duración: 4 horas | Modalidad: Virtual sincrónica
   Domina las funciones de calendario, tareas y reglas de correo
   para organizar tu jornada y reducir interrupciones. Ideal para
   cualquier profesional que gestione múltiples compromisos.

   Ejemplo 3:
   **Presentaciones Ejecutivas con PowerPoint**
   Duración: 6 horas | Modalidad: Presencial
   Diseña presentaciones claras y persuasivas aplicando principios
   de comunicación visual y storytelling. Dirigido a líderes y
   profesionales que presentan ante comités o clientes.

   Ahora genera descripciones con el mismo formato para:
   1. Liderazgo de Equipos Remotos
   2. Introducción a Power BI para Gerentes

   Restricciones: Mantener exactamente el mismo formato, extensión
   y tono de los ejemplos.
   ```

7. Envía el prompt, revisa la respuesta y cópiala en tu plantilla bajo **"Técnicas Shot — Few-shot"**.

8. **Análisis comparativo:** Completa la siguiente tabla en tu plantilla:

   | Aspecto | Zero-shot | One-shot | Few-shot |
   |---|---|---|---|
   | ¿Siguió el formato esperado? | | | |
   | ¿Mantuvo el tono deseado? | | | |
   | ¿La respuesta era consistente en estilo? | | | |
   | ¿Requirió edición posterior? | | | |
   | **Mejor técnica para esta tarea** | | | |

9. Escribe una conclusión de 2-3 oraciones sobre cuándo usarías cada técnica en tu trabajo diario.

**Resultado esperado:** Tres prompts ejecutados (uno por técnica), sus respuestas documentadas, la tabla comparativa completada y una conclusión personal.

**Verificación:**
- [ ] Se ejecutó al menos un prompt zero-shot con respuesta documentada.
- [ ] Se ejecutó al menos un prompt one-shot con un ejemplo incluido.
- [ ] Se ejecutó al menos un prompt few-shot con dos o más ejemplos incluidos.
- [ ] La tabla comparativa está completa con evaluaciones para las tres técnicas.
- [ ] Se escribió la conclusión sobre cuándo usar cada técnica.

---

### Paso 5: Refinamiento conversacional y generación de múltiples formatos (15 minutos)

**Objetivo:** Ejecutar al menos dos ciclos de refinamiento conversacional sobre un mismo prompt, mejorando iterativamente la respuesta, y generar tres formatos de salida distintos (lista, tabla, resumen ejecutivo) a partir del mismo contenido.

**Instrucciones:**

1. Selecciona el **mejor prompt** que hayas creado en los Pasos 3 o 4 — aquel cuya respuesta fue más útil pero que aún tiene espacio de mejora.

2. Inicia un **nuevo chat** en Copilot Chat (modo Trabajo) y envía ese prompt. Espera la respuesta completa.

3. **Primer ciclo de refinamiento — Corrección y profundización:** Lee la respuesta y formula un mensaje de seguimiento **en la misma conversación** (no inicies un chat nuevo). El mensaje debe pedir una corrección o profundización específica. Ejemplos de mensajes de refinamiento:

   ```
   La respuesta es buena, pero necesito que:
   1. Amplíes el punto 3 con más detalle sobre los plazos específicos.
   2. Cambies el tono del segundo párrafo para que sea más directo
      y menos formal.
   3. Elimines la mención a "mejores prácticas generales" y la
      reemplaces con acciones concretas para nuestro contexto.
   ```

4. Envía el mensaje de refinamiento y espera la respuesta actualizada.

5. **Segundo ciclo de refinamiento — Cambio de formato a LISTA:** En la misma conversación, envía el siguiente mensaje:

   ```
   Ahora transforma toda la información anterior en una lista con
   viñetas organizada por prioridad (de mayor a menor importancia).
   Cada punto debe tener máximo 2 líneas. Incluye un encabezado
   descriptivo para la lista.
   ```

6. Copia la respuesta en formato lista en tu plantilla bajo **"Formatos de salida — Lista"**.

7. **Tercer ciclo — Cambio de formato a TABLA:** En la misma conversación, envía:

   ```
   Ahora presenta la misma información como una tabla con las
   siguientes columnas: Elemento, Descripción, Prioridad, Fecha
   límite (si aplica). Ordena de mayor a menor prioridad.
   ```

8. Copia la respuesta en formato tabla en tu plantilla bajo **"Formatos de salida — Tabla"**.

9. **Cuarto ciclo — Cambio de formato a RESUMEN EJECUTIVO:** En la misma conversación, envía:

   ```
   Finalmente, condensa toda la información en un resumen ejecutivo
   de máximo 5 oraciones dirigido a un director que tiene 2 minutos
   para leerlo. Destaca solo las decisiones clave y los próximos pasos.
   ```

10. Copia la respuesta en formato resumen ejecutivo en tu plantilla bajo **"Formatos de salida — Resumen ejecutivo"**.

11. **Reflexión sobre el refinamiento:** En tu plantilla, responde estas preguntas:
    - ¿En qué ciclo de refinamiento la respuesta mejoró más significativamente?
    - ¿Cuál de los tres formatos sería más útil para tu tarea específica y por qué?
    - ¿Qué aprendiste sobre cómo Copilot Chat mantiene el contexto dentro de una misma conversación?

**Resultado esperado:** Una conversación con al menos 4 turnos de interacción (prompt inicial + 3 refinamientos), tres formatos de salida documentados (lista, tabla, resumen ejecutivo) y reflexión escrita.

**Verificación:**
- [ ] Se ejecutaron al menos 2 ciclos de refinamiento en la misma conversación (corrección/profundización + al menos un cambio de formato).
- [ ] Se generaron los tres formatos de salida: lista, tabla y resumen ejecutivo.
- [ ] Los tres formatos contienen esencialmente la misma información presentada de forma diferente.
- [ ] La reflexión sobre el refinamiento está completa con las tres preguntas respondidas.

---

### Paso 6: Construir la biblioteca personal de prompts reutilizables (10 minutos)

**Objetivo:** Consolidar los mejores prompts creados durante el laboratorio en una biblioteca personal estructurada, documentada en el archivo `.docx`, que sirva como referencia reutilizable para el trabajo diario y para el Laboratorio 3.

**Instrucciones:**

1. Abre tu archivo `LAB02_plantilla_biblioteca_prompts_v1.docx` y localiza la sección **"Biblioteca de Prompts Reutilizables"**.

2. Revisa todos los prompts que creaste en los Pasos 3, 4 y 5. Selecciona los **tres mejores prompts** — aquellos que produjeron las respuestas más útiles y que corresponden a tareas que realizas con frecuencia.

3. Para cada prompt seleccionado, completa la siguiente ficha en la plantilla:

   #### Ficha de Prompt Reutilizable — Modelo

   ```
   ╔══════════════════════════════════════════════════════════════╗
   ║  PROMPT #[número]                                           ║
   ╠══════════════════════════════════════════════════════════════╣
   ║  Nombre descriptivo: [ej.: "Correo de seguimiento post-     ║
   ║  reunión con cliente"]                                      ║
   ║                                                             ║
   ║  Tarea recurrente: [descripción de la tarea laboral]        ║
   ║                                                             ║
   ║  Frecuencia de uso: [diaria / semanal / quincenal /         ║
   ║  mensual]                                                   ║
   ║                                                             ║
   ║  Técnica utilizada: [zero-shot / one-shot / few-shot]       ║
   ║                                                             ║
   ║  Prompt completo:                                           ║
   ║  [Copiar aquí el prompt exacto tal como lo enviarías a      ║
   ║  Copilot Chat, incluyendo todos los componentes OCEF]       ║
   ║                                                             ║
   ║  Variables a personalizar: [Listar qué partes del prompt    ║
   ║  deben cambiarse cada vez que se use. Ej.: nombre del       ║
   ║  cliente, fecha de la reunión, compromisos acordados]       ║
   ║                                                             ║
   ║  Formato de salida esperado: [lista / tabla / resumen /     ║
   ║  correo / otro]                                             ║
   ║                                                             ║
   ║  Consejo de refinamiento: [Qué mensaje de seguimiento       ║
   ║  sueles necesitar para ajustar la respuesta. Ej.: "Pedir    ║
   ║  que reduzca a 3 párrafos" o "Solicitar tono más informal"] ║
   ╚══════════════════════════════════════════════════════════════╝
   ```

4. Completa las tres fichas con tus mejores prompts. Asegúrate de que las **variables a personalizar** estén claramente marcadas — esto es lo que hace al prompt verdaderamente reutilizable.

5. Después de las tres fichas, completa el **Checklist de Prompts Efectivos** en la plantilla:

   | # | Criterio | ¿Lo aplico? (Sí/No) |
   |---|---|---|
   | 1 | Mi prompt incluye un objetivo claro y específico | |
   | 2 | Proporcioné contexto sobre mi rol, audiencia o situación | |
   | 3 | Especifiqué el formato de salida esperado | |
   | 4 | Incluí restricciones sobre lo que NO debe contener | |
   | 5 | Definí el tono adecuado para la audiencia | |
   | 6 | Proporcioné datos fuente cuando la tarea lo requiere | |
   | 7 | Incluí ejemplos cuando el formato o estilo no es estándar | |
   | 8 | Revisé el prompt antes de enviarlo para eliminar ambigüedades | |
   | 9 | Planeo al menos un ciclo de refinamiento si la primera respuesta no es perfecta | |
   | 10 | Verifico la respuesta antes de usarla en una comunicación o decisión real | |

6. Guarda el archivo `LAB02_plantilla_biblioteca_prompts_v1.docx` con tus tres fichas y el checklist completados.

**Resultado esperado:** Un archivo `.docx` con tres fichas de prompts reutilizables completamente documentadas y el checklist de 10 criterios marcado.

**Verificación:**
- [ ] La biblioteca contiene exactamente 3 fichas de prompts reutilizables.
- [ ] Cada ficha tiene todos los campos completados, incluyendo las variables a personalizar.
- [ ] Los prompts en las fichas son versiones finales (ya mejoradas con el marco OCEF y refinamiento).
- [ ] El checklist de 10 criterios está completado.
- [ ] El archivo está guardado y listo para usarse como referencia en el Laboratorio 3.

## Validación y Pruebas

Al finalizar todos los pasos, verifica que cumples con los siguientes criterios de completitud del laboratorio:

| # | Criterio de validación | Estado |
|---|---|---|
| 1 | Seleccionaste entre 3 y 5 tareas de bajo o medio riesgo del mapa del Lab 1 | ☐ |
| 2 | Escribiste y documentaste al menos 3 prompts vagos con sus respuestas y diagnóstico | ☐ |
| 3 | Reescribiste al menos 3 prompts con el marco OCEF y documentaste la comparación | ☐ |
| 4 | Ejecutaste al menos un prompt con cada técnica: zero-shot, one-shot y few-shot | ☐ |
| 5 | Completaste la tabla comparativa de las tres técnicas shot | ☐ |
| 6 | Realizaste al menos 2 ciclos de refinamiento conversacional en una misma sesión de chat | ☐ |
| 7 | Generaste 3 formatos de salida diferentes (lista, tabla, resumen ejecutivo) del mismo contenido | ☐ |
| 8 | Tu biblioteca contiene 3 fichas de prompts reutilizables completamente documentadas | ☐ |
| 9 | El checklist de prompts efectivos está completado | ☐ |
| 10 | El archivo `LAB02_plantilla_biblioteca_prompts_v1.docx` está guardado con todo el contenido | ☐ |

**Prueba final de funcionalidad:** Toma uno de los tres prompts de tu biblioteca, ábrelo en un **nuevo chat** de Copilot Chat, reemplaza las variables con datos ficticios diferentes a los que usaste durante el laboratorio, y envíalo. Si la respuesta es útil y relevante sin necesidad de modificar la estructura del prompt, tu prompt es verdaderamente reutilizable.

## Solución de Problemas

### Problema 1: Copilot Chat no muestra la opción de modo "Trabajo" (Work)

**Síntomas:** Al acceder a [https://copilot.microsoft.com](https://copilot.microsoft.com), el selector de modo solo muestra "Web" o no aparece ningún selector. El participante no puede cambiar al modo Trabajo requerido para el laboratorio.

**Causa:** La cuenta del participante no tiene asignada la licencia de Microsoft 365 Copilot Chat, o la licencia fue asignada hace menos de 24 horas y aún no se ha propagado. También puede ocurrir si el participante inició sesión con una cuenta personal de Microsoft en lugar de la cuenta corporativa.

**Solución:**
1. Verifica que estás usando tu **cuenta corporativa** (no una cuenta personal @outlook.com o @hotmail.com). Haz clic en tu avatar en la esquina superior derecha de Copilot Chat y confirma que el correo mostrado es tu dirección corporativa.
2. Si la cuenta es correcta pero no aparece el modo Trabajo, cierra sesión completamente: haz clic en tu avatar → **Cerrar sesión**. Cierra todas las pestañas del navegador. Abre una nueva ventana del navegador y navega a [https://copilot.microsoft.com](https://copilot.microsoft.com). Inicia sesión nuevamente.
3. Si el problema persiste, abre una pestaña de navegación privada/incógnito (`Ctrl + Shift + N` en Chrome, `Ctrl + Shift + P` en Edge), navega a la URL e inicia sesión.
4. Si ninguna de las opciones anteriores funciona, notifica al instructor para que contacte al administrador de TI y verifique el estado de la licencia. Mientras se resuelve, puedes avanzar con los Pasos 1 y 2 del laboratorio documentando los prompts en la plantilla Word sin enviarlos a Copilot Chat.

---

### Problema 2: Copilot Chat genera respuestas en inglés a pesar de que el prompt está en español

**Síntomas:** El participante escribe el prompt completo en español, pero Copilot Chat responde parcial o totalmente en inglés. Esto ocurre especialmente con prompts que contienen términos técnicos en inglés (como nombres de productos, frameworks o acrónimos).

**Causa:** Copilot Chat infiere el idioma de respuesta a partir de múltiples señales, incluyendo la configuración regional de la cuenta Microsoft 365, el idioma del navegador y el contenido del prompt. Si la cuenta o el navegador están configurados en inglés, o si el prompt contiene una proporción significativa de texto en inglés (por ejemplo, en los ejemplos de few-shot), Copilot puede responder en inglés.

**Solución:**
1. Añade una **restricción explícita de idioma** al final de tu prompt:
   ```
   Restricción de idioma: Responde completamente en español
   latinoamericano. Todos los encabezados, descripciones y
   contenido deben estar en español.
   ```
2. Si ya enviaste el prompt y la respuesta vino en inglés, envía un mensaje de seguimiento en la misma conversación:
   ```
   Por favor, regenera la respuesta anterior completamente en
   español latinoamericano, manteniendo el mismo contenido
   y formato.
   ```
3. Para prevenir el problema en futuros prompts, verifica la configuración de idioma de tu navegador: en Edge, ve a `edge://settings/languages` y asegúrate de que **Español** esté como idioma preferido. En Chrome, ve a `chrome://settings/languages`.
4. Incorpora la restricción de idioma como parte estándar de tus fichas de prompts reutilizables si trabajas en un entorno donde la configuración regional puede variar.

## Limpieza

1. **Guardar el archivo final:** Asegúrate de que `LAB02_plantilla_biblioteca_prompts_v1.docx` está guardado con todo el contenido completado (tareas seleccionadas, diagnóstico, comparaciones, técnicas shot, formatos de salida, biblioteca de 3 prompts y checklist).
2. **Conservar el archivo del Laboratorio 1:** No modifiques ni elimines `LAB01_plantilla_mapa_oportunidades_v1.docx`, ya que se utilizará como referencia en el Laboratorio 3.
3. **Historial de conversaciones en Copilot Chat:** No es necesario eliminar las conversaciones creadas durante el laboratorio. Puedes conservarlas como referencia. Sin embargo, si deseas organizar tu historial, puedes renombrar las conversaciones más relevantes haciendo clic en el menú de tres puntos (`...`) junto a cada conversación y seleccionando **Renombrar**. Sugerencia de nomenclatura: `Lab02 - [nombre de la tarea]`.
4. **No se requiere desinstalación de software** ni cambios en la configuración del sistema.

## Resumen

En este laboratorio practicaste el ciclo completo de mejora de prompts para Microsoft 365 Copilot Chat:

- **Diagnosticaste** por qué los prompts vagos producen respuestas genéricas al experimentar directamente con instrucciones sin contexto.
- **Aplicaste** el marco Objetivo-Contexto-Expectativas-Fuente (OCEF) para transformar necesidades vagas en instrucciones precisas, verificando cualitativamente la mejora en cada caso.
- **Diferenciaste** cuándo usar zero-shot (tareas directas), one-shot (cuando el formato importa) y few-shot (cuando se requiere consistencia alta), documentando evidencia de la efectividad de cada técnica.
- **Refinaste** respuestas iterativamente dentro de una misma conversación, descubriendo que Copilot Chat mantiene el contexto y permite correcciones, profundizaciones y cambios de formato sin repetir toda la instrucción.
- **Generaste** tres formatos de salida (lista, tabla, resumen ejecutivo) a partir del mismo contenido, ampliando tu repertorio de posibilidades para adaptar resultados a diferentes audiencias.
- **Construiste** una biblioteca personal de tres prompts reutilizables que podrás aplicar inmediatamente en tu trabajo y que servirá como base para el Laboratorio 3.

### Recursos adicionales

| Recurso | Enlace |
|---|---|
| Documentación de Microsoft: Consejos para escribir prompts efectivos en Copilot | [https://learn.microsoft.com/es-es/copilot/microsoft-365/prompting-tips](https://learn.microsoft.com/es-es/copilot/microsoft-365/prompting-tips) |
| Microsoft Copilot Adoption Hub: Principios de prompting | [https://adoption.microsoft.com/es-es/copilot/](https://adoption.microsoft.com/es-es/copilot/) |
| Investigación de Microsoft: El contexto lo es todo en Copilot | [https://www.microsoft.com/en-us/worklab/ai-data-drop-when-it-comes-to-copilot-context-is-everything](https://www.microsoft.com/en-us/worklab/ai-data-drop-when-it-comes-to-copilot-context-is-everything) |
| Guía de Microsoft 365 Copilot Chat: Casos de uso | [https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-overview](https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-overview) |

---

# Demo: Demostración guiada: resolver el mismo objetivo con un prompt vago, un prompt estructurado y un prompt con ejemplos

## Metadatos

| Campo | Detalle |
|---|---|
| **Duración** | 20 minutos |
| **Complejidad** | Fácil |
| **Nivel Bloom** | Aplicar |
| **Tipo de actividad** | Demostración del instructor |
| **Tecnologías** | Microsoft 365 Copilot Chat (copilot.microsoft.com), Microsoft Edge 124+, Proyector / pantalla compartida |

## Descripción General

En esta demostración, el instructor resuelve un mismo objetivo de negocio —redactar un correo de seguimiento post-reunión para un cliente— tres veces consecutivas utilizando niveles crecientes de calidad de prompt: un prompt vago, un prompt estructurado con el marco Objetivo-Contexto-Expectativas-Fuente y un prompt con ejemplos (few-shot). Los participantes observan cómo cada mejora en la instrucción produce un cambio visible y medible en la calidad de la respuesta de Copilot Chat, y toman notas de las decisiones de diseño que aplicarán en el Laboratorio 2.

> ℹ️ **Nota:** Esta práctica es una **Demostración realizada por el instructor**. El instructor ejecutará los pasos y comandos mientras los alumnos observan, toman notas y analizan el procedimiento, en lugar de realizarla individualmente.

## Objetivos de Aprendizaje

Al finalizar esta demostración, los participantes serán capaces de:

- [ ] Observar en tiempo real cómo la calidad y utilidad de la respuesta de Copilot Chat varía significativamente según la estructura y nivel de detalle del prompt utilizado.
- [ ] Identificar los elementos específicos del marco Objetivo-Contexto-Expectativas-Fuente que producen mayor impacto en la calidad de la respuesta, según lo demostrado por el instructor.
- [ ] Comparar visualmente las respuestas obtenidas con prompt vago, prompt estructurado y prompt con ejemplos (few-shot) sobre el mismo objetivo de negocio.
- [ ] Tomar nota de al menos dos decisiones de diseño de prompt que el instructor justifica en voz alta durante la demostración, para aplicarlas en el Laboratorio 2.

## Prerrequisitos

### Conocimientos previos

| Requisito | Descripción |
|---|---|
| Laboratorio 1 completado | Los participantes deben haber finalizado el Lab 01-00-01 y la Demo 01-00-02, donde se familiarizaron con la interfaz de Copilot Chat y el concepto básico de prompt. |
| Lección 2.1 | Los participantes deben haber estudiado los conceptos de claridad, contexto y los cuatro pasos para transformar una necesidad en un prompt efectivo. |
| Marco de prompt | Conocimiento introductorio de los elementos: Objetivo, Contexto, Expectativas, Fuente, Rol, Formato, Restricciones y Tono. |

### Acceso y recursos del instructor

| Recurso | Detalle |
|---|---|
| Cuenta Microsoft 365 con licencia Copilot Chat | Verificada y funcional al menos 24 horas antes de la sesión. |
| Navegador Microsoft Edge 124+ | Actualizado y con sesión iniciada en la cuenta corporativa del instructor. |
| Proyector o pantalla compartida | Resolución mínima 1920×1080, visible para todos los participantes. |
| Materiales preparados | Los tres prompts redactados previamente (ver sección de instrucciones) y los dos textos de ejemplo para el prompt few-shot. |

### Materiales para los participantes

| Recurso | Detalle |
|---|---|
| Cuaderno o editor de texto | Para tomar notas de las decisiones de diseño observadas. |
| Archivo `LAB02_plantilla_biblioteca_prompts_v1.docx` | Distribuido previamente; los participantes lo usarán en el Laboratorio 2 posterior. |

## Entorno de Laboratorio

### Equipo del instructor

| Componente | Especificación |
|---|---|
| Sistema operativo | Windows 11 22H2 o superior |
| Navegador | Microsoft Edge 124.0.2478.97 o superior |
| RAM disponible | Mínimo 8 GB (16 GB recomendado) |
| Conexión a Internet | Mínimo 10 Mbps de bajada |
| Resolución de pantalla | 1920×1080 (proyectada) |

### Configuración previa del instructor

1. Abrir Microsoft Edge e iniciar sesión con la cuenta corporativa que tiene licencia de Microsoft 365 Copilot Chat.
2. Navegar a **https://copilot.microsoft.com**.
3. Verificar que el selector de modo muestra **Trabajo** (Work). Si muestra "Web", hacer clic en el selector y cambiar a "Trabajo".
4. Confirmar que la interfaz carga correctamente y que el campo de entrada de prompt está visible.
5. Abrir un documento de texto (Notepad o equivalente) con los tres prompts preparados y los dos textos de ejemplo, para poder copiarlos rápidamente durante la demostración.
6. Verificar que el proyector o la pantalla compartida muestra la ventana del navegador con tamaño de fuente legible para todos los participantes. Si es necesario, aumentar el zoom del navegador a 125 % o 150 %.

### Escenario de negocio para la demostración

El instructor utilizará el siguiente escenario ficticio a lo largo de las tres iteraciones:

> **Escenario:** Eres gerente de cuentas en una empresa de consultoría tecnológica llamada **NovaTech Solutions**. Ayer tuviste una reunión de 45 minutos con el equipo de TI de tu cliente **Grupo Meridian** para revisar el avance del proyecto de migración a la nube. En la reunión se acordaron tres puntos: (1) la fecha de migración del servidor principal se mantiene el 28 de junio, (2) Grupo Meridian enviará las credenciales de acceso al entorno de pruebas antes del viernes 13 de junio, y (3) NovaTech presentará un informe de riesgos actualizado el lunes 16 de junio. Necesitas enviar un correo de seguimiento profesional al contacto principal del cliente, **Lic. Andrea Fuentes, Directora de Tecnología**.

## Instrucciones Paso a Paso

### Paso 1: Preparar el escenario y contextualizar a los participantes

**Objetivo:** Establecer el escenario de negocio compartido que se usará en las tres iteraciones, de modo que los participantes comprendan el objetivo antes de ver los prompts.

**Instrucciones:**

1. Proyectar la pantalla del navegador con Copilot Chat abierto en modo **Trabajo**.
2. Explicar en voz alta el escenario de negocio (ver recuadro en la sección "Entorno de Laboratorio"):
   - *"Imaginen que soy gerente de cuentas en NovaTech Solutions. Ayer tuve una reunión con mi cliente Grupo Meridian sobre un proyecto de migración a la nube. Ahora necesito enviar un correo de seguimiento a la Directora de Tecnología, Andrea Fuentes, confirmando los tres acuerdos de la reunión."*
3. Indicar a los participantes que abran su cuaderno o editor de texto para tomar notas.
4. Anunciar la estructura de la demostración:
   - *"Voy a resolver este mismo objetivo tres veces. Primero con un prompt vago, luego con un prompt estructurado y finalmente con un prompt que incluye ejemplos. Quiero que observen las diferencias en las respuestas y anoten qué decisiones de diseño producen mejoras."*
5. Pedir a los participantes que presten atención específica a:
   - El tono de cada respuesta.
   - La presencia o ausencia de los datos concretos (fechas, nombres, compromisos).
   - La extensión y el formato.
   - La utilidad real: ¿podrían enviar esa respuesta tal cual?

**Resultado esperado:** Los participantes comprenden el escenario de negocio y saben qué observar durante las tres iteraciones.

**Verificación:** Preguntar brevemente: *"¿Queda claro el escenario? ¿Cuántos acuerdos se tomaron en la reunión?"* Confirmar que responden "tres".

---

### Paso 2: Ejecutar el prompt vago (Iteración 1)

**Objetivo:** Demostrar cómo un prompt sin contexto ni estructura produce una respuesta genérica e inutilizable.

**Instrucciones:**

1. En Copilot Chat (modo **Trabajo**), escribir el siguiente prompt exactamente como aparece, sin añadir nada más:

```
Escribe un correo de seguimiento de una reunión con un cliente.
```

2. Presionar **Enter** y esperar la respuesta completa de Copilot Chat.
3. **No** cerrar ni limpiar el chat todavía. Dejar la respuesta visible en pantalla.
4. Leer la respuesta en voz alta para los participantes.
5. Analizar la respuesta señalando las siguientes limitaciones (narrar cada observación en voz alta):

   - **Ambigüedad del contenido:** *"Observen que Copilot no sabe quién es el cliente, qué se discutió ni qué se acordó. Ha inventado un contenido genérico que no corresponde a nuestra reunión real."*
   - **Tono indefinido:** *"El tono puede ser demasiado casual o demasiado formal. No le dimos indicación, así que eligió uno por defecto."*
   - **Formato arbitrario:** *"La extensión y la estructura del correo las decidió el modelo. Puede ser demasiado largo o demasiado corto para nuestro propósito."*
   - **Inutilizable sin edición:** *"¿Podría enviar este correo tal cual a la Lic. Andrea Fuentes? Claramente no. Tendría que reescribir casi todo."*

6. Hacer una pausa de 15 segundos para que los participantes terminen de anotar.
7. Verbalizar la **decisión de diseño clave** de este paso:
   - *"La lección aquí es que cuando no proporcionamos contexto, Copilot llena los vacíos con suposiciones genéricas. El prompt no respondió ninguna de las cinco preguntas clave: qué, para quién, por qué, cómo, ni restricciones."*

**Resultado esperado:** Copilot Chat genera un correo genérico de seguimiento que no menciona a NovaTech Solutions, Grupo Meridian, Andrea Fuentes, ni los tres acuerdos específicos. El correo probablemente incluye marcadores de posición como "[Nombre del cliente]" o contenido inventado no relacionado con el escenario.

**Verificación:** Preguntar a los participantes: *"¿Cuántos de los tres acuerdos de nuestra reunión aparecen en esta respuesta?"* La respuesta esperada es "ninguno" o "cero".

---

### Paso 3: Ejecutar el prompt estructurado (Iteración 2)

**Objetivo:** Demostrar cómo aplicar el marco Objetivo-Contexto-Expectativas produce una respuesta significativamente más útil y específica.

**Instrucciones:**

1. Iniciar un **nuevo chat** en Copilot Chat haciendo clic en el botón **"Nuevo chat"** (icono de conversación nueva) para evitar que el contexto de la iteración anterior influya en la respuesta.
2. Verificar que el modo sigue siendo **Trabajo**.
3. Antes de escribir el prompt, explicar en voz alta la estructura que se va a usar:
   - *"Ahora voy a aplicar el marco que vimos en la Lección 2.1. Voy a incluir: un rol, el objetivo concreto, el contexto de la situación, las expectativas de formato y tono, y las restricciones."*
4. Escribir (o pegar desde el documento preparado) el siguiente prompt:

```
Rol: Eres un asistente de redacción ejecutiva para un gerente de cuentas en una empresa de consultoría tecnológica.

Objetivo: Redacta un correo electrónico de seguimiento post-reunión dirigido a un cliente corporativo.

Contexto:
- Empresa: NovaTech Solutions (nosotros, la consultora).
- Cliente: Grupo Meridian.
- Destinataria: Lic. Andrea Fuentes, Directora de Tecnología de Grupo Meridian.
- Reunión: Ayer, 45 minutos, revisión del avance del proyecto de migración a la nube.
- Acuerdos alcanzados:
  1. La fecha de migración del servidor principal se mantiene el 28 de junio.
  2. Grupo Meridian enviará las credenciales de acceso al entorno de pruebas antes del viernes 13 de junio.
  3. NovaTech presentará un informe de riesgos actualizado el lunes 16 de junio.

Formato: Correo electrónico profesional con saludo, cuerpo con los tres acuerdos en lista numerada, y cierre cordial.

Tono: Profesional, cordial y orientado a la acción.

Restricciones:
- Máximo 200 palabras.
- No incluir jerga técnica.
- No mencionar costos ni presupuestos.
- Firmar como "Carlos Méndez, Gerente de Cuentas, NovaTech Solutions".
```

5. Presionar **Enter** y esperar la respuesta completa.
6. Leer la respuesta en voz alta.
7. **Comparar explícitamente** con la respuesta del Paso 2, señalando las mejoras concretas:

   - **Datos específicos presentes:** *"Ahora aparecen los tres acuerdos con fechas exactas: 28 de junio, 13 de junio y 16 de junio. Esto es porque los incluimos en el contexto."*
   - **Nombres correctos:** *"La destinataria es Andrea Fuentes, la empresa es Grupo Meridian. No hay marcadores de posición."*
   - **Tono adecuado:** *"El tono es profesional y cordial, exactamente lo que pedimos. Compárenlo con el tono genérico de la primera respuesta."*
   - **Formato controlado:** *"Los acuerdos están en lista numerada, como solicitamos. La extensión se ajusta al límite de 200 palabras."*
   - **Utilizable directamente:** *"¿Podría enviar este correo tal cual? Con ajustes mínimos, sí. Esa es la diferencia."*

8. Verbalizar las **decisiones de diseño clave** de este paso:
   - *"Decisión 1: Incluir los acuerdos como lista dentro del prompt. Esto garantiza que aparezcan textualmente en la respuesta."*
   - *"Decisión 2: Especificar restricciones negativas — qué NO incluir. Decir 'no mencionar costos' evita que el modelo agregue información no deseada."*
   - *"Decisión 3: Definir el formato exacto — saludo, cuerpo con lista, cierre. Esto elimina la ambigüedad estructural."*

9. Hacer una pausa de 20 segundos para que los participantes anoten.

**Resultado esperado:** Copilot Chat genera un correo electrónico profesional dirigido a "Lic. Andrea Fuentes", firmado por "Carlos Méndez, Gerente de Cuentas, NovaTech Solutions", que incluye los tres acuerdos en lista numerada con las fechas correctas, en tono cordial y profesional, con una extensión aproximada de 150–200 palabras, sin jerga técnica ni mención de costos.

**Verificación:** Preguntar a los participantes:
- *"¿Cuántos de los tres acuerdos aparecen ahora?"* → Respuesta esperada: "los tres".
- *"¿Qué elemento del marco produjo la mayor mejora respecto al primer prompt?"* → Aceptar respuestas como "el contexto", "los acuerdos específicos" o "las restricciones".

---

### Paso 4: Ejecutar el prompt con ejemplos — few-shot (Iteración 3)

**Objetivo:** Demostrar cómo agregar ejemplos concretos dentro del prompt (técnica few-shot) permite que Copilot Chat replique un estilo, tono y estructura específicos que van más allá de lo que una instrucción descriptiva puede lograr.

**Instrucciones:**

1. Iniciar un **nuevo chat** en Copilot Chat.
2. Verificar que el modo sigue siendo **Trabajo**.
3. Explicar el concepto antes de ejecutar:
   - *"El prompt estructurado ya fue muy bueno, pero hay situaciones donde necesitamos que Copilot replique un estilo muy específico — por ejemplo, el estilo de comunicación que usamos en nuestra empresa. En lugar de describir ese estilo con palabras, le mostramos ejemplos. Esto se llama prompting few-shot: le damos al modelo dos o más ejemplos del resultado deseado para que aprenda el patrón."*
4. Escribir (o pegar) el siguiente prompt, que incluye los dos textos de ejemplo:

```
Rol: Eres un asistente de redacción ejecutiva para un gerente de cuentas en una empresa de consultoría tecnológica.

Objetivo: Redacta un correo electrónico de seguimiento post-reunión dirigido a un cliente corporativo.

Contexto:
- Empresa: NovaTech Solutions (nosotros, la consultora).
- Cliente: Grupo Meridian.
- Destinataria: Lic. Andrea Fuentes, Directora de Tecnología de Grupo Meridian.
- Reunión: Ayer, 45 minutos, revisión del avance del proyecto de migración a la nube.
- Acuerdos alcanzados:
  1. La fecha de migración del servidor principal se mantiene el 28 de junio.
  2. Grupo Meridian enviará las credenciales de acceso al entorno de pruebas antes del viernes 13 de junio.
  3. NovaTech presentará un informe de riesgos actualizado el lunes 16 de junio.

Formato: Correo electrónico profesional con saludo, cuerpo con los acuerdos en lista numerada, y cierre cordial con siguiente paso claro.

Tono: Profesional, cordial y orientado a la acción.

Restricciones:
- Máximo 200 palabras.
- No incluir jerga técnica.
- No mencionar costos ni presupuestos.
- Firmar como "Carlos Méndez, Gerente de Cuentas, NovaTech Solutions".

A continuación te muestro dos ejemplos del estilo de correo de seguimiento que utilizo habitualmente. Usa estos ejemplos como referencia para el tono, la estructura y el nivel de detalle:

--- EJEMPLO 1 ---
Asunto: Seguimiento reunión del 2 de mayo — Proyecto Orion

Estimada Ing. Valeria Rojas:

Gracias por el tiempo dedicado a nuestra reunión de ayer. Fue muy productivo revisar juntos el estado del Proyecto Orion.

Para asegurar que estemos alineados, confirmo los acuerdos alcanzados:

1. El lanzamiento piloto se mantiene para el 10 de julio.
2. Su equipo nos compartirá los datos de prueba antes del 20 de mayo.
3. Nosotros entregaremos el manual de usuario actualizado el 25 de mayo.

Quedo atento a cualquier ajuste. No duden en contactarme si surge alguna novedad antes de nuestra próxima sesión.

Saludos cordiales,
Carlos Méndez
Gerente de Cuentas, NovaTech Solutions
--- FIN EJEMPLO 1 ---

--- EJEMPLO 2 ---
Asunto: Seguimiento reunión del 18 de abril — Proyecto Zenith

Estimado Lic. Roberto Paredes:

Agradezco la reunión de ayer. El avance del Proyecto Zenith va por buen camino y me da gusto confirmar lo siguiente:

1. La integración con el sistema SAP se completará antes del 5 de mayo.
2. Su equipo de QA realizará las pruebas de aceptación entre el 6 y el 10 de mayo.
3. NovaTech entregará la documentación final el 12 de mayo.

Como siguiente paso, les enviaré el viernes un recordatorio con el checklist de actividades previas a la integración.

Quedo a sus órdenes.

Saludos cordiales,
Carlos Méndez
Gerente de Cuentas, NovaTech Solutions
--- FIN EJEMPLO 2 ---

Ahora redacta el correo de seguimiento para la reunión con Grupo Meridian usando el mismo estilo de los ejemplos anteriores.
```

5. Presionar **Enter** y esperar la respuesta completa.
6. Leer la respuesta en voz alta.
7. **Comparar las tres respuestas** lado a lado (si es posible, tener las respuestas anteriores visibles en pestañas separadas o en capturas de pantalla):

   - **Estilo replicado:** *"Observen que el correo ahora comienza con 'Estimada Lic. Andrea Fuentes' y usa la misma frase de agradecimiento que mis ejemplos. No le dije 'usa la palabra estimada' — lo aprendió del patrón."*
   - **Estructura idéntica:** *"La estructura es: saludo → agradecimiento → frase de transición → lista numerada → siguiente paso → despedida. Exactamente el patrón de los dos ejemplos."*
   - **Siguiente paso incluido:** *"En el prompt estructurado no mencioné un 'siguiente paso', pero en mis ejemplos siempre incluyo uno. Copilot detectó ese patrón y lo replicó. Esa es la potencia del few-shot."*
   - **Tono consistente:** *"El tono es más natural y más 'mío' que en la iteración anterior, porque el modelo tiene referencia concreta de cómo escribo."*
   - **Línea de asunto:** *"El modelo probablemente generó una línea de asunto con el mismo formato: 'Seguimiento reunión del [fecha] — Proyecto [nombre]'. Eso también lo aprendió de los ejemplos."*

8. Verbalizar las **decisiones de diseño clave** de este paso:
   - *"Decisión 1: Incluir exactamente dos ejemplos, no uno. Con dos ejemplos, el modelo puede identificar el patrón común en lugar de simplemente copiar un único texto."*
   - *"Decisión 2: Los ejemplos usan escenarios diferentes (Proyecto Orion y Proyecto Zenith) pero la misma estructura. Esto le dice al modelo qué es constante (la estructura) y qué es variable (los datos específicos)."*
   - *"Decisión 3: Mantuve todas las instrucciones del prompt estructurado además de los ejemplos. Los ejemplos complementan las instrucciones, no las reemplazan."*

9. Hacer una pausa de 20 segundos para que los participantes completen sus notas.

**Resultado esperado:** Copilot Chat genera un correo que replica fielmente el estilo de los dos ejemplos proporcionados: comienza con "Estimada Lic. Andrea Fuentes", incluye una frase de agradecimiento por la reunión, presenta los tres acuerdos en lista numerada con fechas, incluye un "siguiente paso" concreto, y cierra con "Saludos cordiales" y la firma de Carlos Méndez. La línea de asunto sigue el formato "Seguimiento reunión del [fecha] — Proyecto [nombre de proyecto]".

**Verificación:** Preguntar a los participantes:
- *"¿Qué elemento nuevo apareció en esta respuesta que no estaba en la del prompt estructurado?"* → Respuesta esperada: "el siguiente paso" o "la línea de asunto con formato específico".
- *"¿De dónde aprendió Copilot ese elemento?"* → Respuesta esperada: "de los ejemplos".

---

### Paso 5: Síntesis comparativa y checklist de prompts efectivos

**Objetivo:** Consolidar los aprendizajes de las tres iteraciones y proporcionar a los participantes un checklist práctico que usarán en el Laboratorio 2.

**Instrucciones:**

1. Proyectar (o dibujar en pizarra/pantalla) la siguiente tabla comparativa y narrarla en voz alta:

| Criterio | Prompt vago | Prompt estructurado | Prompt few-shot |
|---|---|---|---|
| **Datos específicos** | ❌ Ninguno | ✅ Los tres acuerdos con fechas | ✅ Los tres acuerdos con fechas |
| **Nombre del destinatario** | ❌ Genérico o marcador | ✅ Lic. Andrea Fuentes | ✅ Lic. Andrea Fuentes |
| **Tono controlado** | ⚠️ Aleatorio | ✅ Profesional y cordial | ✅ Consistente con estilo personal |
| **Formato predecible** | ❌ Arbitrario | ✅ Lista numerada solicitada | ✅ Estructura replicada de ejemplos |
| **Siguiente paso incluido** | ❌ No | ⚠️ Solo si se solicitó | ✅ Aprendido del patrón |
| **Utilizable sin edición** | ❌ No | ✅ Con ajustes mínimos | ✅ Prácticamente listo |
| **Esfuerzo de prompt** | Bajo (1 línea) | Medio (15–20 líneas) | Alto (40+ líneas con ejemplos) |
| **Esfuerzo de edición posterior** | Muy alto | Bajo | Mínimo |

2. Explicar la relación inversamente proporcional:
   - *"Observen el patrón: cuanto más esfuerzo invertimos en el prompt, menos esfuerzo necesitamos después para editar la respuesta. El tiempo total es menor cuando el prompt es bueno."*

3. Mostrar el **checklist de prompts efectivos** que los participantes usarán como referencia en el Laboratorio 2:

```
CHECKLIST DE PROMPTS EFECTIVOS
================================
Antes de enviar un prompt a Copilot Chat, verifica:

□ ¿Definí QUÉ necesito? (tarea concreta)
□ ¿Especifiqué PARA QUIÉN es el resultado? (audiencia)
□ ¿Expliqué POR QUÉ lo necesito? (propósito / situación)
□ ¿Indiqué CÓMO debe verse? (formato, extensión, estructura)
□ ¿Establecí el TONO adecuado? (formal, cordial, directo)
□ ¿Incluí RESTRICCIONES? (qué NO debe incluir)
□ ¿Asigné un ROL al asistente? (perspectiva desde la que responde)
□ ¿Agregué EJEMPLOS si necesito un estilo específico?
□ ¿Releí el prompt verificando que no sea ambiguo?
```

4. Pedir a los participantes que copien o fotografíen el checklist.

5. Cerrar la demostración con una reflexión final:
   - *"Las tres técnicas que vimos — prompt vago, estructurado y few-shot — no son 'buena, mejor y la mejor'. Son herramientas para diferentes situaciones. Si necesitan una lluvia de ideas rápida, un prompt simple puede servir. Si necesitan un entregable profesional con estilo específico, el few-shot es la herramienta correcta. La habilidad está en saber cuándo usar cada una."*

6. Indicar que en el **Laboratorio 2** (siguiente actividad), cada participante aplicará estas técnicas con su propio objetivo de negocio y su propia plantilla de biblioteca de prompts.

**Resultado esperado:** Los participantes tienen notas con al menos dos decisiones de diseño de prompt observadas durante la demostración y una copia del checklist de prompts efectivos.

**Verificación:** Pedir a dos o tres participantes que compartan en voz alta una decisión de diseño que anotaron. Ejemplos válidos:
- "Incluir los datos específicos dentro del prompt para que aparezcan en la respuesta."
- "Usar restricciones negativas para evitar contenido no deseado."
- "Proporcionar dos ejemplos con diferente contenido pero misma estructura."
- "Mantener las instrucciones explícitas incluso cuando se usan ejemplos."

## Validación y Pruebas

Al finalizar la demostración, el instructor debe verificar los siguientes criterios de éxito:

| # | Criterio de validación | Método de verificación | Resultado esperado |
|---|---|---|---|
| 1 | Las tres respuestas de Copilot Chat fueron visibles para todos los participantes. | Confirmación visual / preguntar a participantes del fondo del aula. | Todos confirman que pudieron leer las respuestas. |
| 2 | Los participantes pueden identificar al menos una diferencia entre la respuesta del prompt vago y la del prompt estructurado. | Pregunta directa a 2–3 participantes. | Mencionan diferencias concretas (datos específicos, tono, formato). |
| 3 | Los participantes pueden explicar qué aportaron los ejemplos en la tercera iteración. | Pregunta directa a 2–3 participantes. | Mencionan el estilo replicado, el "siguiente paso" o la línea de asunto. |
| 4 | Los participantes anotaron al menos dos decisiones de diseño de prompt. | Solicitar que levanten la mano quienes tienen dos o más notas. | Al menos el 80 % de los participantes levantan la mano. |
| 5 | Los participantes tienen una copia del checklist de prompts efectivos. | Confirmación verbal. | Todos confirman tenerlo copiado o fotografiado. |

## Solución de Problemas

### Problema 1: Copilot Chat no genera una respuesta diferenciada entre el prompt estructurado y el prompt few-shot

**Síntomas:** La respuesta del prompt few-shot (Iteración 3) es prácticamente idéntica a la del prompt estructurado (Iteración 2), sin replicar el estilo de los ejemplos proporcionados. Los participantes no perciben una mejora significativa.

**Causa:** El modelo puede no distinguir claramente los ejemplos del resto de las instrucciones si no están delimitados visualmente, o si la conversación previa en el mismo chat está influyendo en la respuesta (contaminación de contexto).

**Solución:**
1. Verificar que se inició un **nuevo chat** antes de la Iteración 3 (no continuar en el mismo hilo).
2. Asegurarse de que los delimitadores `--- EJEMPLO 1 ---` y `--- FIN EJEMPLO 1 ---` están presentes y son visibles.
3. Si el problema persiste, agregar al final del prompt la instrucción explícita: `"Es muy importante que repliques exactamente el estilo, la estructura y las frases de transición de los dos ejemplos anteriores."`.
4. Regenerar la respuesta haciendo clic en el botón de regenerar o enviando el prompt nuevamente en un nuevo chat.

---

### Problema 2: Copilot Chat muestra un error o no responde al enviar el prompt few-shot (que es más largo)

**Síntomas:** Al enviar el prompt de la Iteración 3 (que contiene aproximadamente 400–500 palabras incluyendo los ejemplos), Copilot Chat muestra un mensaje de error, se queda cargando indefinidamente, o trunca el prompt.

**Causa:** Problemas de conectividad intermitente, tiempo de espera del servicio excedido, o el prompt supera temporalmente la capacidad de procesamiento del servicio en ese momento.

**Solución:**
1. Verificar la conexión a Internet del equipo del instructor (abrir otra pestaña y navegar a cualquier sitio).
2. Refrescar la página de Copilot Chat con `Ctrl + F5`.
3. Iniciar un nuevo chat e intentar pegar el prompt nuevamente.
4. Si el problema persiste, dividir el prompt en dos mensajes dentro del mismo chat:
   - **Primer mensaje:** Enviar solo los dos ejemplos con la instrucción: `"Te comparto dos ejemplos de correos de seguimiento que uso habitualmente. Analiza su estilo, estructura y tono. En mi siguiente mensaje te pediré que redactes uno nuevo con este mismo estilo."`.
   - **Segundo mensaje:** Enviar el resto del prompt (Rol, Objetivo, Contexto, Formato, Tono, Restricciones) con la instrucción final: `"Usando el estilo de los dos ejemplos anteriores, redacta el correo de seguimiento."`.
5. Si el servicio no responde en absoluto, tener preparadas capturas de pantalla de las respuestas esperadas como respaldo para completar la demostración.

## Limpieza

Al finalizar la demostración, el instructor debe realizar las siguientes acciones:

1. **Cerrar los chats de demostración:** Hacer clic en "Nuevo chat" para limpiar la conversación activa. No es necesario eliminar el historial, pero se recomienda no dejar los prompts de ejemplo visibles si la pantalla permanecerá proyectada durante el Laboratorio 2.
2. **Cerrar el documento de texto auxiliar** (Notepad) que contenía los prompts preparados, para evitar que los participantes copien los prompts en lugar de crear los suyos propios en el Laboratorio 2.
3. **Mantener abierto** Copilot Chat en modo Trabajo, ya que los participantes lo necesitarán inmediatamente para el Laboratorio 2.
4. **Distribuir** (si no se hizo antes) el archivo `LAB02_plantilla_biblioteca_prompts_v1.docx` a todos los participantes.

## Resumen

En esta demostración se ilustró de manera práctica cómo la calidad de un prompt determina directamente la calidad de la respuesta de Copilot Chat. Los tres niveles de prompt demostrados representan una progresión clara:

| Nivel | Técnica | Cuándo usarla |
|---|---|---|
| **1 — Prompt vago** | Sin estructura ni contexto | Solo para exploración inicial o lluvia de ideas rápida. No recomendado para entregables profesionales. |
| **2 — Prompt estructurado** | Marco Objetivo-Contexto-Expectativas-Fuente con restricciones | Para la mayoría de tareas profesionales donde se necesita un resultado específico y controlado. |
| **3 — Prompt few-shot** | Instrucciones estructuradas + 2 o más ejemplos del resultado deseado | Cuando se necesita replicar un estilo, tono o formato muy específico que es difícil de describir solo con palabras. |

### Aprendizajes clave para el Laboratorio 2

- Siempre responder las cinco preguntas clave (qué, para quién, por qué, cómo, restricciones) antes de enviar un prompt.
- Las restricciones negativas ("no incluir X") son tan importantes como las instrucciones positivas.
- Los ejemplos en un prompt few-shot deben variar en contenido pero mantener la misma estructura para que el modelo identifique el patrón.
- Más esfuerzo en el prompt = menos esfuerzo en la edición posterior.

### Recursos adicionales

- [Documentación oficial de Microsoft sobre escritura de prompts efectivos para Copilot](https://learn.microsoft.com/es-es/copilot/microsoft-365/prompting-tips)
- [Principios de prompting del Microsoft Copilot Adoption Hub](https://adoption.microsoft.com/es-es/copilot/)
- [Investigación de Microsoft: el contexto lo es todo en Copilot](https://www.microsoft.com/en-us/worklab/ai-data-drop-when-it-comes-to-copilot-context-is-everything)
