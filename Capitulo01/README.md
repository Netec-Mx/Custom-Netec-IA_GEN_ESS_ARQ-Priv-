# Laboratorio 1. Mi mapa de oportunidades y riesgos: identificar tareas de mi rol que puedo apoyar con Copilot Chat y definir controles de uso

## Metadatos

| Campo | Detalle |
|---|---|
| **Duración** | 80 minutos |
| **Complejidad** | Media |
| **Nivel Bloom** | Crear |

## Descripción General

En este laboratorio inaugural explorarás la interfaz de Microsoft 365 Copilot Chat, identificarás tareas recurrentes de tu rol profesional que pueden apoyarse con IA generativa y las clasificarás según su tipo de soporte y nivel de riesgo. Construirás un **mapa personal de oportunidades y riesgos** en un documento de trabajo estructurado, definirás controles de uso responsable y ejecutarás tus primeros prompts reales en Copilot Chat para evaluar la calidad de las respuestas. Este documento servirá como insumo para los laboratorios posteriores del curso.

## Objetivos de Aprendizaje

Al completar este laboratorio serás capaz de:

- [ ] Identificar al menos cinco tareas recurrentes de tu propio rol laboral que podrían apoyarse con Copilot Chat, clasificándolas por tipo (redactar, resumir, transformar, analizar, comparar, idear).
- [ ] Distinguir entre tareas de bajo riesgo y tareas de alto riesgo para el uso de IA generativa, aplicando criterios de privacidad, alucinaciones y responsabilidad profesional.
- [ ] Definir controles de uso personales que especifiquen qué información no compartir, qué verificar antes de usar una respuesta y en qué casos no delegar a Copilot Chat.
- [ ] Explorar la interfaz de Microsoft 365 Copilot Chat e identificar sus elementos principales, incluyendo el modo Web, el modo Trabajo y la función de adjuntar archivos.
- [ ] Formular y ejecutar al menos tres prompts iniciales en Copilot Chat relacionados con tareas reales del participante, evaluando la calidad y confiabilidad de las respuestas obtenidas.

## Prerrequisitos

### Conocimientos previos

- Comprensión básica de qué es la IA generativa, sus capacidades (redactar, resumir, transformar, idear, analizar) y sus limitaciones fundamentales (fecha de corte, alucinaciones, sensibilidad al prompt), tal como se cubrió en la **Lección 1.1**.
- Entendimiento del principio de que el criterio humano es la capa final de validación de cualquier contenido generado por IA.
- Conocimiento general de las tareas habituales de tu propio rol profesional.

### Acceso y recursos

- Cuenta corporativa con licencia de **Microsoft 365 Copilot Chat** habilitada (verificada al menos 24 horas antes del laboratorio).
- Navegador web compatible: **Microsoft Edge 124.0.2478.97** o **Google Chrome 124.0.6367.119**.
- Conexión a Internet estable (mínimo 5 Mbps por participante).
- Archivo de plantilla proporcionado por el instructor: **`LAB01_plantilla_mapa_oportunidades_v1.docx`**.
- Acceso a **Microsoft Word** (versión 2404, Build 17531.20152) para editar la plantilla.

## Entorno de Laboratorio

### Hardware requerido

| Componente | Requisito mínimo | Recomendado |
|---|---|---|
| Procesador | 64 bits, 2 núcleos | Intel Core i5 / AMD Ryzen 5 o superior |
| RAM | 8 GB | 16 GB |
| Pantalla | 1280 × 768 | 1920 × 1080 |
| Internet | 5 Mbps de bajada | 10 Mbps de bajada |
| Periféricos | Teclado y ratón | Webcam y micrófono (sesiones remotas) |

### Software requerido

| Software | Versión | Propósito |
|---|---|---|
| Microsoft Edge o Google Chrome | Edge 124.0.2478.97 / Chrome 124.0.6367.119 | Navegador para acceder a Copilot Chat |
| Microsoft 365 Copilot Chat (web) | Servicio activo (mayo 2025) | Plataforma principal del laboratorio |
| Microsoft Word | 2404 (Build 17531.20152) | Edición de la plantilla del mapa |

### Configuración inicial

1. Abre tu navegador y navega a **https://copilot.microsoft.com**.
2. Inicia sesión con tu cuenta corporativa (correo y contraseña proporcionados por tu organización).
3. Verifica que la interfaz de Copilot Chat cargue correctamente y que tu nombre de usuario aparezca en la esquina superior derecha.
4. Abre el archivo **`LAB01_plantilla_mapa_oportunidades_v1.docx`** en Microsoft Word. Confirma que puedes editarlo.
5. Organiza tu pantalla con el navegador (Copilot Chat) en una mitad y Word en la otra mitad para facilitar el trabajo simultáneo.

> **Nota:** No cierres la sesión de Copilot Chat durante todo el laboratorio. Trabajarás en una misma sesión continua para los pasos de exploración y ejecución de prompts.

## Instrucciones Paso a Paso

---

### Paso 1: Explorar la interfaz de Microsoft 365 Copilot Chat

**Objetivo:** Familiarizarte con los componentes principales de la interfaz de Copilot Chat, identificando el campo de entrada de prompts, los modos Web y Trabajo, y la función de adjuntar archivos.

**Instrucciones:**

1. En tu navegador, confirma que estás en **https://copilot.microsoft.com** con tu cuenta corporativa activa.

2. Observa la interfaz principal y localiza los siguientes elementos:
   - **Campo de entrada de prompt:** el cuadro de texto en la parte inferior de la pantalla donde escribirás tus instrucciones.
   - **Selector de modo:** busca el control que permite alternar entre **modo Web** y **modo Trabajo (Work)**. Generalmente se encuentra cerca del campo de entrada o en la parte superior de la conversación.
   - **Botón de adjuntar archivos:** identifica el ícono de clip (📎) o el botón que permite cargar archivos a la conversación.
   - **Área de respuesta:** la zona central donde aparecerán las respuestas de Copilot Chat.
   - **Historial de conversaciones:** el panel lateral (si está visible) que muestra conversaciones anteriores.

3. Cambia al **modo Trabajo (Work)** haciendo clic en el selector correspondiente. Confirma visualmente que el modo activo es "Trabajo" o "Work".

4. Haz clic en el botón de adjuntar archivos (📎) para verificar que la opción está disponible. **No adjuntes ningún archivo todavía**; solo confirma que la funcionalidad aparece. Cierra el diálogo de selección de archivos.

5. Cambia brevemente al **modo Web** para observar la diferencia en la interfaz. Luego regresa al **modo Trabajo (Work)**.

6. En tu plantilla **`LAB01_plantilla_mapa_oportunidades_v1.docx`**, localiza la **Sección 1: Exploración de la interfaz** y completa la siguiente tabla de registro:

   | Elemento de la interfaz | ¿Lo encontraste? (Sí/No) | Ubicación en pantalla | Observaciones |
   |---|---|---|---|
   | Campo de entrada de prompt | | | |
   | Selector de modo (Web / Trabajo) | | | |
   | Botón de adjuntar archivos | | | |
   | Área de respuesta | | | |
   | Historial de conversaciones | | | |

7. Escribe tu primer prompt de prueba en modo Trabajo para confirmar que la herramienta responde correctamente:

   ```
   Hola, ¿puedes confirmarme en qué modo estás operando actualmente y qué tipo de información puedes consultar en este modo?
   ```

8. Lee la respuesta de Copilot Chat. Observa si menciona el acceso a datos de tu organización (modo Trabajo) o solo información de la web.

**Resultado esperado:** Has identificado y documentado los cinco elementos principales de la interfaz de Copilot Chat. Copilot Chat responde a tu prompt de prueba y confirma que opera en modo Trabajo con acceso a datos organizacionales.

**Verificación:**
- ✅ La tabla de registro en tu plantilla tiene las cinco filas completadas con "Sí" en la columna de localización.
- ✅ Copilot Chat generó una respuesta coherente a tu prompt de prueba.
- ✅ El modo activo es **Trabajo (Work)**.

> ⏱ **Tiempo estimado:** 10 minutos

---

### Paso 2: Listar y clasificar tareas recurrentes de tu rol profesional

**Objetivo:** Identificar al menos cinco tareas laborales recurrentes que realizas en tu rol y clasificarlas según el tipo de soporte que Copilot Chat podría ofrecer.

**Instrucciones:**

1. Antes de interactuar con Copilot Chat, realiza un ejercicio de reflexión individual. Piensa en tu semana laboral típica y anota en la **Sección 2** de tu plantilla al menos **siete tareas recurrentes** que realizas habitualmente. Ejemplos orientativos (adáptalos a tu rol real):
   - Redactar correos de seguimiento a clientes
   - Resumir minutas de reuniones
   - Preparar reportes semanales de avance
   - Comparar propuestas de proveedores
   - Generar ideas para campañas o proyectos
   - Transformar datos de una tabla a formato narrativo
   - Analizar retroalimentación de encuestas

