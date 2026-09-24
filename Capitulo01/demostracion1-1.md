# Demostración guiada 1.1. Primera conversación controlada: recorrer Microsoft 365 Copilot Chat (Licenciamiento Básico), formular una necesidad de negocio, probar una respuesta y marcar qué partes requieren verificación.

## Metadatos

| Campo | Detalle |
|---|---|
| Duración | 32 minutos |
| Complejidad | Fácil |
| Nivel Bloom | Comprender |
| Plataforma | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Modalidad | Demostración guiada por el instructor |

## Descripción General

En esta demostración observarás un flujo de trabajo completo en Microsoft 365 Copilot Chat. El instructor ejecutará el procedimiento mientras tú analizas las decisiones, registras evidencias y extraes un patrón que podrás reutilizar posteriormente.



## Objetivos de Aprendizaje

Al completar esta actividad serás capaz de:

- [ ] Reconocer y aplicar el procedimiento central de la actividad.
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
- Comprender los contenidos previos requeridos para esta actividad: Conceptos de IA generativa, capacidades y límites de Copilot Chat, alucinaciones, privacidad y uso responsable.
- No se requieren conocimientos de programación, APIs, administración de Microsoft 365 ni construcción de agentes.

### Acceso y recursos

| Elemento | Requisito para esta actividad |
|---|---|
| Cuenta de usuario | Cuenta corporativa habilitada para **Microsoft 365 Copilot Chat (Licenciamiento Básico)**. No se requiere licencia Microsoft 365 Copilot Premium. |
| Acceso | Poder iniciar sesión en el portal de Microsoft 365/Copilot autorizado por la organización. |
| Navegador | Microsoft Edge o Google Chrome en una versión vigente y con JavaScript y cookies habilitados para los servicios de Microsoft 365. |
| Conectividad | Acceso estable a Internet y a los dominios de Microsoft 365 permitidos por la organización. |
| Material de actividad | Hoja o documento para registrar oportunidades, riesgos, observaciones y evidencias. |
| Datos | Utiliza exclusivamente información ficticia, anonimizada, pública o expresamente autorizada para capacitación. |
| Evidencias | Conserva los prompts, respuestas, observaciones y validaciones solicitadas en cada paso. |

Durante la demostración no necesitas ejecutar los prompts al mismo tiempo que el instructor; debes observar, comparar resultados y registrar los hallazgos solicitados.

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

### Paso 1: Prepararte para la observación activa

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Abre un bloc de notas o el documento indicado por el instructor.
2. Crea tres apartados: Información proporcionada, Contenido generado y Elementos por verificar.
3. Durante la demostración registra al menos una observación en cada apartado.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 4 minutos

---

### Paso 2: Observar el recorrido inicial de Copilot Chat

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Identifica el área donde se escribe la solicitud, el historial y las opciones disponibles en la cuenta usada por el instructor.
2. Anota qué elementos de la interfaz son relevantes para iniciar una conversación controlada.
3. Observa cómo el instructor confirma que está trabajando en el entorno correcto antes de escribir información.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 5 minutos

---

### Paso 3: Observar cómo se formula la necesidad de negocio

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Identifica el objetivo de la solicitud, la audiencia y el resultado esperado.
2. Anota qué información aporta el instructor y qué información todavía falta.
3. Observa si Copilot solicita aclaraciones o si el instructor debe agregarlas de forma explícita.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 6 minutos

---

### Paso 4: Analizar la primera respuesta

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Distingue hechos proporcionados por el instructor de contenido generado por Copilot.
2. Marca cifras, nombres, fechas, afirmaciones o recomendaciones que requerirían verificación.
3. Anota al menos un supuesto que aparezca en la respuesta.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 6 minutos

---

### Paso 5: Observar el refinamiento y la verificación

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Compara el primer prompt con el prompt de seguimiento.
2. Identifica qué cambió: contexto, restricciones, formato, audiencia o nivel de detalle.
3. Observa cómo el instructor corrige o elimina elementos que no estén sustentados.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 7 minutos

---

### Paso 6: Registrar el patrón de trabajo

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Resume en una frase qué hizo más confiable la segunda respuesta.
2. Escribe una regla personal que aplicarás antes de utilizar una respuesta de Copilot en tu trabajo.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 4 minutos

## Prompt de referencia

```text
Necesito preparar un mensaje breve para informar a mi equipo sobre un cambio operativo.
Antes de redactarlo, identifica qué información te falta.
Después separa tu respuesta en: 1) hechos que proporcioné, 2) supuestos que realizaste y 3) elementos que debo verificar.
```

> Sustituye los campos de ejemplo únicamente con información ficticia, anonimizada o autorizada cuando reutilices este patrón.

## Resultado esperado

Al finalizar la demostración tendrás notas suficientes para describir el procedimiento observado, identificar buenas prácticas, reconocer riesgos y explicar qué elementos requieren criterio o verificación humana.

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
