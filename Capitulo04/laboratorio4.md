# Laboratorio 4. Reto integrador por rol: resolver una tarea real de principio a fin, refinar el prompt, validar fuentes y contenido, aplicar controles de privacidad y guardar el patrón final en una biblioteca personal

## Metadatos

| Campo | Detalle |
|---|---|
| Duración | 71 minutos |
| Complejidad | Alta |
| Nivel Bloom | Crear |
| Plataforma | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Modalidad | Laboratorio práctico individual |

## Descripción General

En este laboratorio trabajarás directamente en Microsoft 365 Copilot Chat para resolver una situación cercana a tu trabajo. Utilizarás únicamente información ficticia, anonimizada o autorizada y documentarás tanto el resultado como los controles de verificación aplicados.

## Objetivos de Aprendizaje

Al completar esta actividad serás capaz de:

- [ ] Aplicar un procedimiento completo de trabajo con Copilot Chat a una situación de negocio.
- [ ] Distinguir información sustentada, supuestos y elementos que requieren verificación.
- [ ] Aplicar criterios de privacidad, seguridad y revisión humana antes de utilizar una salida.
- [ ] Conservar un patrón reutilizable para futuras tareas de productividad.

## Prerrequisitos

### Conocimientos previos

Antes de iniciar, debes poder:

- Reconocer qué es una instrucción o prompt y distinguirla de la respuesta generada por Copilot.
- Identificar que una respuesta generada por IA puede contener errores, omisiones o información no sustentada y que requiere revisión humana.
- Aplicar la regla del curso de no compartir información confidencial, credenciales, datos personales de terceros ni información restringida.
- Manejar funciones básicas de un navegador: abrir una pestaña, iniciar sesión, copiar y pegar texto y descargar o seleccionar un archivo cuando corresponda.
- Comprender los contenidos previos requeridos para esta actividad: Uso productivo de Copilot Chat, verificación de respuestas, evaluación de fuentes, privacidad, prompt injection y criterio humano.
- No se requieren conocimientos de programación, APIs, administración de Microsoft 365 ni construcción de agentes.

### Acceso y recursos

| Elemento | Requisito para esta actividad |
|---|---|
| Cuenta de usuario | Cuenta corporativa habilitada para **Microsoft 365 Copilot Chat (Licenciamiento Básico)**. No se requiere licencia Microsoft 365 Copilot Premium. |
| Acceso | Poder iniciar sesión en el portal de Microsoft 365/Copilot autorizado por la organización. |
| Navegador | Microsoft Edge o Google Chrome en una versión vigente y con JavaScript y cookies habilitados para los servicios de Microsoft 365. |
| Conectividad | Acceso estable a Internet y a los dominios de Microsoft 365 permitidos por la organización. |
| Material de actividad | Hoja o documento para registrar hallazgos, controles, versión final del prompt y aprendizajes. |
| Datos | Utiliza exclusivamente información ficticia, anonimizada, pública o expresamente autorizada para capacitación. |
| Evidencias | Conserva los prompts, respuestas, observaciones y validaciones solicitadas en cada paso. |

Debes disponer de acceso individual a Copilot Chat para ejecutar los prompts y completar las evidencias del laboratorio.

> **Antes de continuar:** si no puedes abrir Copilot Chat, iniciar una conversación nueva o utilizar el recurso indicado, informa al instructor antes de comenzar la actividad.

## Entorno de Laboratorio

### Hardware requerido

| Componente | Requisito | Motivo |
|---|---|---|
| Equipo | PC o laptop con Windows 10/11, macOS o sistema compatible con un navegador moderno | La actividad se realiza desde la interfaz web; no requiere una estación de trabajo especializada. |
| Procesador y memoria | Capacidad suficiente para ejecutar de forma fluida el navegador y una aplicación adicional para notas/documentos | No se ejecutan modelos de IA localmente. |
| Pantalla | Resolución recomendada de **1280 × 768 o superior** | Permite visualizar simultáneamente la conversación y las instrucciones del laboratorio. |
| Teclado y mouse/touchpad | Funcionales | Necesarios para redactar, editar y comparar prompts y respuestas. |
| Conexión de red | Internet estable | Copilot Chat funciona como servicio en línea. |
| Audio | No requerido | Ninguna tarea depende de entrada o salida de audio. |

> **Nota:** no se requiere GPU dedicada, máquina virtual, servidor, teléfono móvil ni infraestructura local adicional.

### Software requerido

| Software/servicio | Requisito | Uso durante la actividad |
|---|---|---|
| Microsoft 365 Copilot Chat | **Licenciamiento Básico** y sesión corporativa habilitada | Ejecutar o visualizar los prompts y respuestas de la actividad. |
| Microsoft Edge o Google Chrome | Versión vigente | Acceder a Copilot Chat y trabajar con la interfaz web. |
| Aplicación para evidencias | Bloc de notas, Word u otra aplicación autorizada por el instructor | Registrar prompts, respuestas, comparaciones, riesgos y conclusiones. |
| Visor/aplicación de archivos | Solo cuando el ejercicio incluya un archivo de práctica | Abrir la fuente original y contrastarla con la respuesta de Copilot. |