2. Para cada tarea listada, asígnale una **categoría de soporte de IA** usando la siguiente clasificación (una tarea puede tener más de una categoría):

   | Categoría | Descripción | Ejemplo |
   |---|---|---|
   | **Redactar** | Generar texto nuevo desde cero o a partir de instrucciones | Borrador de correo, descripción de puesto |
   | **Resumir** | Condensar información extensa en puntos clave | Resumen ejecutivo de un informe |
   | **Transformar** | Cambiar formato o estructura de contenido existente | Convertir tabla en párrafo narrativo |
   | **Analizar** | Identificar patrones, temas o inconsistencias | Revisar retroalimentación de clientes |
   | **Comparar** | Contrastar dos o más opciones o documentos | Evaluar propuestas de proveedores |
   | **Idear** | Generar alternativas, lluvia de ideas o criterios | Proponer nombres para un proyecto |

3. Ahora utiliza Copilot Chat para enriquecer tu lista. Escribe el siguiente prompt (personalízalo con tu rol real):

   ```
   Soy [tu rol, por ejemplo: coordinador de proyectos en una empresa de tecnología]. 
   Estas son algunas tareas que realizo semanalmente:
   1. [Tarea 1]
   2. [Tarea 2]
   3. [Tarea 3]
   
   ¿Puedes sugerirme otras tareas típicas de este rol que podrían beneficiarse 
   del apoyo de una herramienta de IA generativa? Para cada sugerencia, indica 
   qué tipo de soporte ofrecería la IA: redactar, resumir, transformar, analizar, 
   comparar o idear.
   ```

4. Revisa la respuesta de Copilot Chat. Evalúa críticamente cada sugerencia:
   - ¿La tarea es realmente parte de tu rol o es genérica?
   - ¿La categoría de soporte asignada es correcta?
   - ¿Hay alguna sugerencia que no aplique a tu contexto?

5. Incorpora a tu lista las sugerencias que consideres válidas. Descarta las que no apliquen. Tu lista final debe tener **al menos siete tareas** (mínimo cinco propias + las que adoptes de las sugerencias).

6. Completa la tabla en la **Sección 2** de tu plantilla con el siguiente formato:

   | # | Tarea recurrente | Categoría(s) de soporte | Origen (propia / sugerida por IA) |
   |---|---|---|---|
   | 1 | | | |
   | 2 | | | |
   | 3 | | | |
   | 4 | | | |
   | 5 | | | |
   | 6 | | | |
   | 7 | | | |

**Resultado esperado:** Una tabla con al menos siete tareas recurrentes de tu rol, cada una clasificada por tipo de soporte de IA, con indicación de si fue identificada por ti o sugerida por Copilot Chat.

**Verificación:**
- ✅ La tabla contiene al menos siete tareas.
- ✅ Cada tarea tiene al menos una categoría de soporte asignada (redactar, resumir, transformar, analizar, comparar o idear).
- ✅ Al menos cinco tareas fueron identificadas por ti antes de consultar a Copilot Chat.
- ✅ Las sugerencias de Copilot Chat fueron evaluadas críticamente (no se aceptaron sin revisión).

> ⏱ **Tiempo estimado:** 15 minutos

---

### Paso 3: Evaluar el riesgo de cada tarea para el uso de IA generativa

**Objetivo:** Clasificar cada tarea identificada según su nivel de riesgo al ser apoyada por IA generativa, considerando criterios de privacidad, posibilidad de alucinación e impacto de un error.

**Instrucciones:**

1. Revisa tu lista de tareas del Paso 2. Para cada una, vas a evaluar tres dimensiones de riesgo. Antes de hacerlo, lee las definiciones de cada dimensión:

   | Dimensión de riesgo | Pregunta clave | Ejemplos de riesgo alto |
   |---|---|---|
   | **Privacidad de datos** | ¿Necesitaría compartir con Copilot Chat información personal, confidencial o regulada? | Datos de clientes con nombre y RFC, información financiera no pública, datos de salud de empleados |
   | **Posibilidad de alucinación** | ¿La tarea requiere datos factuales verificables (cifras, fechas, nombres, regulaciones) que el modelo podría inventar? | Citar normativas legales específicas, reportar cifras financieras exactas, mencionar nombres de personas reales |
   | **Impacto de un error** | Si la respuesta de Copilot Chat contuviera un error y yo no lo detectara, ¿cuál sería la consecuencia? | Decisión de negocio incorrecta, comunicación oficial con datos falsos, problema legal o regulatorio |

2. Para cada tarea, asigna un nivel de riesgo en cada dimensión usando la escala:
   - 🟢 **Bajo:** riesgo mínimo o nulo en esta dimensión.
   - 🟡 **Medio:** riesgo moderado que requiere precaución y verificación.
   - 🔴 **Alto:** riesgo significativo; se requieren controles estrictos o podría no ser apropiado usar IA.

3. Determina el **nivel de riesgo global** de cada tarea aplicando esta regla simple:
   - Si **cualquier dimensión es 🔴**, el riesgo global es **Alto**.
   - Si **ninguna dimensión es 🔴 pero al menos una es 🟡**, el riesgo global es **Medio**.
   - Si **todas las dimensiones son 🟢**, el riesgo global es **Bajo**.

4. Utiliza Copilot Chat para contrastar tu evaluación. Escribe el siguiente prompt:

   ```
   Estoy evaluando el riesgo de usar IA generativa para apoyar estas tareas 
   laborales. Para cada una, necesito que me ayudes a identificar posibles 
   riesgos en tres dimensiones: privacidad de datos, posibilidad de que la IA 
   genere información incorrecta (alucinación) y el impacto que tendría un 
   error no detectado.
   
   Tareas:
   1. [Tarea 1 de tu lista]
   2. [Tarea 2 de tu lista]
   3. [Tarea 3 de tu lista]
   [incluye todas tus tareas]
   
   Para cada tarea, indica el nivel de riesgo (bajo, medio o alto) en cada 
   dimensión y explica brevemente por qué.
   ```

5. Compara la evaluación de Copilot Chat con la tuya. Presta especial atención a:
   - ¿Coinciden en las tareas de alto riesgo?
   - ¿Copilot Chat identificó algún riesgo que tú no habías considerado?
   - ¿Hay alguna evaluación de Copilot Chat que consideres incorrecta para tu contexto específico?

   > **Reflexión importante:** Recuerda que la evaluación de riesgo de Copilot Chat es genérica. Tú conoces el contexto real de tu organización, la sensibilidad de los datos que manejas y las consecuencias reales de un error en tu entorno. Tu criterio profesional prevalece sobre la sugerencia del modelo.

6. Completa la tabla de evaluación de riesgo en la **Sección 3** de tu plantilla:

   | # | Tarea | Privacidad | Alucinación | Impacto de error | Riesgo global |
   |---|---|---|---|---|---|
   | 1 | | 🟢/🟡/🔴 | 🟢/🟡/🔴 | 🟢/🟡/🔴 | Bajo/Medio/Alto |
   | 2 | | | | | |
   | ... | | | | | |

**Resultado esperado:** Una tabla completa de evaluación de riesgo para todas tus tareas, con niveles asignados en las tres dimensiones y un riesgo global calculado. Habrás contrastado tu evaluación con la de Copilot Chat y tomado decisiones informadas sobre las diferencias.

**Verificación:**
- ✅ Todas las tareas tienen evaluación en las tres dimensiones de riesgo.
- ✅ El riesgo global de cada tarea es consistente con la regla de clasificación indicada.
- ✅ Al menos una tarea está clasificada como riesgo alto y al menos una como riesgo bajo (si tu lista es realista, esto debería ocurrir naturalmente).
- ✅ Documentaste al menos una diferencia o coincidencia notable entre tu evaluación y la de Copilot Chat.

> ⏱ **Tiempo estimado:** 15 minutos

---

### Paso 4: Construir el mapa de oportunidades y riesgos

**Objetivo:** Integrar las tareas clasificadas y evaluadas en una matriz visual de dos ejes (potencial de beneficio × nivel de riesgo) que constituya tu mapa personal de oportunidades y riesgos.

**Instrucciones:**

1. En la **Sección 4** de tu plantilla, localiza la matriz de dos ejes con el siguiente formato:

   ```
                        POTENCIAL DE BENEFICIO
                    Bajo          Medio          Alto
              ┌─────────────┬──────────────┬──────────────┐
   Riesgo     │             │              │              │
   Alto       │  EVITAR o   │  USAR CON    │  USAR CON    │
              │  NO USAR    │  CONTROLES   │  CONTROLES   │
              │             │  ESTRICTOS   │  ESTRICTOS   │
              ├─────────────┼──────────────┼──────────────┤
   Riesgo     │             │              │              │
   Medio      │  EVALUAR    │  USAR CON    │  USAR CON    │
              │  CASO A     │  VERIFICACIÓN│  VERIFICACIÓN│
              │  CASO       │              │              │
              ├─────────────┼──────────────┼──────────────┤
   Riesgo     │             │              │              │
   Bajo       │  OPCIONAL   │  USAR        │  PRIORIZAR   │
              │             │  LIBREMENTE  │  (QUICK WINS)│
              │             │              │              │
              └─────────────┴──────────────┴──────────────┘
   ```

