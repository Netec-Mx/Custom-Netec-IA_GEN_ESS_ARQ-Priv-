# Laboratorio 3. Trabajo con información en Copilot Chat: resumir, extraer, transformar y verificar un archivo proporcionado por el instructor

## Metadatos

| Campo | Valor |
|---|---|
| **Duración** | 85 minutos |
| **Complejidad** | Alta |
| **Nivel Bloom** | Aplicar |

## Descripción General

En este laboratorio trabajarás directamente con un documento de negocio ficticio (PDF o Word, entre 8 y 15 páginas) proporcionado por el instructor. Adjuntarás el archivo a Microsoft 365 Copilot Chat y ejecutarás cinco bloques de trabajo secuenciales: exploración inicial, resumen con restricciones, extracción dirigida de datos, transformación a formatos de negocio y verificación de fidelidad con detección de límites. Al finalizar, entregarás un documento de síntesis que integre todas las respuestas generadas, las verificaciones realizadas y una reflexión profesional sobre el uso responsable de Copilot Chat.

## Objetivos de Aprendizaje

Al completar este laboratorio, serás capaz de:

- [ ] Adjuntar correctamente un archivo (PDF, Word o Excel) a Copilot Chat y formular preguntas exploratorias de distinto tipo (general, específica, inferencial) sobre su contenido.
- [ ] Generar resúmenes en al menos tres niveles de profundidad (ejecutivo, puntos clave, versión no técnica) y seleccionar el más adecuado para un destinatario específico.
- [ ] Extraer información dirigida del documento (fechas, cifras, responsables, riesgos, compromisos) utilizando prompts con restricciones de formato, verificando cada dato contra el texto original.
- [ ] Transformar secciones del documento en al menos dos formatos de negocio distintos (tabla comparativa, agenda de reunión, plan de acción o correo ejecutivo) aplicando técnicas de prompting estructurado.
- [ ] Identificar al menos un caso donde Copilot Chat genera información que excede o distorsiona el contenido del documento, documentando el hallazgo y los controles de uso responsable aplicables.

## Prerrequisitos

**Conocimientos previos:**

- Haber completado el Laboratorio 1 (01-00-01) con el mapa de oportunidades y riesgos guardado.
- Haber completado el Laboratorio 2 (02-00-01) con la biblioteca de prompts reutilizables en archivo `.docx`.
- Haber observado las demostraciones 01-00-02 y 02-00-02.
- Comprender los cuatro verbos de acción de redacción en Copilot Chat: crear, reescribir, simplificar y adaptar (Lección 3.1).
- Conocer las técnicas de prompting zero-shot, one-shot y few-shot cubiertas en lecciones anteriores.

**Acceso y materiales:**

- Cuenta corporativa con licencia de Microsoft 365 Copilot Chat activa (verificada al menos 24 horas antes del curso).
- Archivo de práctica proporcionado por el instructor: `LAB03_documento_practica_negocio_v1.pdf` (o `.docx`), entre 8 y 15 páginas, máximo 5 MB.
- Archivo de biblioteca de prompts del Laboratorio 2: `LAB02_plantilla_biblioteca_prompts_v1.docx`.
- Archivo de mapa de oportunidades del Laboratorio 1: `LAB01_plantilla_mapa_oportunidades_v1.docx`.
- Navegador web compatible (Microsoft Edge 124+ o Google Chrome 124+).
- Adobe Acrobat Reader 2024.002.20759 o Microsoft Edge para visualizar el PDF de práctica.
- Microsoft Word 2404 para crear el documento de síntesis de entrega.

## Entorno de Laboratorio

**Hardware mínimo del participante:**

| Componente | Requisito mínimo | Recomendado |
|---|---|---|
| Procesador | 64 bits, 2 núcleos | Intel Core i5 / AMD Ryzen 5 o superior |
| RAM | 8 GB | 16 GB |
| Pantalla | 1280×768 | 1920×1080 |
| Internet | 5 Mbps de bajada por participante | 10 Mbps de bajada |

**Software requerido:**

| Software | Versión | Propósito |
|---|---|---|
| Microsoft Edge | 124.0.2478.97+ | Navegador principal para Copilot Chat |
| Google Chrome | 124.0.6367.119+ | Navegador alternativo |
| Microsoft 365 Copilot Chat (web) | Servicio activo mayo 2025 | Plataforma principal del laboratorio |
| Microsoft Word | 2404 (Build 17531.20152) | Documento de síntesis y archivo de práctica `.docx` |
| Adobe Acrobat Reader | 2024.002.20759 | Visualización del PDF de práctica |

**Configuración inicial (antes de comenzar):**

1. Abre Microsoft Edge o Google Chrome.
2. Navega a **https://m365.cloud.microsoft/chat**.
3. Inicia sesión con tu cuenta corporativa.
4. Verifica que puedes alternar al modo **Trabajo** (Work) haciendo clic en el selector de modo en la parte superior del chat. El modo debe mostrar el ícono de maletín o la etiqueta "Trabajo".
5. Verifica que el botón de adjuntar archivo (ícono de clip 📎) está visible en la barra de entrada del chat.
6. Abre el archivo `LAB03_documento_practica_negocio_v1.pdf` (o `.docx`) en Adobe Acrobat Reader o Word para tenerlo disponible como referencia visual durante todo el laboratorio.
7. Crea un nuevo documento en Microsoft Word titulado `LAB03_sintesis_entrega_[TuNombre].docx`. Este será tu documento de entrega.
8. Ten abierto tu archivo `LAB02_plantilla_biblioteca_prompts_v1.docx` del Laboratorio 2 para reutilizar prompts.

> **⚠️ Importante:** Asegúrate de estar en modo **Trabajo** (Work) en Copilot Chat durante todo el laboratorio. El modo Web no permite adjuntar archivos del tenant corporativo y puede generar respuestas basadas en conocimiento general de Internet en lugar del contenido de tu documento.

## Instrucciones Paso a Paso

---

### Paso 1: Adjuntar el archivo y realizar exploración inicial (15 minutos)

**Objective:** Adjuntar correctamente el archivo de práctica a Copilot Chat y formular tres preguntas exploratorias de distinto tipo para evaluar si las respuestas se basan en el contenido del archivo.

**Instructions:**

1. En Copilot Chat (modo **Trabajo**), inicia una **nueva conversación** haciendo clic en "Nuevo chat" o el ícono correspondiente.

2. Haz clic en el **ícono de clip (📎)** en la barra de entrada del chat.

3. Selecciona **"Cargar desde el equipo"** (o "Upload from this device") y navega hasta el archivo `LAB03_documento_practica_negocio_v1.pdf` (o `.docx`).

4. Espera a que el archivo aparezca como adjunto confirmado en la barra de entrada. Verás el nombre del archivo con un ícono de documento.

5. Escribe y envía la siguiente **pregunta general** (Pregunta 1):

   ```
   He adjuntado un documento de negocio. ¿Puedes describir en 3 a 5 oraciones
   de qué trata este documento, cuál es su propósito principal y a qué
   período o contexto se refiere?
   ```

6. Lee la respuesta de Copilot Chat. En tu documento de síntesis (`LAB03_sintesis_entrega_[TuNombre].docx`), crea una sección titulada **"Bloque 1: Exploración inicial"** y pega la respuesta. Debajo, anota:
   - ¿La descripción coincide con lo que ves al abrir el documento original?
   - ¿Copilot Chat mencionó algún dato que no está en el documento?

7. En la **misma conversación** (no inicies un chat nuevo), formula la siguiente **pregunta específica** (Pregunta 2):

   ```
   Del documento adjunto, ¿cuáles son las tres cifras numéricas más
   relevantes que se mencionan? Para cada cifra, indica: el valor exacto,
   la página o sección donde aparece y a qué se refiere.
   ```

8. Verifica cada cifra mencionada por Copilot Chat abriendo el documento original en Adobe Acrobat Reader o Word. En tu documento de síntesis, registra:
   - Cifra reportada por Copilot → Cifra real en el documento → ¿Coincide? (Sí/No)

9. Formula la siguiente **pregunta inferencial** (Pregunta 3):

   ```
   Basándote exclusivamente en la información del documento adjunto,
   ¿cuál consideras que es el mayor riesgo o desafío que se describe
   o se puede inferir del contenido? Justifica tu respuesta citando
   las secciones o datos específicos del documento que respaldan
   tu análisis.
   ```

10. En tu documento de síntesis, pega la respuesta y evalúa:
    - ¿La inferencia está respaldada por contenido real del documento?
    - ¿Copilot Chat agregó información externa no presente en el archivo?
    - Marca con ✅ lo que está respaldado y con ⚠️ lo que parece inferido sin base textual clara.

**Expected output:**

