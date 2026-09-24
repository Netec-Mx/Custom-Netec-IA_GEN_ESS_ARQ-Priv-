# Demostración guiada 1.2. Semáforo de riesgos: clasificar solicitudes seguras, condicionadas y no recomendadas; anonimizar datos y reescribir prompts para reducir exposición

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 38 minutos |
| Modalidad | Demostración guiada |
| Complejidad | Básica |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Capítulo | 1 |
| Resultado principal | Clasificar solicitudes por riesgo y reescribirlas reduciendo exposición de información |

## Descripción General

La demostración introduce un criterio práctico de decisión antes de enviar información a una herramienta generativa. El instructor utiliza un “semáforo” con tres niveles: verde, amarillo y rojo. Los participantes observan cómo una tarea puede conservar su objetivo de negocio aun cuando se eliminen identificadores, cifras sensibles o detalles innecesarios.

## Objetivos de Aprendizaje

- Diferenciar solicitudes de bajo, medio y alto riesgo.
- Identificar información que no es necesaria para resolver una tarea.
- Anonimizar datos antes de utilizarlos en un prompt.
- Reformular solicitudes para minimizar exposición.
- Reconocer situaciones en las que conviene detenerse y consultar políticas internas.

## Prerrequisitos

### Conocimiento Requerido

| Concepto | Nivel |
|---|---|
| Uso básico de Copilot Chat | Básico |
| Identificación básica de información sensible | Básico |
| Revisión humana | Básico |

### Acceso Requerido

- Cuenta corporativa con Microsoft 365 Copilot Chat (Licenciamiento Básico).
- Navegador e Internet.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet. El temario no establece requisitos adicionales.

### Software Requerido

| Software / servicio | Requisito |
|---|---|
| Microsoft 365 Copilot Chat | Licenciamiento Básico |
| Navegador web | Acceso corporativo |

### Configuración Inicial

Prepare tres etiquetas visibles: **Verde**, **Amarillo** y **Rojo**.

Definición didáctica para la actividad:

- **Verde:** información de bajo riesgo o ya preparada para uso interno autorizado.
- **Amarillo:** la tarea puede realizarse, pero primero deben eliminarse o generalizarse datos innecesarios y verificarse políticas.
- **Rojo:** contiene datos cuya exposición no está justificada o requiere autorización/política específica antes de utilizarse.

---

## Paso 1: Clasificar solicitudes

### Objetivo

Aplicar el semáforo a solicitudes realistas de distintas áreas de negocio.

### Instrucciones

1. Presente una solicitud por vez.
2. Pida a los participantes clasificarla antes de explicar la respuesta.

**Caso A**

```text
Crea cinco opciones de asunto para un correo interno que invite al personal a una sesión de capacitación sobre servicio al cliente.
```

**Caso B**

```text
Ayúdame a mejorar la redacción de este seguimiento de cobranza.
Cliente: Empresa Delta.
Saldo vencido: 248,700.
Contacto: Laura Hernández.
Teléfono: 55-0000-0000.
Correo: laura@example.com.
```

**Caso C**

```text
Analiza esta lista de empleados con nombre, domicilio, número de identificación, salario, evaluación de desempeño y observaciones médicas. Indica quién debería ser despedido.
```

3. Clasifique didácticamente:
   - Caso A: verde.
   - Caso B: amarillo; la tarea puede reformularse sin datos identificables ni cifras exactas si no son necesarias.
   - Caso C: rojo para esta práctica; contiene datos personales/sensibles y además delega una decisión laboral de alto impacto.

4. Explique que el semáforo es un recurso didáctico y no sustituye las políticas de la organización.

### Salida Esperada

Los participantes distinguen que el riesgo depende tanto de la información suministrada como de la decisión que se pretende delegar.

### Verificación

- Se clasificaron los tres casos.
- Se justificó la clasificación.
- Se identificaron datos innecesarios en los casos B y C.
- Se reconoció que ciertas decisiones no deben delegarse automáticamente.

---

## Paso 2: Anonimizar una solicitud condicionada

### Objetivo

Conservar el valor de la tarea reduciendo la cantidad de información expuesta.

### Instrucciones

1. Compare la versión original del caso B con esta versión anonimizada:

```text
Ayúdame a mejorar la redacción de un correo de seguimiento de cobranza.

Contexto:
- Es un cliente empresarial.
- Existe un saldo vencido.
- Ya se envió un primer recordatorio.
- Quiero mantener un tono profesional y colaborativo.

Genera:
- asunto;
- cuerpo del mensaje;
- cierre;
- una versión de máximo 130 palabras.

No inventes fechas, compromisos, importes ni consecuencias.
Utiliza los marcadores [CLIENTE], [SALDO] y [FECHA] donde sea necesario.
```

2. Envíe el prompt.
3. Muestre que el objetivo puede lograrse sin nombre, teléfono, correo ni importe real.
4. Explique que los marcadores se reemplazan fuera de la conversación, cuando corresponda.

### Salida Esperada

Un borrador reutilizable que no dependa de datos identificables.

### Verificación

- No aparecen datos reales de personas.
- El texto conserva la intención del seguimiento.
- Los valores sensibles se sustituyen por marcadores.
- La respuesta no inventa amenazas, fechas ni compromisos.

---

## Paso 3: Reescribir una solicitud de alto riesgo

### Objetivo

Transformar una petición improcedente en una actividad de apoyo que conserve revisión humana.

### Instrucciones

1. No utilice datos reales.
2. Sustituya la petición del caso C por una solicitud de apoyo no decisoria:

```text
Ayúdame a crear una lista de criterios neutrales para que un responsable de Recursos Humanos revise de forma consistente un proceso de desempeño.

Los criterios deben centrarse en:
- cumplimiento de objetivos previamente definidos;
- evidencia documentada;
- consistencia en el periodo evaluado;
- acciones de mejora;
- información que debe validar una persona responsable.

No evalúes a ningún empleado y no recomiendes decisiones laborales.
```

3. Revise la respuesta.
4. Identifique qué elementos siguen requiriendo política, contexto organizacional y criterio humano.

### Salida Esperada

Una lista de criterios de revisión, no una decisión sobre personas.

### Verificación

- La herramienta no selecciona ni clasifica empleados.
- La salida se limita a criterios generales.
- Se conserva una etapa explícita de revisión humana.
- El participante puede explicar por qué la segunda formulación reduce el riesgo.

---