2. Para cada tarea de tu lista, evalúa su **potencial de beneficio** al usar Copilot Chat:
   - **Alto:** la tarea consume mucho tiempo, es repetitiva o requiere generar contenido desde cero; Copilot Chat podría ahorrar significativamente tiempo o mejorar calidad.
   - **Medio:** la tarea se beneficiaría parcialmente del apoyo de IA, pero requiere mucho contexto específico o juicio experto.
   - **Bajo:** la tarea es muy rápida de hacer manualmente, o el esfuerzo de formular un buen prompt supera el beneficio.

3. Ubica cada tarea en el cuadrante correspondiente de la matriz, combinando el riesgo global (del Paso 3) con el potencial de beneficio. Escribe el nombre o número de cada tarea en el cuadrante que le corresponda.

4. Identifica visualmente:
   - **Tus "Quick Wins"** (cuadrante inferior derecho): tareas de bajo riesgo y alto beneficio. Estas son las primeras candidatas para usar Copilot Chat de forma regular.
   - **Tus tareas de "Controles estrictos"** (fila superior): tareas de alto riesgo donde, si decides usar Copilot Chat, necesitarás protocolos claros de verificación.
   - **Tus tareas a "Evitar"** (cuadrante superior izquierdo): tareas de alto riesgo y bajo beneficio donde el uso de IA no se justifica.

5. Debajo de la matriz, escribe un párrafo de **3 a 5 oraciones** que resuma tu hallazgo principal. Ejemplo de estructura:

   > "De las [X] tareas analizadas, [Y] se ubican como oportunidades prioritarias (Quick Wins) porque [razón]. Las tareas de mayor riesgo en mi rol son [ejemplos] debido a [razón de riesgo]. Mi estrategia inicial será comenzar usando Copilot Chat para [tareas específicas] y evitar su uso para [tareas específicas] hasta contar con protocolos de verificación adecuados."

**Resultado esperado:** Una matriz visual completada con todas tus tareas ubicadas en sus cuadrantes correspondientes, acompañada de un párrafo de análisis personal.

**Verificación:**
- ✅ Todas las tareas de tu lista aparecen ubicadas en algún cuadrante de la matriz.
- ✅ Has identificado al menos un "Quick Win" y al menos una tarea de alto riesgo.
- ✅ El párrafo de análisis refleja una decisión informada basada en la matriz.

> ⏱ **Tiempo estimado:** 10 minutos

---

### Paso 5: Definir controles de uso responsable personales

**Objetivo:** Establecer reglas personales claras que definan qué información no compartir con Copilot Chat, qué verificar antes de usar una respuesta y en qué casos no delegar a la herramienta.

**Instrucciones:**

1. Basándote en tu evaluación de riesgo (Paso 3) y tu mapa (Paso 4), vas a redactar tres tipos de controles personales. Comienza reflexionando sobre estas preguntas:

   - **¿Qué información NO debo compartir con Copilot Chat?** Piensa en datos personales de terceros, información financiera confidencial, contraseñas, datos regulados (salud, legal), propiedad intelectual sensible.
   - **¿Qué debo verificar SIEMPRE antes de usar una respuesta?** Piensa en cifras, fechas, nombres de personas, citas textuales, normativas legales, datos que cambien frecuentemente.
   - **¿En qué situaciones NO debo delegar a Copilot Chat?** Piensa en decisiones con consecuencias legales, comunicaciones que requieren empatía genuina, situaciones donde un error es inaceptable.

2. Utiliza Copilot Chat para obtener una perspectiva adicional. Escribe el siguiente prompt:

   ```
   Soy [tu rol] y estoy definiendo mis reglas personales para el uso responsable 
   de IA generativa en mi trabajo. Basándote en las mejores prácticas de uso 
   responsable de IA en entornos corporativos, sugiere:
   
   1. Cinco tipos de información que un profesional en mi rol NO debería 
      compartir con un asistente de IA.
   2. Cinco elementos que siempre debería verificar antes de usar una respuesta 
      generada por IA.
   3. Tres situaciones laborales donde NO es recomendable delegar a una 
      herramienta de IA generativa.
   
   Sé específico para mi rol y contexto profesional.
   ```

3. Revisa las sugerencias de Copilot Chat y compáralas con tu reflexión inicial. Recuerda: **las sugerencias del modelo son genéricas; tú debes adaptarlas a las políticas y contexto real de tu organización.**

4. Redacta tus controles personales en la **Sección 5** de tu plantilla, usando el siguiente formato:

   **Lista de NO compartir (información restringida):**
   | # | Tipo de información | Razón | Ejemplo concreto de mi rol |
   |---|---|---|---|
   | 1 | | | |
   | 2 | | | |
   | 3 | | | |
   | 4 | | | |
   | 5 | | | |

   **Lista de verificación obligatoria (antes de usar cualquier respuesta):**
   | # | Elemento a verificar | Método de verificación | Fuente de contraste |
   |---|---|---|---|
   | 1 | | | |
   | 2 | | | |
   | 3 | | | |
   | 4 | | | |
   | 5 | | | |

   **Situaciones de NO delegación:**
   | # | Situación | Por qué no delegar | Qué hacer en su lugar |
   |---|---|---|---|
   | 1 | | | |
   | 2 | | | |
   | 3 | | | |

5. Lee tus controles completos una vez más y pregúntate: "Si un colega nuevo en mi equipo leyera estas reglas, ¿podría seguirlas sin ambigüedad?" Si la respuesta es no, refina la redacción para que sea más concreta y accionable.

**Resultado esperado:** Tres tablas de controles personales completadas: información restringida (mínimo 5 ítems), verificación obligatoria (mínimo 5 ítems) y situaciones de no delegación (mínimo 3 ítems).

**Verificación:**
- ✅ La lista de "NO compartir" tiene al menos 5 tipos de información con razones y ejemplos concretos.
- ✅ La lista de verificación tiene al menos 5 elementos con métodos y fuentes de contraste específicos.
- ✅ Las situaciones de no delegación incluyen alternativas claras ("qué hacer en su lugar").
- ✅ Los controles son específicos a tu rol, no genéricos.

> ⏱ **Tiempo estimado:** 15 minutos

---

### Paso 6: Ejecutar prompts iniciales y evaluar respuestas

**Objetivo:** Formular y ejecutar al menos tres prompts en Copilot Chat relacionados con tareas reales de tu rol, aplicando una lista de verificación básica para evaluar la calidad y confiabilidad de cada respuesta.

**Instrucciones:**

1. De tu mapa de oportunidades (Paso 4), selecciona **tres tareas** que estén en los cuadrantes de "Quick Wins" o "Usar con verificación" (riesgo bajo o medio, beneficio medio o alto).

2. Para cada tarea seleccionada, redacta un prompt que le pida a Copilot Chat realizar esa tarea. Sigue estas pautas al formular tus prompts:
   - **Sé específico:** indica el contexto, el formato deseado y el público objetivo.
   - **Define el alcance:** especifica qué incluir y qué no incluir.
   - **Pide un formato concreto:** lista, tabla, párrafo, correo electrónico, etc.

   **Ejemplo de prompt bien formulado:**
   ```
   Soy coordinador de proyectos de TI. Necesito redactar un correo de 
   seguimiento para el equipo de desarrollo sobre el proyecto de migración 
   a la nube. El correo debe:
   - Tener un tono profesional pero cercano
   - Recordar los tres entregables pendientes para esta semana
   - Solicitar una actualización de estatus antes del viernes
   - No superar los 150 palabras
   
   Los entregables pendientes son: documentación de APIs, pruebas de 
   integración y plan de rollback.
   ```

   **Ejemplo de prompt poco efectivo (evitar):**
   ```
   Escribe un correo para mi equipo.
   ```

3. Ejecuta tus tres prompts en Copilot Chat, uno a la vez. Para cada respuesta, **cópiala** y pégala en la **Sección 6** de tu plantilla.

4. Para cada respuesta, aplica la siguiente **Lista de Verificación de Confiabilidad**:

   | Criterio | Pregunta | Evaluación (✅/⚠️/❌) | Observaciones |
   |---|---|---|---|
   | **Relevancia** | ¿La respuesta aborda lo que pedí? | | |
   | **Completitud** | ¿Incluye todos los elementos que solicité? | | |
   | **Precisión factual** | ¿Los datos, cifras o hechos mencionados son correctos? (Si aplica) | | |
   | **Tono y formato** | ¿El tono y formato coinciden con lo solicitado? | | |
   | **Invenciones** | ¿Hay información que parece inventada o que no puedo verificar? | | |
   | **Usabilidad** | ¿Podría usar esta respuesta tal cual, o necesita edición? | | |

   Usa la siguiente escala:
   - ✅ = Cumple satisfactoriamente
   - ⚠️ = Cumple parcialmente, requiere ajuste
   - ❌ = No cumple o es problemático

5. Debajo de cada evaluación, escribe una **nota de acción** de 1-2 oraciones: ¿usarías esta respuesta tal cual? ¿Qué editarías? ¿Qué verificarías externamente?