- Tres respuestas de Copilot Chat registradas en tu documento de síntesis.
- Cada respuesta acompañada de una verificación manual contra el documento original.
- Identificación clara de si cada respuesta se basa en el contenido del archivo o incluye conocimiento externo.

**Verification:**

- [ ] El archivo aparece como adjunto en la conversación de Copilot Chat.
- [ ] Las tres preguntas (general, específica, inferencial) fueron formuladas y respondidas.
- [ ] Al menos las cifras de la Pregunta 2 fueron verificadas contra el documento original.
- [ ] El documento de síntesis tiene la sección "Bloque 1" con respuestas y anotaciones de verificación.

---

### Paso 2: Generar resúmenes con distintas restricciones (15 minutos)

**Objective:** Aplicar prompts de resumen con variaciones de longitud, formato y audiencia, comparar los resultados y seleccionar el más adecuado para un destinatario ejecutivo ficticio.

**Instructions:**

1. En la **misma conversación** con el archivo adjunto, escribe y envía el siguiente prompt para un **resumen ejecutivo** (Resumen A):

   ```
   Genera un resumen ejecutivo del documento adjunto.
   Restricciones:
   - Máximo 150 palabras.
   - Tono formal y profesional.
   - Estructura: contexto (1-2 oraciones), hallazgos principales (2-3 oraciones),
     conclusión o recomendación (1 oración).
   - No incluyas detalles técnicos ni jerga especializada.
   - El destinatario es un comité directivo que necesita tomar decisiones
     basándose en este resumen.
   ```

2. Pega la respuesta en tu documento de síntesis bajo una nueva sección titulada **"Bloque 2: Resúmenes"**, etiquetándola como **"Resumen A — Ejecutivo (150 palabras)"**.

3. Envía el siguiente prompt para un **resumen en puntos clave** (Resumen B):

   ```
   Resume el documento adjunto en exactamente 5 puntos clave (bullets).
   Cada punto debe tener máximo 2 oraciones.
   Prioriza: datos cuantitativos, decisiones tomadas, compromisos pendientes
   y riesgos identificados.
   Formato: lista con viñetas numeradas.
   ```

4. Pega la respuesta en tu documento de síntesis como **"Resumen B — 5 puntos clave"**.

5. Envía el siguiente prompt para una **versión para audiencia no técnica** (Resumen C):

   ```
   Reescribe el contenido principal del documento adjunto como si
   estuvieras explicándolo a un compañero de trabajo que no tiene
   experiencia en el área temática del documento.
   Usa lenguaje cotidiano, evita siglas sin explicar y utiliza
   analogías si es necesario.
   Extensión: entre 100 y 200 palabras.
   Tono: amigable pero profesional.
   ```

6. Pega la respuesta en tu documento de síntesis como **"Resumen C — Versión no técnica"**.

7. **Compara los tres resúmenes** y responde las siguientes preguntas en tu documento de síntesis:
   - ¿Cuál de los tres resúmenes es más preciso respecto al contenido original?
   - ¿Cuál enviarías a un director general que tiene 2 minutos para leer? ¿Por qué?
   - ¿Alguno de los resúmenes omitió información que consideras crítica?
   - ¿Alguno agregó información que no está en el documento original?

8. Selecciona el resumen que consideres más adecuado para un destinatario ejecutivo y márcalo con **"★ Seleccionado"** en tu documento.

**Expected output:**

- Tres resúmenes con diferentes restricciones, claramente etiquetados en el documento de síntesis.
- Un análisis comparativo escrito por el participante (4 preguntas respondidas).
- Un resumen seleccionado como el más adecuado para audiencia ejecutiva.

**Verification:**

- [ ] Se generaron exactamente tres resúmenes con restricciones distintas.
- [ ] Cada resumen respeta las restricciones solicitadas (longitud, formato, tono).
- [ ] El análisis comparativo incluye respuestas a las cuatro preguntas.
- [ ] Un resumen está marcado como seleccionado con justificación.

---

### Paso 3: Extraer información específica con verificación (15 minutos)

**Objective:** Formular prompts de extracción dirigida para obtener datos puntuales del documento y verificar cada dato extraído contra el texto original.

**Instructions:**

1. En la misma conversación, envía el siguiente prompt de **extracción de compromisos y fechas**:

   ```
   Del documento adjunto, extrae todos los compromisos, plazos o fechas
   límite que se mencionan.
   Presenta la información en una tabla con las siguientes columnas:
   | N° | Compromiso o acción | Fecha o plazo | Responsable (si se menciona) | Sección del documento |
   Si algún campo no está disponible en el documento, escribe "No especificado".
   No inventes información que no esté en el texto.
   ```

2. Pega la tabla generada en tu documento de síntesis bajo la sección **"Bloque 3: Extracción dirigida"**, etiquetándola como **"Extracción A — Compromisos y fechas"**.

3. **Verificación obligatoria:** Abre el documento original y localiza cada compromiso y fecha listados por Copilot Chat. En tu documento de síntesis, agrega una columna adicional a la tabla: **"Verificado (Sí/No/Parcial)"** y complétala manualmente.

4. Envía el siguiente prompt de **extracción de cifras y métricas**:

   ```
   Lista todas las cifras numéricas, porcentajes, montos financieros
   y métricas cuantitativas que aparecen en el documento adjunto.
   Formato de salida:
   - Cifra/métrica: [valor exacto]
   - Contexto: [a qué se refiere en una oración]
   - Ubicación: [sección o página aproximada]
   Ordénalas de mayor a menor relevancia para la toma de decisiones.
   ```

5. Pega el resultado como **"Extracción B — Cifras y métricas"** y verifica al menos 5 cifras contra el documento original. Registra tus hallazgos.

6. Envía el siguiente prompt de **extracción de riesgos o problemas**:

   ```
   Identifica todos los riesgos, problemas, desafíos o áreas de
   preocupación que se mencionan explícitamente en el documento adjunto.
   Para cada uno, indica:
   1. Descripción del riesgo o problema (máximo 2 oraciones)
   2. Cita textual o paráfrasis cercana del documento que lo respalda
   3. Sección donde se encuentra
   Si el documento no menciona riesgos explícitos, indícalo claramente.
   ```

7. Pega el resultado como **"Extracción C — Riesgos y problemas"** y verifica que las citas textuales o paráfrasis realmente existen en el documento original.

8. En tu documento de síntesis, escribe un párrafo de **reflexión sobre la extracción**:
   - ¿Cuántos datos extraídos eran 100% precisos?
   - ¿Encontraste algún dato inventado o distorsionado por Copilot Chat?
   - ¿Qué tipo de extracción (compromisos, cifras, riesgos) fue más confiable?

**Expected output:**

- Tres bloques de extracción con datos estructurados en tablas o listas.
- Verificación manual documentada para cada bloque de extracción.
- Párrafo de reflexión sobre la precisión de la extracción.

**Verification:**

- [ ] Se completaron las tres extracciones (compromisos, cifras, riesgos).
- [ ] Al menos 5 datos de cada extracción fueron verificados contra el documento original.
- [ ] Los hallazgos de verificación están documentados (Sí/No/Parcial).
- [ ] El párrafo de reflexión identifica el nivel de confiabilidad observado.

---

### Paso 4: Transformar contenido en formatos de negocio (20 minutos)

**Objective:** Convertir secciones del documento en al menos dos formatos de negocio distintos, utilizando prompts de la biblioteca del Laboratorio 2 y refinando iterativamente.

**Instructions:**

1. Abre tu archivo `LAB02_plantilla_biblioteca_prompts_v1.docx` y selecciona al menos **dos prompts** que sean aplicables para transformar contenido del documento de práctica. Si tu biblioteca no tiene prompts de transformación directamente aplicables, adáptalos según las indicaciones siguientes.

2. **Transformación 1 — Tabla comparativa.** Envía el siguiente prompt en la misma conversación (o adáptalo desde tu biblioteca):

   ```
   A partir del documento adjunto, crea una tabla comparativa que
   organice la información de las secciones principales.
   La tabla debe tener las siguientes columnas:
   | Sección/Tema | Situación actual | Resultado o avance | Próximos pasos | Responsable |
   Completa cada fila con información extraída exclusivamente del documento.
   Si un campo no tiene información disponible, escribe "No disponible en el documento".
   Formato: tabla en Markdown.
   ```

3. Pega el resultado en tu documento de síntesis bajo la sección **"Bloque 4: Transformación"** como **"Transformación 1 — Tabla comparativa"**.

4. **Evalúa y refina.** Si la tabla tiene celdas vacías que deberían tener contenido, o si detectas información incorrecta, envía un prompt de refinamiento. Ejemplo:

   ```
   En la tabla anterior, la fila sobre [tema específico] tiene el campo
   "Próximos pasos" vacío, pero en la sección [X] del documento
   se mencionan acciones futuras. Por favor, revisa esa sección
   y completa el campo correspondiente.
   ```

