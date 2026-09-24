# Demostración guiada 3.1. Cadena de transformación: partir de un texto fuente y producir resumen ejecutivo, correo, tabla y lista de acciones, verificando que no se agreguen hechos no sustentados

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 35 minutos |
| Modalidad | Demostración guiada |
| Complejidad | Intermedia |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Capítulo | 3 |
| Resultado principal | Transformar una misma fuente en cuatro formatos manteniendo trazabilidad |

## Descripción General

El instructor utiliza un texto fuente único y lo transforma sucesivamente en resumen ejecutivo, correo, tabla y lista de acciones. La demostración hace visible el riesgo de que una transformación introduzca detalles inexistentes y establece una validación contra la fuente antes de reutilizar cada salida.

## Objetivos de Aprendizaje

- Transformar contenido sin cambiar los hechos.
- Adaptar formato y audiencia.
- Solicitar restricciones explícitas.
- Validar cada salida contra la fuente.

## Prerrequisitos

- Uso de prompts estructurados.
- Revisión de respuestas.
- Capítulos 1 y 2.

### Acceso Requerido

Microsoft 365 Copilot Chat (Licenciamiento Básico).

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

Utilice el siguiente texto ficticio:

```text
Durante la revisión mensual del proyecto se confirmó que 18 de 20 actividades previstas fueron completadas. Dos actividades de validación permanecen abiertas porque el área responsable solicitó revisar información adicional. La capacitación de usuarios se realizó con 24 participantes. Se identificaron tres dudas recurrentes relacionadas con el nuevo procedimiento. El equipo acordó preparar una guía breve de preguntas frecuentes. La fecha de cierre de las dos validaciones pendientes todavía no está confirmada.
```

---

## Paso 1: Generar un resumen ejecutivo

### Objetivo

Reducir el contenido conservando los hechos principales.

### Instrucciones

Envíe:

```text
Resume el texto para un gerente.

Incluye:
- avance;
- pendiente principal;
- hecho relevante de adopción;
- información aún no confirmada.

Máximo 100 palabras.
Utiliza únicamente hechos presentes en la fuente.
```

### Salida Esperada

Un resumen que mencione 18 de 20 actividades, dos validaciones abiertas, 24 participantes, tres dudas recurrentes y la ausencia de fecha confirmada, sin agregar responsables o fechas.

### Verificación

- Todos los hechos aparecen en la fuente.
- No hay fechas inventadas.
- No se presentan las validaciones como cerradas.

---

## Paso 2: Convertir el resumen en correo

### Objetivo

Adaptar el contenido a una comunicación ejecutiva sin introducir nueva información.

### Instrucciones

Envíe:

```text
Convierte el resumen en un correo interno.

Incluye:
- asunto;
- apertura de una frase;
- avances;
- pendientes;
- cierre.

Tono profesional y directo.
No agregues compromisos, responsables ni fechas.
```

### Salida Esperada

Un correo breve que conserva la misma información factual.

### Verificación

- El correo no agrega decisiones.
- El tono cambia, pero los hechos se mantienen.

---

## Paso 3: Transformar la información en tabla

### Objetivo

Estructurar el mismo contenido para revisión rápida.

### Instrucciones

Envíe:

```text
Convierte la información original en una tabla con las columnas:
Elemento | Estado | Evidencia de la fuente | Requiere seguimiento

No agregues elementos que no aparezcan en el texto.
```

### Salida Esperada

Una tabla con actividades, validaciones, capacitación, dudas y guía de preguntas frecuentes.

### Verificación

- Cada fila puede rastrearse a la fuente.
- La tabla no introduce nuevos hechos.

---

## Paso 4: Generar lista de acciones y validar

### Objetivo

Diferenciar acciones explícitas de sugerencias.

### Instrucciones

1. Envíe:

```text
Extrae únicamente las acciones explícitas que aparecen en la fuente.
No propongas acciones nuevas.
```

2. Después:

```text
Revisa todas las salidas anteriores.
Identifica cualquier hecho que no aparezca literalmente o de forma inequívoca en la fuente.
Si existe, señálalo para eliminarlo.
```

### Salida Esperada

La acción explícita principal debe ser preparar una guía breve de preguntas frecuentes. No debe aparecer una fecha de cierre inventada.

### Verificación

- Las acciones extraídas son realmente explícitas.
- No se confunden recomendaciones con acuerdos.
- La validación final detecta cualquier desviación.

---