6. Si alguna respuesta obtuvo ⚠️ o ❌ en algún criterio, **reformula el prompt** para intentar mejorar el resultado. Ejecuta el prompt mejorado y compara ambas respuestas. Documenta qué cambió en el prompt y cómo mejoró (o no) la respuesta.

   > **Conexión con la Lección 1.1:** Recuerda que los LLM son sensibles al prompt. Pequeños cambios en la instrucción pueden producir respuestas muy distintas. Este ejercicio te permite experimentar directamente con esa sensibilidad.

**Resultado esperado:** Tres prompts ejecutados con sus respuestas documentadas, cada uno evaluado con la lista de verificación de confiabilidad. Al menos un prompt fue refinado para mejorar la respuesta.

**Verificación:**
- ✅ Has ejecutado al menos tres prompts diferentes, cada uno relacionado con una tarea real de tu rol.
- ✅ Cada respuesta tiene la lista de verificación de confiabilidad completada.
- ✅ Cada respuesta tiene una nota de acción indicando si es usable, qué editar o qué verificar.
- ✅ Al menos un prompt fue reformulado y la nueva respuesta fue comparada con la original.

> ⏱ **Tiempo estimado:** 15 minutos

---

### Paso 7: Consolidar el mapa y preparar el documento final

**Objetivo:** Integrar todos los elementos trabajados en un documento cohesivo que sirva como referencia personal y como insumo para los laboratorios posteriores del curso.

**Instrucciones:**

1. Revisa tu plantilla **`LAB01_plantilla_mapa_oportunidades_v1.docx`** completa. Confirma que las siguientes secciones están terminadas:
   - ✅ Sección 1: Exploración de la interfaz (tabla de elementos)
   - ✅ Sección 2: Tareas recurrentes clasificadas (mínimo 7 tareas)
   - ✅ Sección 3: Evaluación de riesgo por tarea (tres dimensiones + riesgo global)
   - ✅ Sección 4: Matriz de oportunidades y riesgos + párrafo de análisis
   - ✅ Sección 5: Controles de uso responsable (tres tablas)
   - ✅ Sección 6: Prompts ejecutados con evaluación de respuestas

2. Localiza la **Sección 7: Reflexión final** de tu plantilla y responde las siguientes tres preguntas en 2-3 oraciones cada una:

   **a) ¿Cuál es la tarea de mi rol donde Copilot Chat puede generar mayor impacto positivo y por qué?**

   **b) ¿Cuál es el riesgo más importante que debo gestionar al usar IA generativa en mi trabajo y cómo planeo mitigarlo?**

   **c) ¿Qué aprendí hoy sobre las capacidades y limitaciones de la IA generativa que cambia la forma en que la usaré?**

3. Guarda tu documento con el nombre: **`LAB01_mapa_oportunidades_[TuNombre]_v1.docx`**

   Ejemplo: `LAB01_mapa_oportunidades_CarlosGomez_v1.docx`

4. Si el instructor lo indica, comparte tu documento en la ubicación designada (carpeta compartida, Teams, etc.).

5. **Preparación para el Laboratorio 2:** Tu mapa de oportunidades y riesgos será un insumo directo para el siguiente laboratorio. Asegúrate de que el archivo esté accesible y que puedas localizarlo fácilmente.

**Resultado esperado:** Un documento completo, guardado con la nomenclatura correcta, con todas las siete secciones terminadas y listo para ser utilizado como referencia personal y como insumo en el Laboratorio 2.

**Verificación:**
- ✅ Las siete secciones de la plantilla están completas.
- ✅ Las tres preguntas de reflexión final están respondidas con contenido sustantivo (no genérico).
- ✅ El archivo está guardado con la nomenclatura correcta.
- ✅ El documento es legible y coherente si alguien más lo revisara.

> ⏱ **Tiempo estimado:** 10 minutos (incluye revisión final)

---

## Validación y Pruebas

Antes de considerar el laboratorio completado, verifica que cumples con **todos** los criterios siguientes:

### Lista de validación integral

| # | Criterio | Cumple (✅/❌) |
|---|---|---|
| 1 | Identifiqué y documenté los cinco elementos principales de la interfaz de Copilot Chat | |
| 2 | Confirmé que puedo operar en modo Trabajo (Work) y que la función de adjuntar archivos está disponible | |
| 3 | Listé al menos siete tareas recurrentes de mi rol con su categoría de soporte de IA | |
| 4 | Al menos cinco tareas fueron identificadas por mí antes de consultar a Copilot Chat | |
| 5 | Evalué cada tarea en tres dimensiones de riesgo (privacidad, alucinación, impacto de error) | |
| 6 | Construí la matriz de oportunidades y riesgos con todas las tareas ubicadas en cuadrantes | |
| 7 | Identifiqué al menos un "Quick Win" y al menos una tarea de alto riesgo | |
| 8 | Definí al menos 5 tipos de información que no debo compartir con Copilot Chat | |
| 9 | Definí al menos 5 elementos que debo verificar antes de usar cualquier respuesta de IA | |
| 10 | Identifiqué al menos 3 situaciones donde no debo delegar a Copilot Chat | |
| 11 | Ejecuté al menos 3 prompts relacionados con tareas reales de mi rol | |
| 12 | Evalué cada respuesta con la lista de verificación de confiabilidad | |
| 13 | Reformulé al menos un prompt para mejorar la respuesta y documenté la comparación | |
| 14 | Completé las tres preguntas de reflexión final | |
| 15 | Guardé el documento con la nomenclatura correcta | |

**Criterio de aprobación:** Al menos **13 de 15** criterios marcados con ✅.

### Prueba de calidad del mapa

Para verificar que tu mapa tiene la profundidad adecuada, aplica esta prueba rápida:

1. **Prueba de especificidad:** Lee tus tareas listadas. Si alguien de otro departamento las leyera, ¿sabría que son de tu rol específico? Si suenan demasiado genéricas (por ejemplo, "hacer informes"), refínalas con más contexto (por ejemplo, "elaborar el informe semanal de incidentes de ciberseguridad para el comité directivo").

2. **Prueba de accionabilidad de controles:** Lee tus controles de uso responsable. ¿Cada control describe una acción concreta que puedes ejecutar? Si dice "tener cuidado con datos sensibles", cámbialo a "no ingresar nombres, RFC ni datos de contacto de clientes en el prompt".

3. **Prueba de honestidad en la evaluación de respuestas:** Revisa tus evaluaciones del Paso 6. ¿Marcaste algún ❌ o ⚠️? Si todas tus evaluaciones son ✅ en todos los criterios, reconsidera si estás siendo suficientemente crítico. Es muy raro que una respuesta de IA sea perfecta en todos los criterios en el primer intento.

## Solución de Problemas

### Problema 1: No aparece la opción de modo Trabajo (Work) en Copilot Chat

**Síntomas:** Al acceder a https://copilot.microsoft.com, solo se ve el modo Web. No hay un selector visible para cambiar a modo Trabajo. El botón de adjuntar archivos puede estar ausente o deshabilitado.

**Causa:** La cuenta del participante no tiene la licencia de Microsoft 365 Copilot Chat correctamente asignada, o la licencia fue asignada hace menos de 24 horas y aún no se ha propagado. También puede ocurrir si el participante inició sesión con una cuenta personal de Microsoft en lugar de su cuenta corporativa.

**Solución:**
1. Verifica que estás usando tu **cuenta corporativa** (no una cuenta personal como @outlook.com o @hotmail.com). Haz clic en tu avatar/iniciales en la esquina superior derecha y confirma que el correo mostrado es tu correo corporativo.
2. Si estás con la cuenta correcta, cierra sesión completamente de Copilot Chat y del navegador. Borra las cookies del sitio copilot.microsoft.com. Vuelve a iniciar sesión.
3. Si el problema persiste, solicita al instructor que contacte al administrador de TI para verificar que la licencia de Microsoft 365 Copilot Chat está asignada y activa en tu cuenta. El administrador puede verificarlo en el Centro de Administración de Microsoft 365 > Usuarios > [tu cuenta] > Licencias y aplicaciones.
4. Como solución temporal mientras se resuelve el acceso, puedes continuar el laboratorio usando el **modo Web** para los Pasos 2, 3, 5 y 6 (los prompts funcionarán, aunque sin acceso a datos organizacionales). Documenta la incidencia en tu plantilla.

### Problema 2: Copilot Chat genera respuestas genéricas que no se relacionan con mi rol específico

**Síntomas:** Al ejecutar los prompts de los Pasos 2 y 6, Copilot Chat responde con información muy general que podría aplicarse a cualquier profesional. Las sugerencias de tareas no reflejan las particularidades de tu puesto. Las respuestas a prompts de tareas específicas carecen del contexto necesario.

**Causa:** El prompt no incluye suficiente contexto sobre tu rol, industria, tipo de organización o tareas específicas. Los LLM son sensibles al prompt (como se explicó en la Lección 1.1): sin contexto específico, el modelo recurre a patrones genéricos.