5. Documenta en tu síntesis: el prompt original, la primera respuesta, el prompt de refinamiento y la respuesta corregida. Etiqueta claramente cada iteración.

6. **Transformación 2 — Correo ejecutivo.** Envía el siguiente prompt (o adáptalo desde tu biblioteca del Laboratorio 2):

   ```
   Basándote en el documento adjunto, redacta un correo electrónico
   dirigido al director general con las siguientes características:
   - Asunto: claro y específico (máximo 10 palabras).
   - Saludo formal.
   - Primer párrafo: contexto en 2 oraciones (qué es el documento y por qué importa).
   - Segundo párrafo: los 3 hallazgos más relevantes, en formato de viñetas.
   - Tercer párrafo: una recomendación concreta basada en el contenido del documento.
   - Cierre formal con llamado a la acción (solicitar una reunión de 30 minutos).
   - Tono: profesional, conciso, orientado a decisiones.
   - Extensión total: máximo 200 palabras.
   No incluyas información que no esté en el documento.
   ```

7. Pega el resultado como **"Transformación 2 — Correo ejecutivo"**.

8. **Evalúa y refina** el correo. Verifica:
   - ¿El asunto es específico y no genérico?
   - ¿Los 3 hallazgos están respaldados por el documento?
   - ¿La recomendación se deriva lógicamente del contenido?
   - ¿El tono es adecuado para un director general?

   Si necesitas ajustes, envía un prompt de refinamiento. Ejemplo:

   ```
   El correo anterior tiene un tono demasiado informal en el segundo párrafo.
   Reescríbelo manteniendo la misma estructura pero con un tono más formal
   y directo. Además, la recomendación del tercer párrafo no se basa
   en datos del documento. Reformúlala usando la información de la
   sección [X] del documento.
   ```

9. Documenta todas las iteraciones en tu síntesis.

10. **(Opcional — Transformación adicional):** Si el tiempo lo permite, elige un tercer formato de tu biblioteca del Laboratorio 2 (agenda de reunión, plan de acción, minuta, etc.) y genera una transformación adicional. Documéntala como **"Transformación 3 — [Formato elegido]"**.

11. En tu documento de síntesis, escribe un párrafo respondiendo:
    - ¿Cuántas iteraciones de refinamiento necesitaste para cada transformación?
    - ¿Qué tipo de instrucción fue más efectiva para obtener el formato deseado?
    - ¿Qué prompts de tu biblioteca del Laboratorio 2 resultaron más útiles y cuáles necesitaron adaptación?

**Expected output:**

- Al menos dos transformaciones completas en formatos de negocio distintos.
- Documentación de al menos una iteración de refinamiento por transformación.
- Párrafo de reflexión sobre el proceso de transformación y refinamiento.

**Verification:**

- [ ] Se generaron al menos dos transformaciones en formatos de negocio distintos.
- [ ] Cada transformación incluye al menos una iteración de refinamiento documentada.
- [ ] El contenido de las transformaciones fue verificado contra el documento original.
- [ ] Se documentó la reflexión sobre el proceso iterativo.

---

### Paso 5: Verificar fidelidad y detectar límites (15 minutos)

**Objective:** Formular deliberadamente una pregunta cuya respuesta no está en el documento para observar cómo Copilot Chat maneja la ausencia de información, y documentar una reflexión sobre controles de uso responsable.

**Instructions:**

1. Revisa el documento original e identifica un tema o pregunta que **no esté cubierto** en ninguna sección. Por ejemplo, si el documento es un informe trimestral de resultados financieros, podrías preguntar sobre la estrategia de recursos humanos o el plan de sostenibilidad ambiental, temas que probablemente no están en el documento.

2. Formula y envía una **pregunta deliberadamente fuera de alcance**:

   ```
   Basándote exclusivamente en el documento adjunto, ¿cuál es
   [tu pregunta sobre un tema no cubierto en el documento]?
   Proporciona datos específicos del documento que respalden tu respuesta.
   Si la información no está disponible en el documento, indícalo
   explícitamente.
   ```

3. Analiza la respuesta de Copilot Chat y clasifícala en tu documento de síntesis bajo la sección **"Bloque 5: Verificación y límites"**:

   | Comportamiento observado | Marca con ✓ |
   |---|---|
   | Copilot Chat indicó que la información no está en el documento | |
   | Copilot Chat generó una respuesta usando conocimiento externo sin advertirlo | |
   | Copilot Chat generó una respuesta parcialmente basada en el documento y parcialmente inventada | |
   | Copilot Chat se negó a responder | |

4. Si Copilot Chat generó información no presente en el documento, documenta exactamente qué dijo y por qué es problemático. Escribe 2-3 oraciones explicando el riesgo de usar esa respuesta sin verificación.

5. **Prueba de verificación cruzada.** Selecciona una de las respuestas más detalladas que Copilot Chat generó en los pasos anteriores (preferiblemente del Bloque 3 — Extracción). Envía el siguiente prompt:

   ```
   En tu respuesta anterior sobre [tema específico], mencionaste que
   [dato o afirmación específica]. ¿Puedes indicar la cita textual
   exacta del documento donde aparece esta información?
   Copia el texto tal como aparece en el documento original.
   ```

6. Verifica si la cita proporcionada por Copilot Chat es real. Búscala en el documento original usando Ctrl+F. Documenta el resultado:
   - ¿La cita es textualmente correcta?
   - ¿Es una paráfrasis aceptable?
   - ¿Es una fabricación?

7. Abre tu archivo `LAB01_plantilla_mapa_oportunidades_v1.docx` del Laboratorio 1. Revisa los **controles de uso responsable** que definiste. En tu documento de síntesis, responde:
   - ¿Los controles que definiste en el Laboratorio 1 habrían sido suficientes para detectar los problemas encontrados en este laboratorio?
   - ¿Necesitas agregar algún control nuevo? Si es así, ¿cuál?
   - ¿Qué tareas de las realizadas en este laboratorio **no deberían delegarse** a Copilot Chat sin supervisión humana?

8. **Reflexión final.** Escribe un párrafo de cierre (mínimo 5 oraciones) en tu documento de síntesis que responda:
   - ¿Qué funcionó bien al trabajar con Copilot Chat y el documento adjunto?
   - ¿Qué requirió corrección o refinamiento iterativo?
   - ¿Qué no debe delegarse a Copilot Chat según tu experiencia en este laboratorio?
   - ¿Cómo aplicarás lo aprendido en tu trabajo real?

9. Guarda tu documento de síntesis completo: `LAB03_sintesis_entrega_[TuNombre].docx`.

**Expected output:**

- Documentación del comportamiento de Copilot Chat ante una pregunta fuera de alcance.
- Resultado de la prueba de verificación cruzada con cita textual.
- Revisión de controles del Laboratorio 1 con propuestas de mejora.
- Reflexión final de cierre.

**Verification:**

- [ ] Se formuló al menos una pregunta deliberadamente fuera del alcance del documento.
- [ ] El comportamiento de Copilot Chat fue clasificado en la tabla proporcionada.
- [ ] Se realizó al menos una verificación cruzada de cita textual.
- [ ] La reflexión final incluye al menos una tarea que no debe delegarse sin supervisión.
- [ ] El documento de síntesis está completo y guardado.

---

### Paso 6: Compilar y entregar el documento de síntesis (5 minutos)

**Objective:** Organizar el documento de entrega final con todas las secciones requeridas y verificar su completitud.

**Instructions:**

1. Abre tu documento `LAB03_sintesis_entrega_[TuNombre].docx` y verifica que contiene las siguientes secciones en orden:

   ```
   DOCUMENTO DE SÍNTESIS — LABORATORIO 3
   Nombre: [Tu nombre]
   Fecha: [Fecha del laboratorio]

   BLOQUE 1: Exploración inicial
   - Pregunta 1 (general): respuesta + verificación
   - Pregunta 2 (específica): respuesta + tabla de verificación de cifras
   - Pregunta 3 (inferencial): respuesta + evaluación de respaldo textual

   BLOQUE 2: Resúmenes
   - Resumen A — Ejecutivo (150 palabras)
   - Resumen B — 5 puntos clave
   - Resumen C — Versión no técnica
   - Análisis comparativo (4 preguntas)
   - Resumen seleccionado (★)

   BLOQUE 3: Extracción dirigida
   - Extracción A — Compromisos y fechas (con columna de verificación)
   - Extracción B — Cifras y métricas (con verificación)
   - Extracción C — Riesgos y problemas (con verificación de citas)
   - Reflexión sobre precisión de la extracción

   BLOQUE 4: Transformación
   - Transformación 1 — Tabla comparativa (con iteraciones)
   - Transformación 2 — Correo ejecutivo (con iteraciones)
   - (Opcional) Transformación 3
   - Reflexión sobre proceso iterativo

   BLOQUE 5: Verificación y límites
   - Pregunta fuera de alcance + clasificación del comportamiento
   - Prueba de verificación cruzada con cita textual
   - Revisión de controles del Laboratorio 1
   - Reflexión final de cierre
   ```

