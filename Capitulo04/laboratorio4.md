# Laboratorio 4. Reto integrador por rol: resolver una tarea real de principio a fin, refinar el prompt, validar fuentes y contenido, aplicar controles de privacidad y guardar el patrón final en una biblioteca personal

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 71 minutos |
| Modalidad | Laboratorio integrador |
| Complejidad | Intermedia |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Capítulo | 4 |
| Resultado principal | Flujo completo y reusable: necesidad → prompt → resultado → validación → control → biblioteca |

## Descripción General

El laboratorio integra los hábitos trabajados durante el curso. Cada participante selecciona una tarea de su rol, define el resultado deseado, prepara información autorizada, construye y refina un prompt, valida la respuesta, aplica controles de privacidad y guarda el patrón final como recurso reutilizable.

## Objetivos de Aprendizaje

- Resolver una tarea completa con Copilot Chat.
- Diseñar y refinar un prompt.
- Trabajar con una fuente o información proporcionada.
- Validar afirmaciones.
- Aplicar controles de privacidad.
- Documentar un prompt reutilizable.

## Prerrequisitos

### Conocimiento Requerido

| Concepto | Nivel |
|---|---|
| Prompting estructurado | Intermedio |
| Validación de respuestas | Intermedio |
| Manejo responsable de información | Básico–intermedio |
| Trabajo con archivos o texto fuente | Básico–intermedio |

### Acceso Requerido

- Microsoft 365 Copilot Chat (Licenciamiento Básico).
- Navegador e Internet.
- Archivo de práctica del instructor o contenido ficticio.
- Documento de notas para biblioteca personal.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

Seleccione un escenario por rol:

| Perfil | Ejemplo de reto |
|---|---|
| Administración | Convertir información de seguimiento en reporte ejecutivo |
| Comercial | Preparar una reunión y adaptar un mensaje para cliente |
| Finanzas | Transformar observaciones de un reporte en hallazgos y preguntas de validación |
| Recursos Humanos | Convertir una política proporcionada en comunicación y preguntas frecuentes |
| Operaciones | Analizar incidencias y preparar una lista de seguimiento |
| Servicio | Resumir retroalimentación y preparar temas para revisión |

No utilice datos reales sensibles durante el laboratorio.

---

## Paso 1: Definir el reto y el criterio de éxito

### Objetivo

Establecer qué se quiere lograr antes de interactuar con Copilot.

### Instrucciones

Complete:

```text
Mi rol:
Tarea:
Audiencia:
Resultado final:
Fuente que utilizaré:
Qué no debe hacer Copilot:
Qué revisaré antes de utilizar la salida:
```

### Salida Esperada

Una definición concreta del reto.

### Verificación

- Existe una audiencia.
- Existe una fuente o conjunto de datos autorizado.
- Se definen límites.

---

## Paso 2: Revisar privacidad antes de enviar información

### Objetivo

Reducir exposición innecesaria.

### Instrucciones

1. Revise el contenido.
2. Pregúntese:
   - ¿necesito realmente nombres?
   - ¿necesito importes exactos?
   - ¿puedo usar datos ficticios o marcadores?
   - ¿la organización permite utilizar esta información?
3. Sustituya datos cuando sea posible:

```text
[CLIENTE]
[PROYECTO]
[PERSONA]
[FECHA]
[IMPORTE]
```

4. Si la tarea no puede realizarse sin información cuya utilización debe autorizarse, detenga el laboratorio y utilice el material ficticio del instructor.

### Salida Esperada

Una fuente preparada para práctica con el mínimo de información necesaria.

### Verificación

- Se eliminaron datos innecesarios.
- No se utilizaron secretos, credenciales o información sensible real.

---

## Paso 3: Construir el prompt versión 1

### Objetivo

Crear una primera versión estructurada.

### Instrucciones

Use:

```text
Objetivo:
[resultado]

Contexto:
[rol, audiencia y propósito]

Fuente:
[texto o archivo autorizado]

Genera:
[formato]

Restricciones:
- utiliza únicamente la fuente;
- no inventes datos;
- identifica información faltante;
- [otras restricciones de la tarea].
```

2. Ejecute.
3. Registre dos aciertos y dos problemas.

### Salida Esperada

Una primera respuesta evaluable.

### Verificación

- El prompt incluye fuente y formato.
- La respuesta puede compararse con criterios definidos.

---

## Paso 4: Refinar la respuesta

### Objetivo

Corregir problemas sin perder trazabilidad.

### Instrucciones

Utilice mensajes de seguimiento según corresponda:

```text
Reduce la respuesta y conserva únicamente los elementos sustentados.
```

```text
Adapta el tono para [audiencia] sin cambiar hechos.
```

```text
Convierte el resultado en una tabla con las columnas [...]
```

```text
Señala qué información falta para completar la tarea sin hacer suposiciones.
```

### Salida Esperada

Una versión mejor alineada con el propósito.

### Verificación

- Cada refinamiento responde a un problema identificado.
- No se introdujeron nuevos hechos.

---

## Paso 5: Validar fuentes y contenido

### Objetivo

Comprobar la respuesta de forma sistemática.

### Instrucciones

Envíe:

```text
Audita tu respuesta contra la fuente.

Crea una tabla:
Afirmación importante | Evidencia | Sustentada / Inferida / No sustentada

Reglas:
- Si no existe evidencia suficiente, marca “No sustentada”.
- No intentes completar vacíos.
- No uses conocimiento externo.
```

2. Compruebe manualmente al menos cinco afirmaciones o todas si hay menos de cinco.
3. Elimine o corrija cualquier elemento no sustentado.

### Salida Esperada

Una tabla de validación y una versión corregida.

### Verificación

- Se realizó comprobación manual.
- No quedan afirmaciones no sustentadas en la versión final.

---

## Paso 6: Realizar una revisión crítica

### Objetivo

Buscar puntos ciegos antes de cerrar la tarea.

### Instrucciones

Envíe:

```text
Revisa el resultado final como un crítico constructivo.

Identifica:
- un supuesto que todavía pueda estar presente;
- una pregunta que debería hacer antes de utilizarlo;
- una posible interpretación ambigua;
- una comprobación final que deba realizar una persona.

No cambies los hechos ni tomes la decisión por mí.
```

### Salida Esperada

Una lista breve de controles adicionales.

### Verificación

- La herramienta no decide por el participante.
- Se obtiene al menos una comprobación útil.

---

## Paso 7: Guardar el patrón en la biblioteca personal

### Objetivo

Convertir el aprendizaje en un recurso reusable.

### Instrucciones

Documente:

```text
Nombre del patrón:
Cuándo utilizarlo:
Qué fuente requiere:
Prompt final:
Variables que debo reemplazar:
Qué debo verificar:
Información que nunca debo incluir:
Ejemplo de salida aceptable:
```

2. Elimine del patrón cualquier dato específico usado durante el ejercicio.
3. Sustituya por marcadores.
4. Guarde el patrón en su documento personal autorizado.

### Salida Esperada

Un prompt reusable y documentado.

### Verificación

- No contiene datos de la práctica que no deban conservarse.
- Incluye variables reemplazables.
- Incluye controles de privacidad y verificación.
- Puede reutilizarse en una tarea futura.

---