**Solución:**
1. Reformula tu prompt incluyendo **más contexto específico**. En lugar de "Soy coordinador de proyectos", escribe "Soy coordinador de proyectos de infraestructura de TI en una empresa de telecomunicaciones con 500 empleados. Mi equipo tiene 8 personas y gestionamos entre 3 y 5 proyectos simultáneos de migración de servidores y redes."
2. Incluye **ejemplos concretos** de lo que esperas. Por ejemplo: "Tareas como las que hago incluyen: crear cronogramas en MS Project, redactar reportes de avance para el PMO, facilitar reuniones de seguimiento semanal con stakeholders técnicos y de negocio."
3. Si la respuesta sigue siendo genérica, usa un **prompt de seguimiento** en la misma conversación: "La respuesta anterior es demasiado general. Necesito sugerencias más específicas para mi contexto. Mi industria es [X], mis principales interlocutores son [Y] y los documentos que más produzco son [Z]."
4. Recuerda que puedes iterar: cada prompt de seguimiento agrega contexto a la ventana de conversación, lo que ayuda al modelo a generar respuestas más relevantes.

## Limpieza

1. **Guarda tu documento final:** Confirma que `LAB01_mapa_oportunidades_[TuNombre]_v1.docx` está guardado en la ubicación indicada por el instructor.
2. **No elimines tu conversación de Copilot Chat:** El historial de esta sesión puede ser útil como referencia en laboratorios posteriores. Si deseas organizarlo, puedes renombrar la conversación como "Lab 01 - Mapa de oportunidades" en el panel de historial.
3. **Cierra pestañas innecesarias:** Si abriste pestañas adicionales durante el laboratorio (por ejemplo, para verificar información), ciérralas para liberar recursos del navegador.
4. **No cierres sesión de Copilot Chat** si vas a continuar con el siguiente laboratorio en la misma sesión de clase.
5. **Conserva la plantilla original:** Mantén una copia sin modificar de `LAB01_plantilla_mapa_oportunidades_v1.docx` por si necesitas consultarla o reiniciar alguna sección.

## Resumen

En este laboratorio completaste las siguientes actividades clave:

- **Exploraste la interfaz** de Microsoft 365 Copilot Chat, identificando el campo de prompt, los modos Web y Trabajo, y la función de adjuntar archivos.
- **Identificaste y clasificaste** al menos siete tareas recurrentes de tu rol profesional según el tipo de soporte que Copilot Chat puede ofrecer (redactar, resumir, transformar, analizar, comparar, idear).
- **Evaluaste el riesgo** de cada tarea en tres dimensiones (privacidad, alucinación, impacto de error) y construiste una **matriz de oportunidades y riesgos** que te permite priorizar dónde usar IA generativa y dónde no.
- **Definiste controles de uso responsable** personalizados para tu rol: qué información no compartir, qué verificar siempre y cuándo no delegar.
- **Ejecutaste tus primeros prompts** en Copilot Chat, evaluaste las respuestas con una lista de verificación de confiabilidad y practicaste la reformulación de prompts para mejorar resultados.
- **Aplicaste el principio central** de la Lección 1.1: la IA generativa amplifica tu capacidad de producir contenido, pero tu criterio profesional es la capa final e indispensable de validación.

### Conexión con el siguiente laboratorio

Tu documento **`LAB01_mapa_oportunidades_[TuNombre]_v1.docx`** será un insumo directo para el **Laboratorio 2**, donde profundizarás en técnicas de prompting (zero-shot, one-shot y few-shot) aplicadas a las tareas que identificaste como prioritarias en tu mapa.

### Recursos adicionales