2. Verifica que cada sección tiene contenido sustantivo (no solo encabezados vacíos).

3. Guarda el archivo final y entrégalo según las instrucciones del instructor (carga en plataforma, correo electrónico o carpeta compartida).

**Expected output:**

- Documento de síntesis completo con las 5 secciones y todas las subsecciones requeridas.

**Verification:**

- [ ] El documento tiene las 5 secciones principales completas.
- [ ] Cada bloque incluye tanto las respuestas de Copilot Chat como las verificaciones del participante.
- [ ] La reflexión final está presente y tiene al menos 5 oraciones.
- [ ] El archivo está guardado con el nombre correcto y entregado.

## Validación y Pruebas

Utiliza la siguiente lista de verificación integral para confirmar que has completado exitosamente todos los componentes del laboratorio:

**Bloque 1 — Exploración:**

| Criterio | Cumple (✓/✗) |
|---|---|
| El archivo fue adjuntado correctamente en modo Trabajo | |
| Se formularon 3 preguntas de tipo distinto (general, específica, inferencial) | |
| Las cifras de la Pregunta 2 fueron verificadas contra el documento original | |
| Se identificó si Copilot Chat usó conocimiento externo en alguna respuesta | |

**Bloque 2 — Resúmenes:**

| Criterio | Cumple (✓/✗) |
|---|---|
| Se generaron 3 resúmenes con restricciones distintas | |
| El Resumen A no excede 150 palabras | |
| El Resumen B tiene exactamente 5 puntos | |
| Se completó el análisis comparativo con las 4 preguntas | |
| Se seleccionó un resumen con justificación | |

**Bloque 3 — Extracción:**

| Criterio | Cumple (✓/✗) |
|---|---|
| Se completaron 3 extracciones temáticas distintas | |
| Al menos 5 datos por extracción fueron verificados manualmente | |
| Se documentaron los resultados de verificación (Sí/No/Parcial) | |
| Se escribió el párrafo de reflexión sobre precisión | |

**Bloque 4 — Transformación:**

| Criterio | Cumple (✓/✗) |
|---|---|
| Se generaron al menos 2 transformaciones en formatos de negocio distintos | |
| Cada transformación tiene al menos 1 iteración de refinamiento documentada | |
| Se consultó la biblioteca de prompts del Laboratorio 2 | |
| Se escribió la reflexión sobre el proceso iterativo | |

**Bloque 5 — Verificación y límites:**

| Criterio | Cumple (✓/✗) |
|---|---|
| Se formuló una pregunta deliberadamente fuera de alcance | |
| El comportamiento de Copilot Chat fue clasificado en la tabla | |
| Se realizó una verificación cruzada de cita textual | |
| Se revisaron los controles del Laboratorio 1 | |
| La reflexión final tiene al menos 5 oraciones sustantivas | |

**Entrega:**

| Criterio | Cumple (✓/✗) |
|---|---|
| El documento de síntesis tiene las 5 secciones completas | |
| El archivo está nombrado correctamente: `LAB03_sintesis_entrega_[TuNombre].docx` | |
| El archivo fue entregado según las instrucciones del instructor | |

## Solución de Problemas

### Problema 1: El botón de adjuntar archivo no aparece o el archivo no se carga

**Síntomas:** Al abrir Copilot Chat, no se ve el ícono de clip (📎) en la barra de entrada, o al hacer clic en él y seleccionar el archivo, este no se adjunta (no aparece el nombre del archivo en la barra, se muestra un error de carga, o el proceso se queda en "cargando" indefinidamente).

**Causa:** Este problema ocurre típicamente por una de tres razones: (1) el chat está en modo **Web** en lugar de modo **Trabajo**, y el modo Web no soporta adjuntar archivos locales de la misma manera; (2) el archivo excede el tamaño máximo permitido (512 MB, aunque para este laboratorio debe ser menor a 5 MB); o (3) la licencia de Microsoft 365 Copilot Chat del participante no incluye la funcionalidad de adjuntar archivos, lo cual puede ocurrir si la licencia fue asignada recientemente y aún no se ha propagado.

**Solución:**

1. **Verifica el modo de trabajo:** Haz clic en el selector de modo en la parte superior del chat y asegúrate de que dice **"Trabajo"** (Work) con el ícono de maletín. Si está en modo "Web", cámbialo.
2. **Verifica el tamaño del archivo:** Haz clic derecho sobre el archivo en el explorador de archivos, selecciona "Propiedades" y confirma que el tamaño es menor a 5 MB.
3. **Recarga la página:** Presiona `Ctrl+Shift+R` (o `Cmd+Shift+R` en macOS) para forzar una recarga completa de la página de Copilot Chat.
4. **Prueba con otro navegador:** Si usas Chrome, intenta con Edge, o viceversa.
5. **Contacta al instructor:** Si el problema persiste, es probable que la licencia no esté correctamente configurada. El instructor debe verificar con el administrador de TI que la cuenta tiene la licencia de Microsoft 365 Copilot Chat activa y propagada.

---

### Problema 2: Copilot Chat responde con información genérica sin hacer referencia al documento adjunto

**Síntomas:** Después de adjuntar el archivo y formular una pregunta, Copilot Chat responde con información general sobre el tema (por ejemplo, describe qué es un informe trimestral en términos genéricos) en lugar de analizar el contenido específico del documento adjuntado. Las respuestas no mencionan datos, nombres, cifras ni secciones presentes en el archivo.

**Causa:** Esto suele ocurrir cuando: (1) el archivo no se adjuntó correctamente (el nombre del archivo no aparece en la barra de entrada al momento de enviar el prompt); (2) la conversación perdió el contexto del archivo adjunto, lo cual puede suceder si se inició un nuevo chat accidentalmente; o (3) el formato del archivo no es compatible o está corrupto (por ejemplo, un PDF escaneado como imagen sin OCR, que Copilot Chat no puede leer como texto).

**Solución:**

1. **Verifica que el archivo está adjunto en la conversación actual:** Antes de enviar cada prompt, confirma que el nombre del archivo aparece visible en la barra de entrada o que fue adjuntado en un mensaje anterior de la misma conversación.
2. **Re-adjunta el archivo:** Si no estás seguro, haz clic en el ícono de clip (📎) y adjunta el archivo nuevamente en tu siguiente mensaje.
3. **Haz referencia explícita al archivo en el prompt:** Incluye frases como "Del documento adjunto..." o "Basándote exclusivamente en el archivo que acabo de adjuntar..." para orientar a Copilot Chat.
4. **Verifica que el archivo es legible como texto:** Abre el PDF en Adobe Acrobat Reader e intenta seleccionar y copiar texto. Si no puedes seleccionar texto (es una imagen escaneada), el archivo necesita procesamiento OCR previo. Notifica al instructor para que proporcione una versión con texto seleccionable.
5. **Inicia una nueva conversación:** Si la conversación acumuló muchos mensajes, el contexto puede degradarse. Inicia un nuevo chat, adjunta el archivo de nuevo y reformula tu pregunta.

## Limpieza

1. **Conversaciones en Copilot Chat:** No es necesario eliminar las conversaciones; permanecerán en tu historial de chat y pueden servir como referencia futura. Si deseas eliminarlas por razones de orden, haz clic en los tres puntos (⋯) junto a cada conversación en el panel lateral y selecciona "Eliminar".

2. **Archivos locales:** Mantén los siguientes archivos en una carpeta organizada para referencia futura:
   - `LAB03_sintesis_entrega_[TuNombre].docx` (tu entregable).
   - `LAB03_documento_practica_negocio_v1.pdf` (o `.docx`) (el archivo de práctica).
   - `LAB02_plantilla_biblioteca_prompts_v1.docx` (tu biblioteca de prompts).
   - `LAB01_plantilla_mapa_oportunidades_v1.docx` (tu mapa de oportunidades).

3. **Sesión del navegador:** No es necesario cerrar sesión de Microsoft 365 si continuarás con actividades del curso. Si es el final de la jornada, cierra sesión de tu cuenta corporativa en el navegador.

4. **No se crearon recursos en la nube** que requieran eliminación o desaprovisionamiento.

## Resumen

En este laboratorio aplicaste de manera integrada todas las habilidades desarrolladas en los laboratorios anteriores sobre un documento de negocio real. Los aprendizajes clave incluyen:

