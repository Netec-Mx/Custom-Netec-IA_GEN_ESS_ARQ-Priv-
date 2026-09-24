# Laboratorio 2. Clínica de prompts: construir, probar y refinar un conjunto de prompts reutilizables para situaciones reales del trabajo, incorporando criterios de calidad y verificación

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 76 minutos |
| Modalidad | Laboratorio |
| Complejidad | Intermedia |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Capítulo | 2 |
| Resultado principal | Conjunto de prompts reutilizables probados y refinados |

## Descripción General

El participante construirá una pequeña biblioteca de prompts basada en situaciones reales de su función. Cada prompt pasará por tres versiones: solicitud inicial, versión estructurada y versión validada. El laboratorio prioriza utilidad, repetibilidad y capacidad de revisión.

## Objetivos de Aprendizaje

- Construir prompts a partir de tareas reales.
- Aplicar objetivo, contexto, expectativas y fuente.
- Añadir formato, restricciones, tono y ejemplos cuando aporten valor.
- Refinar prompts mediante conversación.
- Documentar criterios de calidad y verificación.

## Prerrequisitos

### Conocimiento Requerido

- Capítulos 1 y 2.
- Uso básico de Copilot Chat.
- Capacidad de describir una tarea laboral sin incluir datos sensibles.

### Acceso Requerido

- Microsoft 365 Copilot Chat.
- Navegador e Internet.
- Documento de notas.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat (Licenciamiento Básico).

### Configuración Inicial

Cree una plantilla con estas secciones:

```text
Nombre del prompt:
Tarea:
Versión inicial:
Versión estructurada:
Versión refinada:
Criterios de calidad:
Qué debe verificarse:
```

---

## Paso 1: Seleccionar tres situaciones de trabajo

### Objetivo

Definir tareas que puedan resolverse mediante prompts reutilizables.

### Instrucciones

1. Elija tres categorías diferentes:
   - comunicación;
   - resumen/transformación;
   - análisis/comparación/ideación.
2. Ejemplos:
   - convertir notas en correo;
   - resumir un reporte;
   - comparar opciones;
   - preparar preguntas para una reunión;
   - transformar un texto técnico en explicación ejecutiva.
3. Describa cada tarea en una oración.

### Salida Esperada

Tres tareas concretas y sin datos sensibles.

### Verificación

- Cada tarea produce un entregable claro.
- Las tareas son repetibles.
- Ninguna requiere delegar una decisión de alto impacto.

---

## Paso 2: Crear la versión inicial

### Objetivo

Registrar cómo se formularía espontáneamente cada tarea.

### Instrucciones

1. Escriba un prompt corto para cada tarea.
2. Ejemplo:

```text
Resume este reporte.
```

3. Ejecute cada prompt con contenido ficticio o proporcionado por el instructor.
4. Registre qué faltó.

### Salida Esperada

Tres prompts iniciales y observaciones sobre sus limitaciones.

### Verificación

- Se ejecutaron los tres prompts.
- Se documentaron omisiones o ambigüedades.

---

## Paso 3: Estructurar cada prompt

### Objetivo

Mejorar control y utilidad.

### Instrucciones

1. Reescriba cada prompt con:
   - objetivo;
   - contexto;
   - fuente;
   - formato;
   - restricciones;
   - tono cuando corresponda.
2. Ejemplo de transformación:

**Solicitud inicial**

```text
Resume este documento.
```

**Solicitud estructurada**

```text
Resume este documento para un gerente de operaciones.

Utiliza únicamente la información del documento.

Incluye:
- tres hallazgos principales;
- dos riesgos;
- acciones pendientes;
- información que requiere validación.

Máximo 180 palabras.
No agregues nombres, fechas, cifras ni conclusiones que no estén sustentadas.
```

3. Ejecute la nueva versión.
4. Registre qué mejoró.

### Salida Esperada

Tres prompts estructurados y resultados más controlados.

### Verificación

- Todos los prompts establecen un objetivo.
- Todos definen formato y restricciones.
- La fuente queda delimitada cuando la tarea depende de información aportada.

---

## Paso 4: Añadir ejemplos solo cuando sean útiles

### Objetivo

Decidir de forma consciente cuándo emplear one-shot o few-shot.

### Instrucciones

1. Seleccione uno de sus tres prompts.
2. Cree un ejemplo pequeño del formato esperado.
3. Añada:

```text
Usa el siguiente ejemplo únicamente como patrón de estructura y tono.
No copies datos del ejemplo en la respuesta final.
```

4. Compare el resultado con la versión sin ejemplo.
5. Si el ejemplo no mejora el resultado, documente que no es necesario.

### Salida Esperada

Una decisión justificada sobre el uso de ejemplos.

### Verificación

- El ejemplo no introduce hechos falsos.
- El participante puede explicar si aportó valor o no.

---

## Paso 5: Refinar conversacionalmente

### Objetivo

Mejorar una respuesta sin reconstruir el prompt desde cero.

### Instrucciones

1. Elija una salida y envíe una instrucción de refinamiento:

```text
Mantén el contenido sustentado, pero reduce la respuesta a 120 palabras.
Conserva únicamente los tres puntos más relevantes para un gerente.
```

2. Después envíe:

```text
Ahora revisa si introdujiste algún dato que no aparezca en la fuente.
Si existe, elimínalo.
```

3. Finalmente:

```text
Devuélveme la instrucción completa que debería reutilizar la próxima vez para obtener este tipo de resultado desde el inicio.
```

### Salida Esperada

Una versión final del prompt más reusable y una respuesta refinada.

### Verificación

- La versión final incorpora los aprendizajes del refinamiento.
- No depende de recordar el historial de conversación para funcionar.

---

## Paso 6: Definir criterios de calidad y verificación

### Objetivo

Convertir la biblioteca de prompts en un recurso controlado.

### Instrucciones

1. Para cada prompt, complete:

```text
La respuesta es aceptable si:
- ...
- ...
- ...

Antes de usarla debo verificar:
- ...
- ...
- ...
```

2. Ejemplo:

```text
La respuesta es aceptable si:
- respeta el formato solicitado;
- utiliza solamente información de la fuente;
- mantiene el tono ejecutivo.

Antes de usarla debo verificar:
- cifras y fechas;
- nombres o responsables;
- que las acciones realmente estén acordadas.
```

### Salida Esperada

Tres prompts reutilizables con criterios de aceptación y verificación.

### Verificación

- La biblioteca contiene tres prompts completos.
- Cada prompt tiene controles explícitos.
- El participante podría reutilizarlo en una tarea futura.

---