| Recurso | Enlace | Relevancia |
|---|---|---|
| Introducción a los modelos de lenguaje de gran escala — Microsoft Learn | [https://learn.microsoft.com/es-es/azure/ai-services/openai/concepts/models](https://learn.microsoft.com/es-es/azure/ai-services/openai/concepts/models) | Profundizar en cómo funcionan los LLM |
| Principios de IA responsable — Microsoft | [https://www.microsoft.com/es-es/ai/responsible-ai](https://www.microsoft.com/es-es/ai/responsible-ai) | Marco de referencia para los controles de uso que definiste |
| AI literacy for the workplace — OECD | [https://www.oecd-ilibrary.org/science-and-technology/oecd-artificial-intelligence-papers_49a4c6e8-en](https://www.oecd-ilibrary.org/science-and-technology/oecd-artificial-intelligence-papers_49a4c6e8-en) | Contexto sobre alfabetización en IA para profesionales |
| Generative AI explained — MIT Technology Review | [https://www.technologyreview.com/2023/02/08/1068068/chatgpt-is-everywhere-heres-what-it-cant-do/](https://www.technologyreview.com/2023/02/08/1068068/chatgpt-is-everywhere-heres-what-it-cant-do/) | Perspectiva sobre limitaciones de la IA generativa |

---

# Demo: Demostración guiada: recorrer Copilot Chat, resolver una necesidad de negocio y comparar una interacción segura frente a una riesgosa

## Metadatos

| Campo | Detalle |
|---|---|
| **Duración** | 20 minutos |
| **Complejidad** | Fácil |
| **Nivel de Bloom** | Aplicar |

## Descripción General

En esta demostración en vivo, el instructor recorrerá la interfaz completa de Microsoft 365 Copilot Chat, resolverá una necesidad de negocio concreta mediante un prompt estructurado y comparará lado a lado una interacción segura frente a una riesgosa que incluye datos sensibles ficticios. Los participantes observarán, tomarán notas y, al finalizar, actualizarán su mapa de oportunidades y riesgos iniciado en el Laboratorio 1 con al menos tres buenas prácticas y tres riesgos identificados durante la sesión.

> ℹ️ **Nota:** Esta práctica es una **Demostración realizada por el instructor**. El instructor ejecutará los pasos y comandos mientras los alumnos observan, toman notas y analizan el procedimiento, en lugar de realizarla individualmente.

## Objetivos de Aprendizaje

Al finalizar esta demostración, los participantes serán capaces de:

- [ ] Identificar los elementos funcionales clave de la interfaz de Microsoft 365 Copilot Chat (selector de modo Web/Trabajo, barra de conversación, botón de adjuntar archivo, historial de conversaciones).
- [ ] Describir el proceso completo de resolución de una necesidad de negocio con Copilot Chat: formulación del prompt, obtención de respuesta y evaluación crítica del resultado.
- [ ] Distinguir una interacción segura (sin datos sensibles, con verificación) de una interacción riesgosa (con datos confidenciales, sin validación) y explicar las consecuencias de cada una.
- [ ] Registrar al menos tres buenas prácticas y tres riesgos observados para incorporarlos a su mapa personal del Laboratorio 1.

## Prerrequisitos

### Conocimiento previo

| Requisito | Descripción |
|---|---|
| Laboratorio 1 completado | Los participantes deben haber finalizado el Lab 01-00-01 y tener su archivo `LAB01_plantilla_mapa_oportunidades_v1.docx` abierto o accesible para tomar notas. |
| Conceptos de la Lección 1.1 | Comprensión básica de qué es la IA generativa, sus capacidades (redacción, síntesis, transformación) y sus limitaciones (fecha de corte, alucinaciones, sensibilidad al prompt). |

### Acceso y materiales del instructor

| Elemento | Detalle |
|---|---|
| Cuenta corporativa con licencia | El instructor debe tener una cuenta Microsoft 365 con licencia de Copilot Chat habilitada y verificada al menos 24 horas antes. |
| Escenario de negocio preparado | El instructor debe tener listos los prompts y datos ficticios descritos en esta guía (Acto 1, 2 y 3). |
| Proyector o pantalla compartida | Resolución mínima de 1920×1080, visible para todos los participantes (presencial o remoto). |
| Archivo de ejemplo (opcional) | Un archivo `.docx` de ejemplo de 1-2 páginas con contenido ficticio de negocio para demostrar la función de adjuntar archivos. Nombre sugerido: `DEMO_informe_trimestral_ficticio_v1.docx`. |

### Materiales de los participantes

| Elemento | Detalle |
|---|---|
| `LAB01_plantilla_mapa_oportunidades_v1.docx` | Archivo del Laboratorio 1, abierto y listo para agregar notas. |
| Bloc de notas o editor de texto | Para registrar observaciones durante la demostración. |

## Entorno de Laboratorio

### Equipo del instructor

| Componente | Especificación |
|---|---|
| Navegador | Microsoft Edge 124.0.2478.97 o superior |
| URL de acceso | `https://copilot.microsoft.com` |
| Sistema operativo | Windows 11 22H2 o superior |
| Conexión a Internet | Mínimo 10 Mbps de bajada |
| Pantalla compartida | Proyector o herramienta de videoconferencia con compartir pantalla a 1920×1080 |

### Configuración previa del instructor (antes de la sesión)

1. Abrir Microsoft Edge y navegar a `https://copilot.microsoft.com`.
2. Iniciar sesión con la cuenta corporativa que tiene licencia de Copilot Chat.
3. Verificar que el selector de modo **Trabajo** (Work) está disponible en la interfaz.
4. Cerrar cualquier conversación previa para iniciar con una interfaz limpia (clic en **Nuevo chat**).
5. Tener preparado en el escritorio el archivo `DEMO_informe_trimestral_ficticio_v1.docx` (contenido ficticio, sin datos reales).
6. Tener esta guía de demostración abierta en una pestaña o documento separado como referencia.
7. Verificar que el proyector o la pantalla compartida muestra correctamente la interfaz de Copilot Chat.

### Contenido del archivo de demostración (opcional)

Si el instructor desea demostrar la función de adjuntar archivos, puede crear un documento Word breve con el siguiente contenido ficticio:

#### Ejemplo: `DEMO_informe_trimestral_ficticio_v1.docx`

```
INFORME TRIMESTRAL — Q1 2025
Empresa: Soluciones Globales Ficticia S.A.

RESUMEN EJECUTIVO
El primer trimestre de 2025 cerró con ingresos de $4.2 millones USD,
un incremento del 12% respecto al Q4 2024. El equipo de ventas superó
la meta trimestral en un 8%. Se identificaron tres riesgos operativos
que requieren atención inmediata.

RESULTADOS CLAVE
- Ingresos totales: $4,200,000 USD
- Clientes nuevos: 47
- Tasa de retención: 91%
- NPS (Net Promoter Score): 72

RIESGOS IDENTIFICADOS
1. Retraso en la implementación del módulo de facturación (15 días).
2. Rotación de personal en el equipo de soporte técnico (3 bajas).
3. Dependencia de un solo proveedor de infraestructura cloud.

PRÓXIMOS PASOS
- Reunión de revisión con el equipo de producto: 15 de abril de 2025.
- Plan de mitigación de riesgos: entrega antes del 30 de abril de 2025.
- Kick-off del proyecto de diversificación de proveedores: mayo 2025.
```

## Instrucciones Paso a Paso

> **Nota para el instructor:** Esta demostración se estructura en tres actos secuenciales. Cada acto tiene un objetivo claro y un tiempo sugerido. Hable en voz alta durante todo el proceso: explique qué hace, por qué lo hace y qué deben observar los participantes. Invite a los participantes a tomar notas activamente.

---

### Paso 1: Preparar a los participantes para la observación activa

**Objective:** Establecer el marco de observación para que los participantes sepan exactamente qué buscar durante la demostración y cómo registrar sus aprendizajes.

**Instructions:**

1. Pida a los participantes que abran su archivo `LAB01_plantilla_mapa_oportunidades_v1.docx` o un bloc de notas.
2. Indique que durante la demostración deberán registrar observaciones en dos categorías:
   - **Buenas prácticas** (mínimo 3): acciones del instructor que representan un uso seguro, efectivo o responsable de Copilot Chat.
   - **Riesgos observados** (mínimo 3): situaciones donde la IA podría generar problemas si no se aplica criterio humano.
3. Escriba en la pantalla o pizarrón las dos categorías para que queden visibles durante toda la demostración.
4. Explique brevemente la estructura de la demostración:
   - **Acto 1** (~5 min): Recorrido de la interfaz de Copilot Chat.
   - **Acto 2** (~7 min): Resolución de una necesidad de negocio con un prompt estructurado.
   - **Acto 3** (~5 min): Comparación entre interacción segura e interacción riesgosa.
   - **Cierre** (~3 min): Ronda de preguntas y actualización de mapas.

**Expected output:** Los participantes tienen su documento de notas abierto y comprenden la estructura de la demostración.

**Verification:** Pregunte: *"¿Todos tienen abierto su mapa de oportunidades o un bloc de notas? ¿Alguien tiene alguna duda sobre qué observar?"*. Confirme visualmente que los participantes están listos.

---

### Paso 2: Acto 1 — Recorrido de la interfaz de Copilot Chat

**Objective:** Demostrar cada elemento funcional de la interfaz de Microsoft 365 Copilot Chat para que los participantes puedan identificarlos y comprender su propósito.

**Instructions:**

1. En el navegador del instructor, navegue a `https://copilot.microsoft.com` (debe estar ya autenticado con la cuenta corporativa).
2. **Muestre la pantalla principal** y señale los siguientes elementos mientras los describe en voz alta:

   **a) Selector de modo Web / Trabajo:**
   - Localice el selector de modo en la parte superior de la interfaz.
   - Haga clic en **Web** y explique: *"En modo Web, Copilot Chat utiliza información pública de Internet. No accede a datos del tenant corporativo."*
   - Cambie a **Trabajo** (Work) y explique: *"En modo Trabajo, Copilot Chat puede acceder a datos del tenant de Microsoft 365 de la organización y permite adjuntar archivos. Este es el modo que usaremos en la mayoría de los laboratorios de este curso."*
   - **Punto clave para los participantes:** *"Observen que el modo Trabajo es el que habilita funciones corporativas. Siempre verifiquen en qué modo están antes de escribir un prompt."*

   **b) Barra de conversación (campo de entrada de prompt):**
   - Señale el campo de texto donde se escribe el prompt.
   - Explique: *"Aquí es donde formulamos nuestra instrucción o pregunta. La calidad de lo que escribimos aquí determina la calidad de la respuesta. Esto se llama 'prompting' y lo exploraremos a fondo en lecciones posteriores."*

   **c) Botón de adjuntar archivo (clip o ícono de archivo):**
   - Localice el ícono de adjuntar archivo junto a la barra de conversación.
   - Haga clic en él para mostrar las opciones (subir desde el equipo, seleccionar de OneDrive, etc.).
   - Explique: *"Copilot Chat permite adjuntar archivos de hasta 512 MB. En el Laboratorio 3 trabajaremos extensamente con esta función. Por ahora, solo quiero que sepan dónde está y qué hace."*
   - **Opcional:** Si preparó el archivo `DEMO_informe_trimestral_ficticio_v1.docx`, adjúntelo brevemente para mostrar cómo aparece en la conversación, pero no envíe un prompt todavía.
   - Cancele o cierre el diálogo de adjuntar si no desea usarlo aún.

   **d) Historial de conversaciones (panel lateral):**
   - Muestre el panel lateral izquierdo donde aparecen conversaciones anteriores.
   - Explique: *"Copilot Chat guarda un historial de sus conversaciones. Pueden volver a una conversación previa, pero recuerden que el modelo tiene una ventana de contexto limitada: en conversaciones muy largas puede 'olvidar' instrucciones anteriores, como vimos en la Lección 1.1."*

   **e) Botón de Nuevo chat:**
   - Muestre cómo iniciar una nueva conversación limpia.
   - Explique: *"Es buena práctica iniciar un nuevo chat cuando cambian de tema o tarea. Esto evita que el contexto de una conversación anterior contamine la nueva."*

   **f) Diferencia entre Copilot Chat y Microsoft 365 Copilot completo:**
   - Explique verbalmente: *"Lo que estamos usando es Microsoft 365 Copilot Chat, accesible desde copilot.microsoft.com. Esto es diferente de la licencia completa de Microsoft 365 Copilot, que integra IA directamente dentro de Word, Excel, PowerPoint y Outlook. En este curso nos enfocamos en Copilot Chat."*

3. Haga una pausa breve y pregunte: *"¿Alguien tiene alguna pregunta sobre los elementos de la interfaz que acabamos de ver?"*

**Expected output:** Los participantes pueden ver claramente en la pantalla compartida cada elemento de la interfaz: selector de modo, barra de conversación, botón de adjuntar, historial y botón de nuevo chat.

**Verification:** Pida a los participantes que levanten la mano (o usen la reacción en la herramienta de videoconferencia) si pueden identificar dónde está el selector de modo Web/Trabajo. Confirme que la mayoría responde correctamente.

---

### Paso 3: Acto 2 — Resolución de una necesidad de negocio con Copilot Chat

**Objective:** Demostrar el ciclo completo de uso de Copilot Chat para una tarea de negocio real: formular un prompt estructurado, obtener la respuesta, evaluarla críticamente e identificar qué verificar antes de usar el resultado.

**Instructions:**

1. **Presente el escenario de negocio en voz alta:**

   > *"Imaginen que soy un gerente de operaciones. Acabo de salir de una reunión de revisión trimestral y necesito enviar un resumen ejecutivo al director general en los próximos 30 minutos. Tengo mis notas de la reunión, pero no tengo tiempo de redactar un documento pulido desde cero. Voy a usar Copilot Chat para generar un borrador de resumen ejecutivo."*

2. **Asegúrese de estar en modo Trabajo** (Work) en Copilot Chat. Si no lo está, cámbielo y señale el cambio a los participantes.

3. **Inicie un nuevo chat** haciendo clic en el botón correspondiente.

4. **Escriba el siguiente prompt en la barra de conversación** (léalo en voz alta mientras lo escribe para que los participantes puedan seguirlo):

   ```
   Actúa como un gerente de operaciones que necesita comunicar resultados a la dirección general.

   Con base en las siguientes notas de reunión, genera un resumen ejecutivo profesional de máximo 200 palabras, con tono formal y orientado a resultados. Incluye: logros clave, riesgos identificados y próximos pasos.

   Notas de la reunión:
   - Ingresos Q1 2025: $4.2M USD, +12% vs Q4 2024
   - 47 clientes nuevos captados
   - Tasa de retención: 91%
   - NPS: 72
   - Riesgo: retraso de 15 días en módulo de facturación
   - Riesgo: 3 bajas en equipo de soporte técnico
   - Riesgo: dependencia de un solo proveedor cloud
   - Próxima revisión con equipo de producto: 15 abril 2025
   - Plan de mitigación de riesgos: entrega antes del 30 abril 2025
   ```