- **Adjuntar y explorar:** Aprendiste que la calidad de las respuestas de Copilot Chat depende de que el archivo esté correctamente adjuntado, de que el modo Trabajo esté activo y de que las preguntas sean específicas y variadas.
- **Resumir con restricciones:** Comprobaste que el mismo documento puede resumirse de formas radicalmente diferentes según las restricciones de longitud, formato y audiencia, y que la selección del resumen adecuado es una decisión humana.
- **Extraer con verificación:** Experimentaste que la extracción dirigida es una de las capacidades más útiles de Copilot Chat, pero que cada dato extraído debe verificarse contra el documento original antes de usarse en decisiones.
- **Transformar iterativamente:** Practicaste la transformación de contenido en formatos de negocio y confirmaste que el refinamiento iterativo (ajustar el prompt basándose en la respuesta anterior) es una técnica esencial para obtener resultados de calidad.
- **Verificar y detectar límites:** Identificaste que Copilot Chat puede generar información plausible pero no presente en el documento, lo cual refuerza la necesidad de los controles de uso responsable definidos en el Laboratorio 1.

**Recursos adicionales:**

- [Microsoft Learn — Adjuntar archivos en Microsoft 365 Copilot Chat](https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-overview)
- [Microsoft Adoption — Prompting con Microsoft 365 Copilot: guía práctica](https://adoption.microsoft.com/es-es/copilot/)
- [Plain Language Guidelines — Referencia internacional para simplificación de textos](https://www.plainlanguage.gov/guidelines/)
- Tu archivo `LAB02_plantilla_biblioteca_prompts_v1.docx` — continúa enriqueciéndolo con los prompts que mejor funcionaron en este laboratorio.
- Tu archivo `LAB01_plantilla_mapa_oportunidades_v1.docx` — actualízalo con los nuevos controles identificados en el Bloque 5.

---

# Demo: Demostración guiada: agregar un archivo, resumirlo, extraer información, transformar la salida y verificarla contra la fuente

## Metadatos

| Campo | Detalle |
|---|---|
| **Duración** | 20 minutos |
| **Complejidad** | Media |
| **Nivel Bloom** | Aplicar (Apply) |
| **Tipo de actividad** | Demostración en vivo del instructor |
| **Plataforma** | Microsoft 365 Copilot Chat (https://m365.cloud.microsoft/chat) |

## Descripción General

En esta demostración, el instructor ejecuta en vivo el flujo completo de trabajo con archivos adjuntos en Microsoft 365 Copilot Chat: carga de un documento PDF y un documento Word, formulación de prompts de resumen ejecutivo, extracción de datos clave, transformación de formato y verificación de las respuestas contra el contenido original del archivo. Los estudiantes observan cómo el instructor construye y refina cada prompt paso a paso, verbalizando su razonamiento, y registran los patrones de prompting demostrados como base para el laboratorio práctico posterior (Lab 04-00-01).

> ℹ️ **Nota:** Esta práctica es una **Demostración realizada por el instructor**. El instructor ejecutará los pasos y comandos mientras los alumnos observan, toman notas y analizan el procedimiento, en lugar de realizarla individualmente.

## Objetivos de Aprendizaje

Al finalizar esta demostración, los estudiantes serán capaces de:

- [ ] Describir el proceso completo de carga de un archivo (PDF y Word) en Microsoft 365 Copilot Chat y la formulación de prompts sobre su contenido.
- [ ] Identificar los patrones de prompting para resumen ejecutivo, extracción dirigida, transformación de formato y verificación de fuente demostrados por el instructor.
- [ ] Explicar cómo ajustar tono, audiencia y extensión en un prompt de refinamiento iterativo sobre un documento adjunto.
- [ ] Reconocer cuándo una respuesta de Copilot Chat excede la información disponible en el archivo fuente (exceso de alcance).
- [ ] Registrar en sus notas los cuatro bloques fundamentales de prompting (resumen, extracción, transformación, verificación) que aplicarán en el Lab 04-00-01.

## Prerrequisitos

### Conocimiento previo

| Requisito | Descripción |
|---|---|
| Interfaz de Copilot Chat | Los estudiantes deben haber completado los labs del Batch 1 (módulos 1 y 2) o tener conocimiento equivalente de la interfaz básica de Copilot Chat, incluyendo cómo iniciar una conversación y cambiar entre modo Web y modo Trabajo. |
| Conceptos de prompting | Familiaridad con la estructura básica de un prompt (rol, tarea, contexto, formato de salida) cubierta en lecciones anteriores. |
| Lección 3.1 completada | Los estudiantes deben haber revisado los conceptos de crear, reescribir, simplificar y adaptar tono y audiencia presentados en la Lección 3.1. |

### Acceso y preparación del instructor

| Requisito | Verificación |
|---|---|
| Cuenta corporativa con licencia Microsoft 365 Copilot Chat activa | El instructor debe confirmar acceso a https://m365.cloud.microsoft/chat y verificar que el modo **Trabajo** está disponible al menos 1 hora antes de la sesión. |
| Archivos de práctica preparados | **Archivo PDF**: Informe ejecutivo ficticio (máx. 10 páginas, entre 8-15 páginas de contenido de negocio, con al menos 5 datos verificables). **Archivo Word**: Propuesta de proyecto ficticia (máx. 8 páginas). Ambos archivos deben seguir la nomenclatura `LAB03_documento_practica_negocio_v1.pdf` y `LAB03_documento_practica_propuesta_v1.docx`. |
| Archivos descargados localmente | Los archivos deben estar guardados en una carpeta accesible del equipo del instructor (por ejemplo, `C:\CursoMCopilot\Lab03\` o `~/CursoMCopilot/Lab03/`). |
| Proyección de pantalla | Proyector físico o pantalla compartida en videoconferencia configurada y probada con resolución mínima de 1920×1080. |
| Navegador preparado | Microsoft Edge 124+ abierto con una pestaña limpia en https://m365.cloud.microsoft/chat, sesión iniciada con la cuenta corporativa del instructor. |

### Preparación de los estudiantes

| Elemento | Instrucción |
|---|---|
| Material de notas | Cada estudiante debe tener a mano papel, cuaderno o un documento de texto abierto (Notepad, TextEdit o similar) para registrar los patrones de prompting. |
| Atención activa | Los estudiantes **NO** ejecutan acciones en sus equipos durante esta demo. Deben cerrar aplicaciones no relacionadas para mantener la atención en la proyección. |

## Entorno de Laboratorio

### Hardware del instructor

| Componente | Especificación mínima |
|---|---|
| Procesador | Intel Core i5 / AMD Ryzen 5 o superior (64 bits) |
| RAM | 8 GB mínimo (16 GB recomendado) |
| Pantalla | 1920×1080 para proyección clara |
| Conexión a Internet | 10 Mbps de bajada (estable) |
| Proyector / Pantalla compartida | Resolución mínima 1920×1080 |

### Software del instructor

| Software | Versión / Detalle |
|---|---|
| Microsoft Edge | 124.0.2478.97 o superior |
| Microsoft 365 Copilot Chat (web) | https://m365.cloud.microsoft/chat — modo **Trabajo** activado |
| Archivos de práctica | `LAB03_documento_practica_negocio_v1.pdf` (≤ 5 MB) y `LAB03_documento_practica_propuesta_v1.docx` (≤ 5 MB) |
| Adobe Acrobat Reader (opcional) | 2024.002.20759 — para mostrar el contenido original del PDF si se necesita verificación visual |

### Configuración previa a la demostración

Antes de iniciar la demostración frente a los estudiantes, el instructor debe completar esta lista de verificación:

1. Abrir Microsoft Edge e iniciar sesión en https://m365.cloud.microsoft/chat con la cuenta corporativa.
2. Verificar que el selector de modo muestra **Trabajo** (Work) como opción disponible y seleccionarlo.
3. Confirmar que el botón de adjuntar archivos (ícono de clip 📎) está visible en la barra de entrada del chat.
4. Tener los dos archivos de práctica abiertos en el explorador de archivos para acceso rápido.
5. Abrir el archivo PDF en Adobe Acrobat Reader en una ventana separada (para la verificación visual del Paso 7).
6. Preparar un documento de texto con los prompts pre-escritos (como respaldo en caso de errores de tipeo en vivo).
7. Verificar que la proyección es legible desde la posición más alejada del aula o que la pantalla compartida se ve correctamente.

## Instrucciones Paso a Paso

> **Nota para el instructor:** En cada paso, verbalice en voz alta su razonamiento al construir el prompt. Explique **por qué** elige cada elemento (rol, tarea, contexto, formato, restricciones). Haga pausas para preguntar a los estudiantes qué esperan que ocurra antes de enviar cada prompt.

### Paso 1: Abrir Copilot Chat y verificar el modo Trabajo

**Objetivo:** Confirmar que el entorno está listo y que los estudiantes comprenden la diferencia entre el modo Web y el modo Trabajo para el trabajo con archivos adjuntos.

**Instrucciones:**

1. En Microsoft Edge, navegue a **https://m365.cloud.microsoft/chat**.
2. Señale a los estudiantes el selector de modo en la interfaz. Explique brevemente:
   - **Modo Web**: Copilot busca información en Internet. No accede a archivos corporativos ni permite adjuntar documentos del tenant.
   - **Modo Trabajo**: Copilot accede a datos del tenant corporativo y permite adjuntar archivos locales para análisis.
3. Seleccione el modo **Trabajo** haciendo clic en el selector correspondiente.
4. Señale el ícono de clip (📎) en la barra de entrada del chat y explique: *"Este botón es el que usaremos para cargar archivos. En modo Trabajo, Copilot puede procesar el contenido del archivo y responder preguntas sobre él."*
5. Inicie una nueva conversación haciendo clic en **Nuevo chat** (si hay conversaciones previas abiertas).

**Resultado esperado:** La interfaz de Copilot Chat muestra el modo **Trabajo** activo, el ícono de adjuntar archivos está visible y se ha iniciado una conversación limpia.

**Verificación:** El indicador de modo muestra "Trabajo" y la barra de entrada incluye el botón de adjuntar (📎). No hay mensajes previos en la conversación.

---

### Paso 2: Cargar el archivo PDF de práctica

**Objetivo:** Demostrar el proceso de carga de un archivo PDF en Copilot Chat y confirmar que el sistema lo reconoce correctamente.

**Instrucciones:**

1. Haga clic en el ícono de clip (📎) en la barra de entrada del chat.
2. En el diálogo de selección de archivos, navegue a la carpeta donde guardó los archivos de práctica.
3. Seleccione el archivo `LAB03_documento_practica_negocio_v1.pdf` y haga clic en **Abrir**.
4. Espere a que Copilot Chat muestre la confirmación de que el archivo ha sido adjuntado. Señale a los estudiantes el indicador visual (nombre del archivo visible en la barra de entrada o como chip adjunto).
5. Explique a los estudiantes: *"Copilot ahora tiene acceso al contenido de este PDF. Cada prompt que escribamos en esta conversación puede hacer referencia a este documento. Es importante notar que el archivo no se 'sube' permanentemente: solo está disponible dentro de esta conversación."*
6. Antes de enviar cualquier prompt, pregunte a los estudiantes: *"Si yo escribo simplemente 'Resume este documento', ¿qué creen que obtendremos? ¿Será útil o genérico?"*

**Resultado esperado:** El archivo PDF aparece adjunto en la conversación. Copilot Chat muestra el nombre del archivo como referencia visual.

**Verificación:** El nombre del archivo `LAB03_documento_practica_negocio_v1.pdf` es visible como archivo adjunto en la interfaz del chat antes de enviar el primer prompt.

---

### Paso 3: Formular un prompt de resumen ejecutivo ajustado a audiencia directiva

**Objetivo:** Demostrar cómo construir un prompt de resumen con especificaciones de audiencia, tono y extensión, y mostrar la diferencia entre un prompt vago y uno estructurado.

**Instrucciones:**

1. **Primero, demuestre un prompt vago** (como contraste pedagógico). Escriba en la barra de entrada:

```
Resume este documento.
```

2. Envíe el prompt y espere la respuesta. Señale a los estudiantes las características de la respuesta:
   - ¿Es demasiado larga o corta?
   - ¿El tono es apropiado para una audiencia directiva?
   - ¿Incluye detalles técnicos innecesarios para un comité directivo?

3. Explique: *"Este resultado es un punto de partida, pero no es lo que necesitaríamos para presentar a un comité directivo. Vamos a construir un prompt mucho más específico."*

4. **Ahora, formule el prompt estructurado.** Escriba:

```
Eres un analista de negocio senior.
Resume el documento adjunto como un resumen ejecutivo
dirigido al comité directivo de la empresa.
El tono debe ser formal y profesional.
Extensión máxima: 200 palabras.
Enfócate en: hallazgos principales, impacto de negocio
y recomendaciones clave.
No incluyas detalles técnicos ni metodología.
```

5. Envíe el prompt y espere la respuesta.
6. Lea la respuesta en voz alta y señale:
   - Cómo el rol asignado ("analista de negocio senior") influye en el enfoque.
   - Cómo la restricción de extensión (200 palabras) fuerza la síntesis.
   - Cómo la exclusión explícita ("No incluyas detalles técnicos") filtra contenido.
7. Pregunte a los estudiantes: *"¿Notan la diferencia entre la primera respuesta y esta? ¿Qué elementos del prompt produjeron esa diferencia?"*

**Resultado esperado:** Copilot Chat genera un resumen ejecutivo conciso (aproximadamente 200 palabras), con tono formal, enfocado en hallazgos, impacto y recomendaciones, sin detalles técnicos.

**Verificación:** Comparar visualmente ambas respuestas (prompt vago vs. prompt estructurado). La segunda respuesta debe ser notablemente más enfocada, más corta y con tono más ejecutivo.

---

### Paso 4: Refinar el prompt para cambiar tono y extensión

**Objetivo:** Demostrar el refinamiento iterativo de un prompt, mostrando cómo ajustar tono (de formal a conversacional) y extensión sin repetir toda la instrucción.

**Instrucciones:**

1. Explique a los estudiantes: *"Ahora vamos a refinar la respuesta anterior sin empezar de cero. Copilot Chat mantiene el contexto de la conversación, así que podemos hacer ajustes incrementales."*

2. Escriba el siguiente prompt de refinamiento:

```
Ahora reescribe ese mismo resumen, pero con un tono
conversacional y accesible, como si estuvieras explicando
los puntos clave a un colega en una reunión informal.
Extensión: máximo 150 palabras.
Usa oraciones cortas y evita jerga corporativa.
```

3. Envíe el prompt y espere la respuesta.
4. Compare en voz alta las diferencias entre el resumen formal (Paso 3) y el conversacional:
   - Cambios en vocabulario (formal → coloquial).
   - Cambios en estructura de oraciones (complejas → cortas).
   - Cambios en el nivel de detalle.
5. Señale: *"Observen que no tuve que volver a adjuntar el archivo ni repetir el contexto completo. Copilot Chat recuerda el documento y la conversación previa. Este es el poder del refinamiento iterativo."*
6. Pregunte a los estudiantes: *"¿Para qué situación real usarían la versión formal y para cuál la conversacional?"*

**Resultado esperado:** Copilot Chat genera una versión del resumen con tono conversacional, oraciones más cortas, vocabulario accesible y extensión reducida (~150 palabras).

**Verificación:** La respuesta debe mantener los mismos puntos clave del resumen ejecutivo del Paso 3, pero con un tono claramente diferente. Verificar que la información de fondo no cambió, solo la forma de expresarla.

---

### Paso 5: Extraer información específica en formato de lista numerada

**Objetivo:** Demostrar el patrón de prompting de extracción dirigida, solicitando datos concretos del documento en un formato estructurado.

**Instrucciones:**

1. Explique: *"Ahora pasamos de resumir a extraer. Extraer significa pedirle a Copilot que localice datos específicos dentro del documento: fechas, cifras, nombres, compromisos. Este es uno de los patrones más útiles en el trabajo diario."*

2. Escriba el siguiente prompt:

```
Del documento adjunto, extrae los siguientes datos
en una lista numerada:
1. Todas las fechas mencionadas y su contexto
2. Cifras financieras o métricas de rendimiento
3. Nombres de personas o equipos responsables
4. Compromisos o acciones pendientes con fecha límite
5. Riesgos o alertas identificados

Si alguno de estos datos no aparece en el documento,
indica explícitamente "No encontrado en el documento".
```

3. Envíe el prompt y espere la respuesta.
4. Señale a los estudiantes los elementos clave de este prompt:
   - **Lista de categorías específicas**: Le dice a Copilot exactamente qué buscar.
   - **Formato de salida explícito**: Lista numerada.
   - **Cláusula de seguridad**: *"Si no aparece, indica 'No encontrado'"* — esto previene que Copilot invente datos.
5. Revise la respuesta punto por punto. Para cada dato extraído, pregunte: *"¿Este dato les parece que viene del documento o podría ser una invención?"*
6. Si algún dato dice "No encontrado en el documento", señale: *"Esto es exactamente lo que queremos. Copilot nos está diciendo que no tiene esa información, en lugar de inventarla. La cláusula de seguridad funcionó."*

**Resultado esperado:** Una lista numerada con cinco categorías, cada una conteniendo los datos extraídos del documento o la indicación explícita de "No encontrado en el documento" donde corresponda.

**Verificación:** Abra el archivo PDF en Adobe Acrobat Reader (ventana separada) y verifique manualmente al menos 2-3 de los datos extraídos. Señale a los estudiantes cómo se realiza esta verificación cruzada.

---

### Paso 6: Transformar la lista en tabla comparativa

**Objetivo:** Demostrar el patrón de transformación de formato, convirtiendo información ya extraída en una estructura visual diferente (tabla).

**Instrucciones:**

1. Explique: *"Tenemos una lista de datos extraídos. Pero si necesitamos presentar esta información a alguien, una tabla puede ser más efectiva. Vamos a pedirle a Copilot que transforme el formato sin cambiar el contenido."*

2. Escriba el siguiente prompt:

```
Transforma la información que acabas de extraer
en una tabla con las siguientes columnas:
| Categoría | Dato específico | Página o sección del documento | Nivel de prioridad (Alta/Media/Baja) |

Ordena la tabla por nivel de prioridad de mayor a menor.
Si no puedes determinar la página exacta, indica
"Sección no identificada".
Para el nivel de prioridad, usa tu criterio basado
en el contexto del documento.
```

3. Envíe el prompt y espere la respuesta.
4. Señale a los estudiantes la tabla generada:
   - ¿Las columnas corresponden a lo solicitado?
   - ¿Los datos son consistentes con la lista del Paso 5?
   - ¿La columna de "Nivel de prioridad" tiene sentido según el contexto del documento?
5. Explique: *"Observen que le pedí a Copilot que asignara un nivel de prioridad 'usando su criterio'. Esto es una decisión de diseño del prompt: a veces queremos que la IA haga una inferencia. Pero ¡cuidado! Esa prioridad es una sugerencia de la IA, no un hecho del documento. El juicio final siempre es nuestro."*
6. Señale la diferencia entre datos verificables (fechas, cifras) y datos inferidos (nivel de prioridad) en la tabla.

**Resultado esperado:** Una tabla Markdown con cuatro columnas, conteniendo los datos extraídos en el Paso 5, organizada por prioridad, con indicaciones claras donde la información de sección no fue identificable.

**Verificación:** Confirmar que todos los datos de la lista del Paso 5 aparecen en la tabla (no se perdió información en la transformación). Verificar que la columna de prioridad contiene valores válidos (Alta, Media, Baja).

---

### Paso 7: Verificar las respuestas contra el contenido original del archivo

**Objetivo:** Demostrar el patrón de verificación de fuente, pidiendo a Copilot que cite las secciones del documento que respaldan cada afirmación, e identificar posibles excesos de alcance.

**Instrucciones:**

1. Explique: *"Este es el paso más importante de toda la demostración. Hasta ahora, Copilot nos ha dado resúmenes, listas y tablas. Pero ¿cómo sabemos que todo eso realmente está en el documento? Vamos a pedirle que nos muestre sus fuentes."*

2. Escriba el siguiente prompt:

```
Para cada uno de los 3 datos más importantes que extrajiste
del documento, haz lo siguiente:
1. Cita el párrafo o fragmento exacto del documento
   que respalda ese dato.
2. Indica en qué sección del documento se encuentra.
3. Evalúa tu nivel de confianza: ¿el dato está
   explícitamente en el documento, o lo inferiste
   a partir del contexto?

Si alguno de los datos que mencionaste anteriormente
NO tiene respaldo directo en el documento, indícalo
honestamente.
```

3. Envíe el prompt y espere la respuesta.
4. **Verificación cruzada en vivo:** Abra la ventana de Adobe Acrobat Reader con el PDF y busque los fragmentos citados por Copilot.
   - Para cada cita, localice el texto en el documento original.
   - Señale a los estudiantes: *"Vean, este fragmento sí aparece en la página X del documento. La cita es precisa."*
   - Si alguna cita no coincide exactamente o está parafraseada, señale: *"Aquí Copilot parafraseó en lugar de citar textualmente. Esto es común. No es necesariamente un error, pero debemos verificar que el sentido se preservó."*
5. **Identificación de excesos de alcance:** Revise si alguna respuesta anterior contenía información que NO está en el documento. Explique: *"Un 'exceso de alcance' ocurre cuando Copilot agrega información de su conocimiento general que no proviene del archivo adjunto. Por ejemplo, si el documento habla de un proyecto y Copilot agrega estadísticas de la industria que no están en el archivo, eso es un exceso."*
6. Si detecta un exceso, señálelo explícitamente: *"Este dato NO aparece en nuestro documento. Copilot lo infirió o lo tomó de su conocimiento general. En un contexto profesional, esto podría ser peligroso si lo presentamos como información del informe."*
7. Si no detecta excesos evidentes, formule una pregunta deliberada para provocar uno:

```
Según el documento adjunto, ¿cuál es la proyección
de ingresos para el próximo año fiscal?
```

8. Si el documento no contiene esa información, Copilot debería indicarlo. Si en cambio genera una respuesta con datos no presentes en el archivo, señale: *"Aquí tenemos un ejemplo claro de exceso de alcance. El documento no contiene proyecciones de ingresos, pero Copilot generó una respuesta. Esto es exactamente lo que debemos detectar y cuestionar."*

**Resultado esperado:** Copilot proporciona citas o fragmentos del documento para respaldar los datos principales. Al menos un caso muestra la diferencia entre dato explícito y dato inferido. La pregunta deliberada del punto 7 revela el comportamiento de Copilot ante información no disponible.

**Verificación:** Comparación visual directa entre las citas de Copilot y el contenido del PDF abierto en Adobe Acrobat Reader. Los estudiantes deben poder observar la correspondencia (o falta de ella) en la pantalla proyectada.

---

### Paso 8: Repetir el flujo con el archivo Word

**Objetivo:** Demostrar que el flujo de trabajo (resumen, extracción, transformación) funciona de manera consistente entre formatos de archivo (PDF → Word), y señalar cualquier diferencia de comportamiento.

**Instrucciones:**

1. Explique: *"Ahora vamos a repetir los pasos clave con un archivo Word para verificar que el comportamiento es consistente entre formatos. No repetiremos los 7 pasos completos, sino los 3 más representativos: carga, resumen y extracción."*

2. Inicie una **nueva conversación** en Copilot Chat (haga clic en **Nuevo chat**).

3. Haga clic en el ícono de clip (📎) y seleccione el archivo `LAB03_documento_practica_propuesta_v1.docx`.

4. Espere la confirmación de carga y señale: *"Observen que el proceso de adjuntar es idéntico para PDF y Word. Copilot Chat maneja ambos formatos de la misma manera."*

5. Escriba el prompt de resumen ejecutivo (similar al Paso 3):

```
Eres un gerente de proyectos.
Resume el documento adjunto como un resumen ejecutivo
de máximo 200 palabras, en tono profesional,
enfocado en el alcance del proyecto, los entregables
principales y los riesgos identificados.
```

6. Envíe y revise brevemente la respuesta. Señale similitudes y diferencias con el resumen del PDF.

7. Escriba un prompt de extracción (similar al Paso 5):

```
Extrae del documento adjunto:
1. Fechas clave y hitos del proyecto
2. Presupuesto o cifras financieras mencionadas
3. Responsables de cada entregable
4. Riesgos con su nivel de impacto

Si algún dato no está en el documento, indica
"No encontrado en el documento".
```

8. Envíe y revise la respuesta.

9. Cierre este segmento explicando: *"Como pueden ver, los mismos patrones de prompting funcionan independientemente del formato del archivo. La clave no es el formato, sino la calidad del prompt y la verificación posterior."*

**Resultado esperado:** Copilot Chat procesa el archivo Word de manera equivalente al PDF, generando un resumen ejecutivo y una lista de datos extraídos con estructura y calidad comparables.

**Verificación:** El archivo Word se adjunta sin errores, el resumen mantiene la extensión y tono solicitados, y la extracción incluye las categorías pedidas con la cláusula de "No encontrado" donde aplica.

---

### Paso 9: Recapitulación y registro de patrones por los estudiantes

**Objetivo:** Consolidar los cuatro patrones de prompting demostrados y dar tiempo a los estudiantes para completar sus notas antes del cierre.

**Instrucciones:**

1. Proyecte o dicte el siguiente resumen de patrones para que los estudiantes lo registren:

```
PATRONES DE PROMPTING DEMOSTRADOS — Lab 03-00-02

1. RESUMEN EJECUTIVO
   Estructura: Rol + "Resume el documento adjunto" + audiencia
   + tono + extensión máxima + enfoque + exclusiones
   
2. EXTRACCIÓN DIRIGIDA
   Estructura: "Extrae del documento adjunto" + lista de
   categorías específicas + formato de salida (lista/tabla)
   + cláusula de seguridad ("Si no aparece, indica...")
   
3. TRANSFORMACIÓN DE FORMATO
   Estructura: "Transforma la información anterior en"
   + formato deseado (tabla, lista, diagrama textual)
   + columnas o estructura + criterio de ordenamiento
   
4. VERIFICACIÓN DE FUENTE
   Estructura: "Para cada dato, cita el fragmento exacto
   del documento" + sección + nivel de confianza
   + instrucción de honestidad ante datos no respaldados
```

2. Dé 2 minutos para que los estudiantes completen sus notas.

3. Pregunte: *"¿Alguien tiene dudas sobre alguno de estos patrones antes de que los apliquen ustedes mismos en el próximo laboratorio?"*

4. Responda las preguntas que surjan.

**Resultado esperado:** Los estudiantes tienen registrados los cuatro patrones de prompting con su estructura, listos para aplicarlos en el Lab 04-00-01.

**Verificación:** Verificación informal: preguntar a 2-3 estudiantes que muestren o lean sus notas para confirmar que capturaron los patrones correctamente.

## Validación y Pruebas

Al finalizar la demostración, el instructor debe confirmar que se cumplieron los siguientes criterios de éxito:

| Criterio | Método de validación | ✅ / ❌ |
|---|---|---|
| Se cargó exitosamente un archivo PDF en Copilot Chat | El archivo apareció como adjunto visible en la conversación | |
| Se cargó exitosamente un archivo Word en Copilot Chat | El archivo apareció como adjunto visible en una segunda conversación | |
| Se generó un resumen ejecutivo con tono formal | La respuesta cumplió con extensión (~200 palabras), tono formal y enfoque solicitado | |
| Se demostró refinamiento iterativo (cambio de tono) | La segunda versión del resumen mostró tono conversacional manteniendo los mismos puntos clave | |
| Se extrajeron datos específicos en lista numerada | La respuesta incluyó las 5 categorías solicitadas con datos del documento o indicación de "No encontrado" | |
| Se transformó la lista en tabla | La tabla generada contenía las columnas solicitadas y los datos consistentes con la lista previa | |
| Se realizó verificación contra fuente | Copilot proporcionó citas o fragmentos del documento y se compararon visualmente con el PDF original | |
| Se identificó o provocó un exceso de alcance | Se demostró al menos un caso donde Copilot generó información no presente en el documento, o indicó correctamente que no la encontró | |
| Los estudiantes registraron los 4 patrones | Verificación informal con 2-3 estudiantes confirmó que tomaron notas de los patrones | |

**Pregunta de validación para los estudiantes** (hacer al cierre):

> *"Si tuvieran que explicarle a un colega los cuatro patrones de prompting que vimos hoy, ¿cuáles son y en qué orden los aplicarían?"*

Respuesta esperada: Resumen → Extracción → Transformación → Verificación.

## Solución de Problemas

### Problema 1: El botón de adjuntar archivos no aparece o está deshabilitado

**Síntomas:** Al abrir Copilot Chat en https://m365.cloud.microsoft/chat, el ícono de clip (📎) no es visible en la barra de entrada, o aparece en gris y no responde al hacer clic.

**Causa:** El modo activo es **Web** en lugar de **Trabajo**. La función de adjuntar archivos locales solo está disponible en modo Trabajo. Alternativamente, la cuenta del instructor puede no tener la licencia de Microsoft 365 Copilot Chat correctamente asignada, o la licencia fue asignada hace menos de 24 horas y aún no se ha propagado.

**Solución:**
1. Verifique el selector de modo en la interfaz de Copilot Chat. Si muestra "Web", cámbielo a **Trabajo**.
2. Si el modo Trabajo no está disponible como opción, cierre sesión y vuelva a iniciar sesión en https://m365.cloud.microsoft/chat.
3. Si persiste, abra una pestaña de incógnito/privada en Edge, navegue a https://m365.cloud.microsoft/chat e inicie sesión nuevamente.
4. Si el problema continúa, contacte al administrador de TI para verificar que la licencia de Microsoft 365 Copilot Chat está activa en la cuenta del instructor. La licencia debe haberse asignado al menos 24 horas antes.
5. **Plan de contingencia para la demostración:** Si no se puede resolver en 2 minutos, el instructor puede copiar y pegar el contenido del documento directamente en el chat (sin adjuntar el archivo) y explicar que el flujo con archivo adjunto es idéntico pero más conveniente. Marcar el problema para resolverlo antes del siguiente laboratorio.

---

### Problema 2: Copilot Chat genera un resumen que no corresponde al contenido del archivo adjunto

**Síntomas:** Tras adjuntar el archivo y solicitar un resumen, la respuesta de Copilot contiene información que claramente no está en el documento (temas diferentes, datos de otro contexto, o un resumen genérico que podría aplicarse a cualquier documento).

**Causa:** Esto puede ocurrir si: (a) el archivo no se adjuntó correctamente y Copilot está respondiendo desde su conocimiento general, (b) el archivo es demasiado grande o tiene un formato que Copilot no pudo procesar completamente (por ejemplo, PDF escaneado como imagen sin OCR), o (c) hay una conversación previa con contexto residual que interfiere.

**Solución:**
1. Verifique que el nombre del archivo aparece como adjunto en la conversación. Si no aparece, vuelva a adjuntarlo.
2. Inicie un **Nuevo chat** para eliminar cualquier contexto residual de conversaciones anteriores.
3. Adjunte el archivo nuevamente en la conversación limpia.
4. Reformule el prompt incluyendo una referencia explícita al archivo: *"Basándote exclusivamente en el documento adjunto [nombre del archivo], resume..."*
5. Si el problema persiste con el PDF, pruebe con el archivo Word como alternativa. Algunos PDFs con formato complejo (tablas anidadas, imágenes con texto, escaneos) pueden procesarse de forma incompleta.
6. Verifique que el archivo no supera los 5 MB recomendados. Si es más grande, use una versión reducida.
7. **Nota pedagógica:** Si este problema ocurre durante la demostración, aprovéchelo como ejemplo real de por qué la verificación (Paso 7) es esencial. Diga a los estudiantes: *"Esto es exactamente lo que puede pasar en su trabajo diario. Por eso siempre verificamos."*

## Limpieza

Al finalizar la demostración:

1. **Conversaciones de Copilot Chat:** No es necesario eliminar las conversaciones. Pueden servir como referencia si el instructor necesita mostrar los resultados nuevamente. Sin embargo, si la política de la organización requiere limpieza:
   - Haga clic en el menú de opciones (⋯) junto a cada conversación en el panel lateral.
   - Seleccione **Eliminar** para cada conversación creada durante la demo.

2. **Archivos de práctica:** Los archivos locales (`LAB03_documento_practica_negocio_v1.pdf` y `LAB03_documento_practica_propuesta_v1.docx`) deben conservarse en la carpeta del instructor para posible reutilización. No es necesario eliminarlos.

3. **Ventanas del navegador:** Cierre las pestañas de Adobe Acrobat Reader que se abrieron para la verificación visual. Mantenga la pestaña de Copilot Chat abierta si hay actividades subsiguientes.

4. **Notas de los estudiantes:** Confirme que los estudiantes han guardado sus notas con los cuatro patrones de prompting, ya que las necesitarán para el Lab 04-00-01.

## Resumen

En esta demostración se cubrió el flujo completo de trabajo con archivos adjuntos en Microsoft 365 Copilot Chat, organizado en cuatro patrones de prompting fundamentales:

| Patrón | Propósito | Elemento clave del prompt |
|---|---|---|
| **Resumen ejecutivo** | Sintetizar un documento completo para una audiencia específica | Rol + audiencia + tono + extensión + enfoque + exclusiones |
| **Extracción dirigida** | Localizar datos concretos dentro del documento | Categorías específicas + formato de salida + cláusula de seguridad |
| **Transformación de formato** | Convertir información en una estructura visual diferente | Formato deseado + columnas/estructura + criterio de ordenamiento |
| **Verificación de fuente** | Confirmar que las respuestas están ancladas en el documento | Solicitud de citas textuales + sección + nivel de confianza |

**Lecciones clave para los estudiantes:**

- La especificidad del prompt determina la calidad de la respuesta. Un prompt vago genera resultados genéricos.
- El refinamiento iterativo permite ajustar tono, extensión y enfoque sin repetir todo el contexto.
- La cláusula de seguridad (*"Si no aparece, indica 'No encontrado'"*) es una herramienta esencial para prevenir alucinaciones.
- La verificación contra la fuente original es un paso **no negociable** en cualquier flujo profesional con IA generativa.
- Los patrones funcionan de manera consistente entre formatos de archivo (PDF y Word).

### Conexión con el siguiente laboratorio

Los cuatro patrones demostrados en esta sesión son los bloques fundamentales que los estudiantes aplicarán de forma autónoma en el **Lab 04-00-01** (reto integrador). Se recomienda que los estudiantes revisen sus notas antes de iniciar ese laboratorio.

### Recursos adicionales

- [Microsoft Learn — Adjuntar archivos en Microsoft 365 Copilot Chat](https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-overview)
- [Microsoft Adoption — Guía de prompting para Microsoft 365 Copilot](https://adoption.microsoft.com/es-es/copilot/)
- [Plain Language Guidelines — Simplificación de textos profesionales](https://www.plainlanguage.gov/guidelines/)
