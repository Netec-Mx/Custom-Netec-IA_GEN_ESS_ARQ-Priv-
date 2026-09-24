# Demostración guiada 4.2. Challenge my thinking: someter una propuesta a revisión crítica. Descubrir supuestos, puntos ciegos, contraargumentos y oportunidades de mejora

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 40 minutos |
| Modalidad | Demostración guiada |
| Complejidad | Intermedia |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Capítulo | 4 |
| Resultado principal | Utilizar IA para ampliar el análisis sin delegar la decisión |

## Descripción General

El instructor presenta una propuesta ficticia y pide a Copilot que la cuestione de manera estructurada. La salida se utiliza para descubrir supuestos, riesgos, información faltante y contraargumentos. La herramienta no decide si la propuesta debe aprobarse.

## Objetivos de Aprendizaje

- Solicitar crítica estructurada.
- Identificar supuestos y puntos ciegos.
- Generar contraargumentos.
- Separar hechos de hipótesis.
- Mantener la decisión final bajo revisión humana.

## Prerrequisitos

Uso de Copilot Chat y principios de validación.

### Acceso Requerido

Microsoft 365 Copilot Chat.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

Utilice esta propuesta ficticia:

```text
Propuesta:
Reducir la reunión operativa semanal de 60 a 30 minutos.
Antes de la reunión, cada responsable enviará una actualización breve.
La reunión se utilizará únicamente para bloqueos y decisiones pendientes.

Objetivo:
Reducir tiempo de reunión y hacer el seguimiento más enfocado.

Información disponible:
No se ha probado todavía el nuevo formato.
No existe una medición formal del tiempo actual dedicado a seguimiento fuera de la reunión.
```

---

## Paso 1: Identificar supuestos

### Objetivo

Hacer visibles las premisas implícitas.

### Instrucciones

Envíe:

```text
Analiza la propuesta sin aprobarla ni rechazarla.

Identifica:
- supuestos;
- información faltante;
- riesgos;
- grupos que podrían verse afectados.

Diferencia claramente lo que proviene del texto de lo que es una hipótesis para investigar.
```

### Salida Esperada

Lista de supuestos e información faltante, identificada como hipótesis cuando corresponda.

### Verificación

- No presenta hipótesis como hechos.
- No emite una decisión final.

---

## Paso 2: Generar contraargumentos

### Objetivo

Explorar objeciones razonables.

### Instrucciones

Envíe:

```text
Construye cuatro contraargumentos razonables que podría plantear alguien que no esté de acuerdo con la propuesta.

Para cada uno indica:
- preocupación;
- evidencia que sería necesaria para evaluarla;
- pregunta que deberíamos responder antes de decidir.
```

### Salida Esperada

Cuatro objeciones estructuradas y preguntas de validación.

### Verificación

- Las objeciones son relevantes.
- No se inventa evidencia.

---

## Paso 3: Mejorar la propuesta

### Objetivo

Convertir la crítica en mejoras verificables.

### Instrucciones

Envíe:

```text
Con base en los supuestos y objeciones, propone mejoras al diseño de la prueba.

No decidas si debemos implementar la propuesta definitivamente.
Enfócate en:
- qué medir;
- cuánto tiempo probar;
- qué feedback recopilar;
- qué condiciones indicarían que debemos ajustar.
```

### Salida Esperada

Un esquema de prueba o piloto, expresado como propuesta para revisión.

### Verificación

- La salida no confunde sugerencias con decisiones.
- Se proponen métricas o criterios que pueden discutirse.

---

## Paso 4: Separar análisis de decisión

### Objetivo

Cerrar la actividad reforzando la responsabilidad humana.

### Instrucciones

Envíe:

```text
Resume:
1. hechos disponibles;
2. supuestos;
3. preguntas abiertas;
4. alternativas para revisar.

No recomiendes una decisión final.
```

### Salida Esperada

Un paquete de análisis listo para discusión humana.

### Verificación

- No existe una decisión delegada a Copilot.
- Hechos y supuestos están separados.

---