5. **Antes de enviar el prompt**, haga una pausa y explique la estructura:

   > *"Observen que este prompt tiene una estructura clara: primero defino el rol ('Actúa como...'), luego la tarea específica ('genera un resumen ejecutivo'), después las restricciones ('máximo 200 palabras, tono formal'), y finalmente proporciono los datos de entrada. Esta estructura mejora significativamente la calidad de la respuesta. Esto se conecta con lo que vimos en la Lección 1.1 sobre la sensibilidad al prompt."*

6. **Envíe el prompt** (presione Enter o haga clic en el botón de enviar).

7. **Espere la respuesta** de Copilot Chat. Mientras se genera, comente:

   > *"Recuerden que el modelo está generando esta respuesta token a token, calculando la continuación más probable. No está 'pensando' como lo haría una persona; está aplicando patrones estadísticos aprendidos durante su entrenamiento."*

8. **Lea la respuesta en voz alta** una vez generada.

9. **Evalúe críticamente la respuesta frente a los participantes.** Haga las siguientes verificaciones en voz alta:

   - **Verificación de datos numéricos:** *"¿Los $4.2M coinciden con lo que le proporcioné? ¿El 12% está correcto? ¿Los 47 clientes nuevos aparecen bien?"* — Confirme que los datos se reflejan correctamente.
   - **Verificación de completitud:** *"¿Incluyó los tres riesgos que mencioné? ¿Están los próximos pasos?"* — Señale si falta algún elemento.
   - **Verificación de invenciones:** *"¿Agregó algún dato que yo NO le proporcioné? Esto es crucial: si el modelo añade información que no estaba en mis notas, eso podría ser una alucinación."* — Si el modelo añadió algo, señálelo explícitamente.
   - **Verificación de tono:** *"¿El tono es realmente formal y orientado a resultados como pedí, o suena demasiado casual o genérico?"*
   - **Verificación de extensión:** *"¿Respetó el límite de 200 palabras aproximadamente?"*

10. **Resuma el ciclo completo para los participantes:**

    > *"Lo que acaban de ver es el ciclo completo: (1) formulé la tarea con un prompt estructurado, (2) Copilot Chat generó una respuesta, y (3) yo revisé, validé y decidí si el resultado es utilizable. Este tercer paso —el criterio humano— es el que marca la diferencia entre usar la IA de forma responsable y usarla a ciegas. Como vimos en la Lección 1.1: la IA amplifica tu capacidad de producir contenido, pero no reemplaza tu responsabilidad sobre ese contenido."*

**Expected output:** Copilot Chat genera un resumen ejecutivo de aproximadamente 150-250 palabras con los datos proporcionados, estructurado en logros clave, riesgos y próximos pasos. La respuesta debe ser coherente y en tono formal.

**Verification:** Pregunte a los participantes: *"¿Alguien detectó algún dato en la respuesta que NO estaba en las notas originales que le proporcioné?"*. Facilite una breve discusión de 30-60 segundos. Si algún participante identifica una adición no solicitada, felicítelo y use el ejemplo para reforzar el concepto de alucinación.

---

### Paso 4: Acto 3 — Comparación entre interacción segura e interacción riesgosa

**Objective:** Demostrar de forma contrastada una interacción que incluye datos sensibles ficticios (riesgosa) y su equivalente segura, para que los participantes identifiquen las diferencias de riesgo y sus consecuencias.

**Instructions:**

1. **Introduzca el acto con una explicación clara:**

   > *"Ahora vamos a ver algo muy importante: la diferencia entre usar Copilot Chat de forma segura y de forma riesgosa. Voy a hacer la misma tarea dos veces. Primero, de forma RIESGOSA —incluyendo datos sensibles ficticios— y luego de forma SEGURA. Quiero que observen las diferencias y piensen en las consecuencias."*

2. **Inicie un nuevo chat** para separar esta interacción de la anterior.

3. **INTERACCIÓN RIESGOSA — Escriba el siguiente prompt** (léalo en voz alta, enfatizando los datos sensibles):

   ```
   Necesito redactar un correo para el cliente Juan Pérez García
   (juan.perez@clientereal.com, tel: +52 55 1234 5678) de la empresa
   Tecnologías Avanzadas S.A. de C.V., informándole que su contrato
   #CT-2025-0892 por $385,000 USD será renovado con un descuento del
   15% porque su cuenta está en riesgo de cancelación. Su ejecutivo
   asignado es María López (ID empleado: EMP-4521). Incluye que el
   margen de utilidad de este contrato es del 42%.
   ```

4. **ANTES de enviar**, haga una pausa dramática y explique:

   > *"ATENCIÓN: No voy a enviar este prompt. Pero quiero que observen lo que contiene."*

5. **Señale cada elemento riesgoso** en el prompt, uno por uno:

   | Dato sensible en el prompt | Tipo de riesgo |
   |---|---|
   | Nombre completo del cliente: Juan Pérez García | Datos personales identificables (PII) |
   | Correo electrónico: juan.perez@clientereal.com | Información de contacto personal |
   | Teléfono: +52 55 1234 5678 | Información de contacto personal |
   | Nombre de empresa real del cliente | Información comercial confidencial |
   | Número de contrato: CT-2025-0892 | Información contractual confidencial |
   | Monto: $385,000 USD | Información financiera confidencial |
   | Descuento del 15% | Estrategia comercial interna |
   | Cuenta en riesgo de cancelación | Información estratégica sensible |
   | ID de empleado: EMP-4521 | Dato interno de recursos humanos |
   | Margen de utilidad: 42% | Información financiera altamente confidencial |

6. **Explique las consecuencias:**

   > *"Si envío este prompt, toda esta información queda registrada en la conversación. Dependiendo de la configuración del tenant y las políticas de retención de datos, estos datos podrían quedar almacenados. Además, estoy exponiendo información que podría violar políticas de privacidad, acuerdos de confidencialidad con el cliente, y regulaciones de protección de datos. El margen de utilidad del 42% es información que muchas empresas consideran secreto comercial."*

7. **Borre el prompt del campo de texto** sin enviarlo.

8. **Inicie un nuevo chat** nuevamente.

9. **INTERACCIÓN SEGURA — Escriba el siguiente prompt** (léalo en voz alta, señalando las diferencias):

   ```
   Actúa como un ejecutivo de cuentas corporativas.

   Redacta un correo profesional para un cliente cuyo contrato de
   servicios está próximo a renovarse. El tono debe ser cordial y
   orientado a la retención. El correo debe:
   - Agradecer la relación comercial
   - Informar sobre la próxima renovación del contrato
   - Mencionar que se ha preparado una propuesta con condiciones
     preferenciales como reconocimiento a su lealtad
   - Invitar al cliente a una reunión para revisar la propuesta
   - Tener un máximo de 150 palabras

   No incluyas nombres, montos ni datos específicos; yo los agregaré
   después manualmente.
   ```

10. **Envíe el prompt** y espere la respuesta.

11. **Lea la respuesta en voz alta** y señale las diferencias clave:

    > *"Observen: obtuve un correo profesional, bien estructurado y listo para personalizar. Pero no expuse NINGÚN dato sensible. Ahora yo puedo tomar esta plantilla, copiarla a mi correo electrónico, y agregar manualmente el nombre del cliente, el número de contrato y los detalles específicos en un entorno seguro. El resultado final es el mismo —un correo profesional— pero el proceso fue completamente seguro."*

12. **Resuma los principios de la comparación:**

    > *"Las tres reglas que acabamos de aplicar son:*
    > 1. *Nunca incluir datos personales identificables (nombres reales, correos, teléfonos) en un prompt.*
    > 2. *Nunca incluir información financiera confidencial (montos, márgenes, descuentos específicos) en un prompt.*
    > 3. *Usar Copilot Chat para generar la estructura y el lenguaje, y agregar los datos sensibles manualmente después, fuera de la herramienta.*
    >
    > *Y una cuarta regla transversal: siempre revisar la respuesta antes de usarla. En el Acto 2 vimos cómo verificar datos. Aquí vemos cómo proteger datos. Ambas son caras de la misma moneda: el criterio humano."*

**Expected output:** Copilot Chat genera un correo de plantilla profesional, cordial y orientado a retención, sin datos específicos de clientes, montos ni información confidencial. El correo debe tener espacios o marcadores implícitos donde el usuario puede insertar datos manualmente.

**Verification:** Pregunte a los participantes: *"¿Cuántos datos sensibles identificaron en el prompt riesgoso?"*. La respuesta correcta es al menos 8-10 elementos. Pida a 2-3 participantes que mencionen ejemplos específicos. Confirme que comprenden por qué cada uno representa un riesgo.

---

### Paso 5: Cierre — Ronda de preguntas y actualización de mapas

**Objective:** Consolidar los aprendizajes de la demostración mediante una ronda de preguntas y la actualización formal del mapa de oportunidades y riesgos del Laboratorio 1.

**Instructions:**