No instales extensiones, complementos, herramientas de terceros ni software adicional para completar esta actividad. No se utilizan Power Automate, Copilot Studio, APIs ni código.

### Configuración inicial

1. Inicia el equipo y confirma que tienes conexión a Internet.
2. Abre **Microsoft Edge** o **Google Chrome**.
3. Inicia sesión únicamente con la **cuenta corporativa asignada o autorizada para el curso**.
4. Accede a **Microsoft 365 Copilot Chat** desde el portal autorizado por tu organización.
5. Confirma que la sesión corresponde a la cuenta correcta antes de introducir cualquier información.
6. Inicia una **conversación nueva** para evitar que mensajes de actividades anteriores influyan en los resultados.
7. Comprueba que puedes escribir un mensaje en el cuadro de conversación. No envíes todavía información real de negocio.
8. Abre la aplicación que utilizarás para registrar evidencias y crea un documento nuevo con el nombre de la actividad.
9. Si la actividad utiliza un archivo proporcionado por el instructor, guárdalo en una ubicación conocida y **ábrelo primero para comprobar que es el archivo correcto**. No cargues archivos personales ni corporativos distintos de los autorizados para la práctica.
10. Prepara dos áreas de trabajo: una con estas instrucciones y otra con Copilot Chat. Puedes utilizar ventanas lado a lado o pestañas independientes.
11. Antes de comenzar, verifica este control:
   - [ ] Puedo acceder a Copilot Chat.
   - [ ] Estoy utilizando la cuenta autorizada.
   - [ ] Puedo iniciar una conversación nueva.
   - [ ] Tengo abierto el documento para registrar evidencias.
   - [ ] Tengo disponible el archivo de práctica, si esta actividad lo requiere.
   - [ ] No utilizaré datos sensibles, credenciales ni información restringida.

> ⚠️ **Importante:** si un prompt de ejemplo contiene nombres, cifras, clientes, empleados u otros datos, trátalos como datos ficticios de capacitación. No los sustituyas por información confidencial de tu organización.

## Instrucciones Paso a Paso

---

### Paso 1: Seleccionar y delimitar el reto

**Objetivo:** Completar esta etapa del laboratorio y conservar evidencia de tu trabajo.

**Instrucciones:**

1. Elige una tarea real de tu rol que sea de bajo o medio riesgo.
2. Representa cualquier dato sensible con información ficticia o anonimizada.
3. Define objetivo, audiencia, fuente disponible y resultado esperado.

**Resultado esperado:** Tendrás un resultado documentado que podrás utilizar en el siguiente paso y validar al finalizar el laboratorio.

**Verificación:** Confirma que completaste todos los puntos del paso y que puedes explicar por qué el resultado es válido.

> ⏱ **Tiempo estimado:** 10 minutos

---

### Paso 2: Diseñar el prompt inicial

**Objetivo:** Completar esta etapa del laboratorio y conservar evidencia de tu trabajo.

**Instrucciones:**

1. Construye el prompt con objetivo, contexto, expectativas, fuente, formato y restricciones.
2. Incluye una instrucción para no inventar información y señalar ausencias.

**Resultado esperado:** Tendrás un resultado documentado que podrás utilizar en el siguiente paso y validar al finalizar el laboratorio.

**Verificación:** Confirma que completaste todos los puntos del paso y que puedes explicar por qué el resultado es válido.

> ⏱ **Tiempo estimado:** 12 minutos

---

### Paso 3: Ejecutar y evaluar críticamente

**Objetivo:** Completar esta etapa del laboratorio y conservar evidencia de tu trabajo.

**Instrucciones:**

1. Ejecuta el prompt.
2. Clasifica el contenido en sustentado, inferido y por verificar.
3. Identifica al menos una oportunidad de mejora.

**Resultado esperado:** Tendrás un resultado documentado que podrás utilizar en el siguiente paso y validar al finalizar el laboratorio.

**Verificación:** Confirma que completaste todos los puntos del paso y que puedes explicar por qué el resultado es válido.

> ⏱ **Tiempo estimado:** 12 minutos

---

### Paso 4: Refinar y volver a probar

**Objetivo:** Completar esta etapa del laboratorio y conservar evidencia de tu trabajo.

**Instrucciones:**

1. Ajusta el prompt para corregir las debilidades detectadas.
2. Si aplica, incorpora ejemplo, tono, formato o restricción adicional.
3. Compara ambas versiones.

**Resultado esperado:** Tendrás un resultado documentado que podrás utilizar en el siguiente paso y validar al finalizar el laboratorio.

**Verificación:** Confirma que completaste todos los puntos del paso y que puedes explicar por qué el resultado es válido.

> ⏱ **Tiempo estimado:** 12 minutos

---

### Paso 5: Validar fuentes, privacidad y uso final

**Objetivo:** Completar esta etapa del laboratorio y conservar evidencia de tu trabajo.

