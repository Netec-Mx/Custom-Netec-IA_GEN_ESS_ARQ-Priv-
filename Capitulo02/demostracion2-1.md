# Demostración guiada 2.1. Anatomía del prompt: convertir solicitudes vagas en prompts estructurados y comparar cómo cambia la calidad, precisión y formato de la respuesta

## Metadatos

| Campo | Detalle |
|---|---|
| Duración | 35 minutos |
| Complejidad | Media |
| Nivel Bloom | Analizar |
| Plataforma | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Modalidad | Demostración guiada por el instructor |

## Descripción General

En esta demostración observarás un flujo de trabajo completo en Microsoft 365 Copilot Chat. El instructor ejecutará el procedimiento mientras tú analizas las decisiones, registras evidencias y extraes un patrón que podrás reutilizar posteriormente.

> ℹ️ **Nota:** Esta actividad es una demostración realizada por el instructor. El instructor ejecutará los pasos en pantalla mientras tú observas, tomas notas y analizas el procedimiento. No necesitas reproducir cada acción durante la demostración.

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
- Comprender los contenidos previos requeridos para esta actividad: Conceptos del capítulo 1 y fundamentos de prompting: objetivo, contexto, expectativas, fuente, formato, restricciones y tono.
- No se requieren conocimientos de programación, APIs, administración de Microsoft 365 ni construcción de agentes.

### Acceso y recursos

| Elemento | Requisito para esta actividad |
|---|---|
| Cuenta de usuario | Cuenta corporativa habilitada para **Microsoft 365 Copilot Chat (Licenciamiento Básico)**. No se requiere licencia Microsoft 365 Copilot Premium. |
| Acceso | Poder iniciar sesión en el portal de Microsoft 365/Copilot autorizado por la organización. |
| Navegador | Microsoft Edge o Google Chrome en una versión vigente y con JavaScript y cookies habilitados para los servicios de Microsoft 365. |
| Conectividad | Acceso estable a Internet y a los dominios de Microsoft 365 permitidos por la organización. |
| Material de actividad | Hoja o documento para registrar versiones de prompts, resultados y comparaciones. |
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

### Paso 1: Identificar una solicitud vaga

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Lee la solicitud inicial mostrada por el instructor.
2. Anota qué elementos faltan para comprender exactamente qué se necesita.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 5 minutos

---

### Paso 2: Separar los componentes del prompt

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Identifica objetivo, contexto, expectativas y fuente.
2. Observa cómo pueden agregarse rol, formato, restricciones y tono cuando aportan claridad.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 7 minutos

---

### Paso 3: Comparar la primera y segunda respuesta

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Revisa la respuesta obtenida con la solicitud vaga.
2. Compárala con la respuesta producida por el prompt estructurado.
3. Anota tres diferencias observables en precisión, utilidad o formato.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 8 minutos

---

### Paso 4: Detectar sobre-especificación y ambigüedad

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Observa un ejemplo con información insuficiente y otro con instrucciones innecesariamente extensas.
2. Identifica qué información aporta valor y cuál solo agrega ruido.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 6 minutos

---

### Paso 5: Construir una lista de comprobación

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Registra las preguntas que debes hacerte antes de enviar un prompt: qué quiero, para quién, con qué contexto, con qué fuente y en qué formato.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 5 minutos

---

### Paso 6: Cerrar con un patrón reutilizable

**Objetivo:** Observar y analizar este momento de la demostración.

**Instrucciones:**

1. Escribe una plantilla breve de prompt que puedas adaptar a tareas de tu trabajo.

**Resultado esperado:** Tendrás notas concretas que te permitan explicar qué hizo el instructor, qué resultado obtuvo y qué debe verificarse.

**Verificación:** Confirma que registraste al menos una observación concreta antes de continuar.

> ⏱ **Tiempo estimado:** 4 minutos

## Prompt de referencia

```text
Objetivo: [qué necesito lograr].
Contexto: [situación necesaria para comprender la tarea].
Fuente: [información o archivo que debe utilizarse].
Formato esperado: [tabla, lista, correo, resumen, etc.].
Restricciones: [qué no debe inventar, longitud, tono o límites].
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
