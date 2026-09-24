# Demostración guiada 2.2. Experimento controlado: resolver una misma tarea con zero-shot, one-shot y few-shot; imponer formatos y restricciones y comparar los resultados

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 42 minutos |
| Modalidad | Demostración guiada |
| Complejidad | Intermedia |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Capítulo | 2 |
| Resultado principal | Comprender cuándo los ejemplos ayudan a orientar formato, tono y consistencia |

## Descripción General

El instructor resuelve la misma tarea tres veces: sin ejemplo, con un ejemplo y con varios ejemplos. El objetivo no es demostrar que una técnica siempre es superior, sino observar cuándo los ejemplos aportan claridad y cuándo resultan innecesarios.

## Objetivos de Aprendizaje

- Diferenciar zero-shot, one-shot y few-shot.
- Utilizar ejemplos como guía de forma y estilo.
- Imponer formatos y restricciones explícitas.
- Comparar resultados sin asumir que más ejemplos siempre producen una mejor respuesta.

## Prerrequisitos

### Conocimiento Requerido

| Concepto | Nivel |
|---|---|
| Prompt estructurado | Básico |
| Revisión de formato | Básico |
| Copilot Chat | Básico |

### Acceso Requerido

- Microsoft 365 Copilot Chat (Licenciamiento Básico).

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat y navegador web.

### Configuración Inicial

Utilice una conversación nueva o reinicie el contexto entre variantes cuando sea posible.

---

## Paso 1: Zero-shot

### Objetivo

Resolver la tarea sin proporcionar ejemplos.

### Instrucciones

1. Utilice estos datos ficticios:

```text
Incidencia: retraso en entrega de reporte mensual.
Impacto: el comité no contará con la versión final antes de su reunión.
Estado: análisis completado; falta validar dos cifras.
Acción siguiente: revisión con Finanzas.
```

2. Envíe:

```text
Convierte la información en una actualización ejecutiva.

Formato:
- Situación
- Impacto
- Estado
- Siguiente acción

Máximo 80 palabras.
No inventes responsables, fechas ni cifras.
```

3. Guarde la respuesta como **Versión A**.

### Salida Esperada

Una actualización ejecutiva con las cuatro secciones solicitadas.

### Verificación

- Respeta la estructura.
- No agrega datos inexistentes.
- Se mantiene dentro de una extensión breve.

---

## Paso 2: One-shot

### Objetivo

Mostrar a Copilot un ejemplo del patrón esperado.

### Instrucciones

1. Añada un ejemplo ficticio:

```text
Ejemplo del formato esperado:

Situación: El proveedor entregó parcialmente la documentación.
Impacto: La validación no puede cerrarse.
Estado: Se revisó la información disponible.
Siguiente acción: Confirmar los documentos faltantes con el proveedor.
```

2. Después del ejemplo, agregue los datos originales y pida:

```text
Ahora aplica exactamente esta estructura al siguiente caso.
No copies el contenido del ejemplo; úsalo únicamente como patrón.
```

3. Guarde la respuesta como **Versión B**.

### Salida Esperada

Una salida más cercana al patrón mostrado, sin copiar hechos del ejemplo.

### Verificación

- Mantiene las cuatro etiquetas.
- No transfiere al nuevo caso el “proveedor” del ejemplo.
- El texto se ajusta a los datos del nuevo escenario.

---

## Paso 3: Few-shot

### Objetivo

Utilizar varios ejemplos para reforzar un patrón de salida.

### Instrucciones

1. Proporcione dos ejemplos breves adicionales, cada uno con situaciones diferentes.
2. Indique:

```text
Los ejemplos muestran únicamente el patrón de redacción.
No reutilices hechos, nombres ni circunstancias de los ejemplos.

Genera la actualización del caso original con:
- una frase por sección;
- lenguaje ejecutivo;
- máximo 70 palabras;
- sin recomendaciones que no estén sustentadas.
```

3. Guarde la respuesta como **Versión C**.

### Salida Esperada

Una salida consistente con el patrón y con menor variación de estilo.

### Verificación

- La salida respeta una frase por sección.
- No copia hechos de los ejemplos.
- Mantiene la información original.

---

## Paso 4: Comparar y decidir cuándo usar ejemplos

### Objetivo

Determinar si los ejemplos agregaron valor real.

### Instrucciones

1. Compare A, B y C mediante esta tabla:

| Criterio | A | B | C |
|---|---|---|---|
| Formato correcto | | | |
| Tono consistente | | | |
| Información sustentada | | | |
| Supuestos introducidos | | | |
| Esfuerzo para construir el prompt | | | |

2. Concluya:
   - zero-shot es suficiente cuando la instrucción ya define claramente la salida;
   - one-shot puede ayudar cuando se desea un patrón específico;
   - few-shot puede ser útil cuando la consistencia entre varias salidas importa.

### Salida Esperada

Una comparación práctica de las tres técnicas.

### Verificación

- El participante distingue las tres técnicas.
- Puede justificar cuál usaría según la tarea.
- No concluye automáticamente que few-shot siempre sea necesario.

---