1. **Facilite una ronda de preguntas** (2-3 minutos):
   - Pregunte: *"¿Qué les llamó más la atención de lo que vimos?"*
   - Pregunte: *"¿Alguien pensó en una situación de su propio trabajo donde podría aplicar lo que vimos en el Acto 2?"*
   - Pregunte: *"¿Alguien pensó en una situación de su propio trabajo donde podría cometer el error que vimos en el Acto 3?"*
   - Responda las preguntas de los participantes de forma breve y concreta.

2. **Pida a los participantes que actualicen su mapa** del Laboratorio 1 (`LAB01_plantilla_mapa_oportunidades_v1.docx`). Dé 2 minutos para que registren:

   **Buenas prácticas observadas (mínimo 3):**
   - Ejemplo: Verificar en qué modo (Web/Trabajo) se encuentra Copilot Chat antes de escribir un prompt.
   - Ejemplo: Estructurar el prompt con rol, tarea, restricciones y datos de entrada.
   - Ejemplo: Revisar la respuesta verificando datos numéricos, completitud, invenciones y tono antes de usarla.
   - Ejemplo: Usar Copilot Chat para generar plantillas genéricas y agregar datos sensibles manualmente después.
   - Ejemplo: Iniciar un nuevo chat al cambiar de tema o tarea.

   **Riesgos observados (mínimo 3):**
   - Ejemplo: Incluir datos personales (nombres, correos, teléfonos) en los prompts.
   - Ejemplo: Compartir información financiera confidencial (montos, márgenes) con la herramienta.
   - Ejemplo: Usar la respuesta de Copilot Chat sin verificar si agregó datos que no estaban en la entrada original (alucinaciones).
   - Ejemplo: No verificar datos numéricos antes de incluirlos en comunicaciones oficiales.
   - Ejemplo: Confiar en que el modelo "entiende" el contexto cuando en realidad opera por patrones probabilísticos.

3. **Cierre la demostración** con un mensaje de transición:

   > *"Lo que acabamos de ver resume los tres pilares de este curso: conocer la herramienta, usarla de forma efectiva y usarla de forma responsable. En los próximos laboratorios, ustedes serán quienes operen Copilot Chat directamente. Lo que aprendieron hoy observando será la base para hacerlo con confianza y criterio."*

**Expected output:** Los participantes tienen su mapa del Laboratorio 1 actualizado con al menos 3 buenas prácticas y 3 riesgos derivados de la demostración.

**Verification:** Pida a 2-3 voluntarios que compartan en voz alta una buena práctica y un riesgo que registraron. Confirme que las respuestas reflejan lo observado durante la demostración y no son genéricas.

## Validación y Pruebas

Al finalizar la demostración, el instructor debe confirmar que se cumplieron los siguientes criterios de éxito:

| Criterio | Método de verificación | Resultado esperado |
|---|---|---|
| Los participantes identifican los elementos de la interfaz | Pregunta rápida: *"¿Dónde se cambia entre modo Web y Trabajo?"* | Al menos el 80% de los participantes puede señalar o describir la ubicación correcta. |
| Los participantes comprenden el ciclo prompt → respuesta → validación | Pregunta: *"¿Cuáles son los tres pasos que vimos para resolver una tarea de negocio?"* | Los participantes mencionan: formular el prompt, obtener la respuesta, y revisar/validar antes de usar. |
| Los participantes distinguen interacción segura de riesgosa | Pregunta: *"¿Cuál es la diferencia principal entre los dos prompts del Acto 3?"* | Los participantes mencionan que el prompt riesgoso contenía datos personales y confidenciales, mientras que el seguro usaba una plantilla genérica. |
| Los mapas del Laboratorio 1 fueron actualizados | Verificación visual o pregunta: *"¿Quién ya registró al menos 3 prácticas y 3 riesgos?"* | Al menos el 90% de los participantes confirma haber actualizado su mapa. |

## Solución de Problemas

### Problema 1: El modo Trabajo (Work) no aparece disponible en Copilot Chat del instructor

**Síntomas:** Al abrir `https://copilot.microsoft.com`, el selector de modo solo muestra "Web" o no aparece la opción "Trabajo". La interfaz se comporta como la versión gratuita de Copilot.

**Causa:** La cuenta del instructor no tiene asignada la licencia de Microsoft 365 Copilot Chat, la licencia fue asignada hace menos de 24 horas y aún no se ha propagado, o el instructor inició sesión con una cuenta personal en lugar de la cuenta corporativa.

**Solución:**
1. Verifique que la URL sea exactamente `https://copilot.microsoft.com` (no `copilot.microsoft.com` sin HTTPS ni una URL diferente como `bing.com/chat`).
2. Haga clic en el ícono de perfil en la esquina superior derecha y confirme que la cuenta mostrada es la cuenta corporativa (dominio de la organización, no @outlook.com o @hotmail.com).
3. Si la cuenta es correcta pero el modo Trabajo no aparece, cierre todas las pestañas del navegador, borre la caché del navegador (`Ctrl+Shift+Delete` → seleccionar "Cookies" e "Imágenes en caché" → Borrar), y vuelva a iniciar sesión.
4. Si persiste, contacte al administrador de TI para confirmar que la licencia está activa. Como plan de contingencia, el instructor puede realizar la demostración solo en modo Web, explicando verbalmente las diferencias con el modo Trabajo y mostrando capturas de pantalla previamente preparadas del modo Trabajo.

### Problema 2: Copilot Chat genera una respuesta en inglés en lugar de español

**Síntomas:** A pesar de que el prompt fue escrito en español, Copilot Chat responde parcial o totalmente en inglés, o mezcla ambos idiomas en la respuesta.

**Causa:** La configuración de idioma del navegador o de la cuenta de Microsoft 365 del instructor está establecida en inglés. Copilot Chat a veces toma señales del idioma del sistema además del idioma del prompt.

**Solución:**
1. **Solución inmediata en el prompt:** Agregue al inicio del prompt la instrucción explícita: `Responde completamente en español.` Esto suele corregir el problema en la mayoría de los casos.
2. **Solución en el navegador:** En Microsoft Edge, vaya a `edge://settings/languages` y asegúrese de que "Español" esté como primer idioma de la lista. Reinicie el navegador.
3. **Solución en Microsoft 365:** Navegue a `https://myaccount.microsoft.com/settingsandprivacy/language` y configure el idioma de visualización a "Español (España)" o "Español (México)".
4. Si ninguna de las soluciones anteriores funciona de inmediato, el instructor puede continuar la demostración añadiendo `Responde en español.` al final de cada prompt y explicar a los participantes que esta es una práctica recomendada cuando el idioma de respuesta no coincide con el esperado.

## Limpieza

Dado que esta es una demostración del instructor y los participantes no ejecutaron acciones en sus propios equipos, la limpieza es mínima:

1. **Instructor:** Elimine las conversaciones de demostración del historial de Copilot Chat para evitar confusión en futuras sesiones:
   - En el panel lateral izquierdo, localice las conversaciones creadas durante la demostración.
   - Haga clic en los tres puntos (⋯) junto a cada conversación y seleccione **Eliminar**.
   - Confirme la eliminación.

2. **Instructor:** Si subió el archivo `DEMO_informe_trimestral_ficticio_v1.docx` durante la demostración, no es necesario eliminarlo ya que contiene solo datos ficticios. Sin embargo, si desea mantener el entorno limpio, puede eliminarlo de la ubicación de carga.

3. **Participantes:** No requieren limpieza. Deben conservar su archivo `LAB01_plantilla_mapa_oportunidades_v1.docx` actualizado, ya que lo seguirán utilizando en laboratorios posteriores.

## Resumen

En esta demostración se cubrieron los tres pilares fundamentales del uso profesional de Microsoft 365 Copilot Chat:

| Acto | Pilar | Aprendizaje clave |
|---|---|---|
| **Acto 1: Recorrido de interfaz** | Conocer la herramienta | Identificar el selector de modo Web/Trabajo, la barra de conversación, el botón de adjuntar archivos, el historial y el botón de nuevo chat. El modo Trabajo es el requerido para funciones corporativas. |
| **Acto 2: Resolución de necesidad de negocio** | Usar la herramienta de forma efectiva | Un prompt estructurado (rol + tarea + restricciones + datos) produce mejores resultados. Toda respuesta debe verificarse antes de usarse: datos numéricos, completitud, invenciones y tono. |
| **Acto 3: Comparación seguro vs. riesgoso** | Usar la herramienta de forma responsable | Nunca incluir datos personales, financieros o confidenciales en los prompts. Usar Copilot Chat para generar plantillas genéricas y agregar datos sensibles manualmente después. |

**Conexión con la Lección 1.1:** Esta demostración aplicó en la práctica los conceptos teóricos de la lección: las capacidades de la IA generativa (redacción, síntesis), sus limitaciones (posibles alucinaciones, sensibilidad al prompt) y la necesidad indispensable del criterio humano como capa final de validación.

### Recursos adicionales

- [Guía de uso responsable de Microsoft 365 Copilot — Microsoft Learn](https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-privacy)
- [Mejores prácticas de prompting para Copilot — Microsoft Adoption](https://adoption.microsoft.com/es-es/copilot/)
- [Principios de IA responsable — Microsoft](https://www.microsoft.com/es-es/ai/responsible-ai)

---
