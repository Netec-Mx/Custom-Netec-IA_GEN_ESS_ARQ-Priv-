# Demostración guiada 1.1. Primera conversación controlada: recorrer Microsoft 365 Copilot Chat (Licenciamiento Básico), formular una necesidad de negocio, probar una respuesta y marcar qué partes requieren verificación

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 32 minutos |
| Modalidad | Demostración guiada |
| Complejidad | Básica |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Capítulo | 1. IA Generativa y Microsoft 365 Copilot Chat (Licenciamiento Básico) para el trabajo cotidiano |
| Resultado principal | Formular una solicitud de negocio básica, revisar la respuesta y separar lo utilizable de lo que requiere verificación |

## Descripción General

En esta demostración el instructor realiza una primera interacción controlada con Microsoft 365 Copilot Chat. La actividad muestra cómo convertir una necesidad cotidiana en una solicitud clara, cómo revisar la respuesta generada y cómo identificar afirmaciones, cifras, fechas, nombres o recomendaciones que deben verificarse antes de utilizarse.

La demostración no busca obtener una respuesta “perfecta” en el primer intento. El propósito es establecer desde el inicio un hábito de trabajo: **pedir → revisar → verificar → refinar**.

## Objetivos de Aprendizaje

- Reconocer los elementos principales de la interfaz de Microsoft 365 Copilot Chat.
- Formular una necesidad de negocio en lenguaje natural.
- Comparar una solicitud vaga con una solicitud contextualizada.
- Identificar información que puede utilizarse directamente y contenido que requiere validación.
- Aplicar revisión humana antes de reutilizar una respuesta.

## Prerrequisitos

### Conocimiento Requerido

| Concepto | Nivel |
|---|---|
| Uso básico de navegador web | Básico |
| Redacción de solicitudes en lenguaje natural | Básico |
| Criterio para revisar información de trabajo | Básico |

### Acceso Requerido

- Cuenta corporativa con Microsoft 365 Copilot Chat (Licenciamiento Básico).
- Navegador web.
- Conexión a Internet.
- Acceso al material de práctica proporcionado por el instructor.

## Entorno del Laboratorio

### Hardware Mínimo

El temario del curso no define especificaciones de CPU, memoria o almacenamiento. Se requiere únicamente un equipo que permita utilizar un navegador web compatible y mantener una conexión estable a Internet.

### Software Requerido

| Software / servicio | Requisito |
|---|---|
| Navegador web | Compatible con Microsoft 365 |
| Microsoft 365 Copilot Chat | Licenciamiento Básico |
| Editor de texto opcional | Para conservar prompts y observaciones |

### Configuración Inicial

1. Inicie sesión con la cuenta corporativa autorizada.
2. Abra Microsoft 365 Copilot Chat.
3. Inicie una conversación nueva.
4. Compruebe que puede escribir y enviar una solicitud.
5. Mantenga visible una hoja de notas para registrar qué información requeriría validación.

---

## Paso 1: Recorrer la interfaz y definir la necesidad

### Objetivo

Identificar el área de conversación y establecer una necesidad de negocio suficientemente concreta para iniciar una interacción.

### Instrucciones

1. Muestre el área donde se introduce una nueva solicitud.
2. Explique que una interacción útil comienza con una necesidad concreta, no con la búsqueda de una “respuesta mágica”.
3. Utilice el siguiente escenario:

   **Escenario:** una coordinadora debe preparar un resumen breve para su gerente sobre el estado de varias actividades de la semana.

4. Muestre primero una solicitud demasiado vaga:

```text
Ayúdame con mi reporte semanal.
```

5. Pregunte al grupo qué información falta para que la herramienta pueda producir algo realmente útil.
6. Identifique al menos estos elementos:
   - propósito;
   - audiencia;
   - información disponible;
   - formato esperado;
   - restricciones.

### Salida Esperada

El participante debe reconocer que la solicitud inicial no establece suficiente contexto y que la respuesta dependerá de supuestos de la herramienta.

### Verificación

- Se identificó la necesidad de negocio.
- El grupo detectó al menos tres datos faltantes en la solicitud.
- Quedó claro que un prompt vago obliga a la herramienta a completar contexto por inferencia.

---

## Paso 2: Convertir la necesidad en una solicitud controlada

### Objetivo

Construir una instrucción que limite el alcance y defina el resultado esperado.

### Instrucciones

1. Utilice estos datos ficticios:

```text
Actividades de la semana:
- Actualización del inventario: completada.
- Revisión de contratos con proveedores: 8 de 10 revisados.
- Capacitación interna: reprogramada para el jueves siguiente.
- Incidencias operativas: 3 abiertas; 1 de ellas pendiente de información del proveedor.
- Presupuesto del área: revisión preliminar terminada; falta aprobación del gerente.
```

2. Envíe este prompt:

```text
Necesito preparar un resumen semanal para mi gerente.

Utiliza únicamente la información que proporciono a continuación.

Genera:
- tres avances principales;
- dos pendientes;
- un riesgo que deba revisar el gerente;
- una lista de acciones para la próxima semana.

Máximo 180 palabras.
No inventes fechas, responsables, montos ni causas que no aparezcan en la información.

Información:
[pegar las actividades de la semana]
```

3. Lea la respuesta junto con los participantes.
4. Subraye qué partes provienen directamente de los datos y cuáles representan interpretación.

### Salida Esperada

La respuesta debe presentar avances, pendientes, riesgo y acciones con formato breve, sin añadir datos externos al escenario.

### Verificación

- La salida contiene las cuatro secciones solicitadas.
- No aparecen responsables, fechas o cifras inexistentes.
- El resumen respeta aproximadamente la longitud solicitada.
- Es posible rastrear cada punto hasta la información suministrada.

---

## Paso 3: Marcar qué debe verificarse

### Objetivo

Distinguir hechos aportados por el usuario, inferencias razonables y afirmaciones que no deberían utilizarse sin validación.

### Instrucciones

1. Envíe el siguiente mensaje de seguimiento:

```text
Revisa tu respuesta anterior contra la información que te proporcioné.

Clasifica cada afirmación importante como:
- Sustentada directamente.
- Inferida.
- No sustentada.

Para cada afirmación indica qué dato de la fuente la respalda.
Si una afirmación no está sustentada, propón eliminarla o reformularla.
```

2. Compare la clasificación con la información original.
3. Señale que incluso cuando la herramienta declara que algo está sustentado, la persona debe comprobarlo.
4. Si Copilot presenta una inferencia como hecho, pida corregirla:

```text
Reescribe el resumen eliminando toda afirmación no sustentada.
Cuando exista una inferencia útil, identifícala explícitamente como “interpretación para revisar”.
```

### Salida Esperada

Una revisión en la que los elementos principales queden asociados con evidencia disponible y las inferencias queden diferenciadas.

### Verificación

- Cada afirmación importante tiene una referencia a la información proporcionada.
- Las inferencias están diferenciadas de los hechos.
- No se mantienen afirmaciones sin sustento.
- El resultado final puede revisarse antes de compartirlo.

---