**Instrucciones:**

1. Comprueba los hechos relevantes contra la fuente original.
2. Confirma que no se expusieron datos restringidos.
3. Decide qué partes son utilizables, cuáles debes editar y cuáles debes descartar.

**Resultado esperado:** Tendrás un resultado documentado que podrás utilizar en el siguiente paso y validar al finalizar el laboratorio.

**Verificación:** Confirma que completaste todos los puntos del paso y que puedes explicar por qué el resultado es válido.

> ⏱ **Tiempo estimado:** 12 minutos

---

### Paso 6: Guardar el patrón en tu biblioteca personal

**Objetivo:** Completar esta etapa del laboratorio y conservar evidencia de tu trabajo.

**Instrucciones:**

1. Documenta nombre del prompt, propósito, entradas, variables, restricciones, formato de salida y lista de verificación.
2. Agrega una nota que indique cuándo NO debes reutilizar el patrón.
3. Guarda la versión final en el formato indicado por el instructor.

**Resultado esperado:** Tendrás un resultado documentado que podrás utilizar en el siguiente paso y validar al finalizar el laboratorio.

**Verificación:** Confirma que completaste todos los puntos del paso y que puedes explicar por qué el resultado es válido.

> ⏱ **Tiempo estimado:** 13 minutos

## Prompt de referencia

```text
Analiza esta propuesta de forma crítica sin tomar la decisión por mí.
Identifica supuestos, puntos ciegos, contraargumentos, evidencia faltante y riesgos.
Convierte cada observación en una pregunta o acción de validación.
```

> Sustituye los campos de ejemplo únicamente con información ficticia, anonimizada o autorizada cuando reutilices este patrón.

## Resultado esperado

Al finalizar el laboratorio tendrás un resultado útil y verificable, acompañado de los prompts utilizados, las decisiones de refinamiento y una evidencia clara de los controles de privacidad y validación aplicados.

## Verificación Final

- [ ] Puedo explicar el objetivo de la actividad y el flujo seguido.
- [ ] Distinguí hechos sustentados, supuestos y elementos por verificar.
- [ ] No utilicé datos sensibles, confidenciales o no autorizados.
- [ ] Verifiqué los elementos relevantes antes de considerar utilizable la salida.
- [ ] Conservé al menos un patrón, prompt o criterio reutilizable.

## Solución de problemas

### Copilot responde de forma demasiado general

**Síntomas:** La respuesta podría aplicarse a cualquier persona o situación y no refleja el contexto esperado.

**Causa probable:** El prompt no contiene suficiente objetivo, contexto, audiencia o formato de salida.

**Solución:**
1. Agrega únicamente el contexto necesario para comprender la tarea.
2. Especifica la audiencia y el formato esperado.
3. Añade restricciones claras, por ejemplo: "No inventes datos" o "Indica No disponible si la fuente no contiene la respuesta".
4. No agregues información sensible solo para hacer la respuesta más específica.

### Copilot presenta información que no puedes comprobar

**Síntomas:** Aparecen cifras, fechas, nombres, causas o conclusiones que no estaban en la información proporcionada.

**Solución:**
1. Detén el uso de esa parte de la respuesta.
2. Contrasta el dato contra la fuente original o una fuente autorizada.
3. Reformula el prompt para limitar la respuesta a la información disponible.
4. Si no existe evidencia, conserva el elemento como "No verificado" o elimínalo del resultado final.

### No aparece una función esperada en Copilot Chat

**Solución:**
1. Confirma que utilizas la cuenta indicada para el curso.
2. Actualiza la página y vuelve a comprobar la interfaz.
3. Informa al instructor si la función continúa sin aparecer.
4. No cambies a servicios o cuentas no autorizadas para completar el ejercicio.

## Limpieza

1. Guarda únicamente los archivos y notas que el instructor indique conservar.
2. Cierra documentos de práctica que ya no necesites.
3. No conserves copias locales de información sensible o no autorizada.
4. Si continuarás con la siguiente actividad en la misma sesión, mantén abierta la cuenta y los recursos que indique el instructor.

## Resumen

En esta actividad trabajaste con un patrón de uso controlado de Microsoft 365 Copilot Chat. El objetivo no es aceptar automáticamente una respuesta, sino formular una necesidad con claridad, revisar la salida, comprobar su evidencia y decidir conscientemente qué puede utilizarse.

### Conexión con la siguiente actividad

Conserva tus notas y prompts. Las actividades posteriores reutilizan progresivamente los criterios de claridad, contexto, formato, evidencia, privacidad y revisión humana.

### Recursos adicionales

| Recurso | Enlace | Relevancia |
|---|---|---|
| Microsoft 365 Copilot | https://www.microsoft.com/microsoft-365/copilot | Información general del producto |
| Microsoft Learn | https://learn.microsoft.com/ | Documentación y aprendizaje oficial |
| IA responsable de Microsoft | https://www.microsoft.com/ai/responsible-ai | Principios de uso responsable |
