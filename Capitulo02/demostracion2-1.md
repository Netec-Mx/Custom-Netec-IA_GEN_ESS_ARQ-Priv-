# Demostración guiada 2.1. Anatomía del prompt: convertir solicitudes vagas en prompts estructurados y comparar cómo cambia la calidad, precisión y formato de la respuesta

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 35 minutos |
| Modalidad | Demostración guiada |
| Complejidad | Básica–intermedia |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Capítulo | 2. Prompting efectivo |
| Resultado principal | Construir prompts con objetivo, contexto, expectativas, fuente, formato y restricciones |

## Descripción General

La demostración muestra cómo una misma necesidad produce resultados distintos cuando se formula de manera vaga o estructurada. El instructor construye el prompt en capas y compara cambios en relevancia, precisión, tono y formato.

## Objetivos de Aprendizaje

- Reconocer los componentes de un prompt estructurado.
- Mejorar solicitudes vagas de forma incremental.
- Separar objetivo, contexto, fuente, formato y restricciones.
- Observar el efecto de cada elemento sobre la respuesta.

## Prerrequisitos

### Conocimiento Requerido

| Concepto | Nivel |
|---|---|
| Uso básico de Copilot Chat | Básico |
| Revisión de respuestas | Básico |
| Capítulo 1 completado | Recomendado |

### Acceso Requerido

- Microsoft 365 Copilot Chat (Licenciamiento Básico).
- Navegador e Internet.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

| Software / servicio | Requisito |
|---|---|
| Microsoft 365 Copilot Chat | Licenciamiento Básico |
| Navegador | Requerido |

### Configuración Inicial

Abra una conversación nueva para evitar que el contexto previo influya en el ejercicio.

---

## Paso 1: Probar una solicitud vaga

### Objetivo

Observar cómo una instrucción insuficiente produce una salida genérica.

### Instrucciones

1. Envíe:

```text
Haz un correo sobre el cambio de proceso.
```

2. Revise la respuesta.
3. Identifique qué tuvo que asumir Copilot:
   - qué proceso cambió;
   - quién recibe el correo;
   - qué debe hacer el lector;
   - cuándo aplica;
   - tono;
   - extensión.

### Salida Esperada

Un correo genérico con supuestos no definidos por el usuario.

### Verificación

- Se identificaron al menos cuatro supuestos.
- El grupo puede explicar por qué la respuesta no está lista para usarse.

---

## Paso 2: Construir el prompt por capas

### Objetivo

Añadir información de forma incremental y observar el impacto.

### Instrucciones

1. Agregue el **objetivo**:

```text
Redacta un correo para comunicar un cambio de proceso.
El objetivo es que el personal conozca el nuevo procedimiento y sepa qué debe hacer.
```

2. Agregue **contexto**:

```text
Audiencia: personal administrativo.
Cambio: a partir de la próxima semana las solicitudes internas deberán registrarse mediante un formulario antes de enviarse a revisión.
```

3. Agregue **expectativas y formato**:

```text
Incluye:
- asunto;
- explicación breve del cambio;
- tres acciones que debe realizar el personal;
- cierre con invitación a consultar dudas.

Máximo 170 palabras.
```

4. Agregue **restricciones**:

```text
No inventes enlaces, nombres de sistemas, responsables ni fechas distintas de las proporcionadas.
Tono profesional, claro y cercano.
```

5. Envíe el prompt completo.

### Salida Esperada

Un correo más relevante y estructurado, alineado con la audiencia y sin información inventada.

### Verificación

- Existe asunto.
- Se describen tres acciones.
- El tono es apropiado.
- No aparecen nombres de plataformas o responsables inexistentes.

---

## Paso 3: Comparar calidad, precisión y formato

### Objetivo

Convertir la comparación en criterios observables.

### Instrucciones

1. Pida:

```text
Compara tu primera respuesta con la respuesta obtenida con el prompt estructurado.

Evalúa:
- claridad;
- relevancia;
- precisión;
- adecuación a la audiencia;
- cumplimiento de formato;
- cantidad de supuestos.

No asignes una calificación global. Explica diferencias concretas.
```

2. Revise la comparación.
3. Confirme manualmente si las diferencias son reales.

### Salida Esperada

Una comparación que muestre que la estructura reduce ambigüedad y mejora el control de la salida.

### Verificación

- La comparación usa criterios concretos.
- Se detectan menos supuestos en la segunda versión.
- El participante puede identificar qué componente produjo cada mejora.

---
