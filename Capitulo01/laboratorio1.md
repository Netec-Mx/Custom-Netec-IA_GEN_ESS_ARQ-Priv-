# Laboratorio 1. Mi mapa de oportunidades y uso seguro de Microsoft 365 Copilot Chat (Licenciamiento Básico): Identificar tareas reales del entorno laboral en las que Copilot puede aportar valor, experimentar con instrucciones básicas y determinar qué información puede utilizarse, qué resultados deben verificarse y qué riesgos deben considerarse antes de utilizar una respuesta

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 77 minutos |
| Modalidad | Laboratorio |
| Complejidad | Básica |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Capítulo | 1 |
| Resultado principal | Mapa personal de oportunidades, riesgos y controles de uso |

## Descripción General

El participante construirá un mapa de tareas de su propio entorno laboral que podrían beneficiarse de Copilot Chat. Cada oportunidad se probará con una solicitud básica y luego se revisará desde tres perspectivas: utilidad, verificación y seguridad. El resultado final es una tabla de decisiones que identifica qué tareas son apropiadas, cuáles requieren condiciones y cuáles deben evitarse o escalarse.

## Objetivos de Aprendizaje

- Identificar tareas reales donde Copilot Chat puede aportar valor.
- Formular prompts iniciales para tareas cotidianas.
- Determinar qué información es necesaria y cuál debe eliminarse.
- Identificar qué resultados requieren verificación.
- Crear reglas personales de uso seguro.

## Prerrequisitos

### Conocimiento Requerido

| Concepto | Nivel |
|---|---|
| Uso básico de navegador | Básico |
| Conocimiento de las propias tareas de trabajo | Básico |
| Principios explicados en el capítulo 1 | Básico |

### Acceso Requerido

- Cuenta corporativa con Microsoft 365 Copilot Chat (Licenciamiento Básico).
- Navegador web e Internet.
- Material de práctica del instructor.
- No utilizar datos personales, confidenciales o sensibles reales durante el laboratorio.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador web e Internet. No se requieren herramientas de desarrollo.

### Software Requerido

| Software / servicio | Requisito |
|---|---|
| Microsoft 365 Copilot Chat | Licenciamiento Básico |
| Navegador web | Requerido |
| Hoja de notas o documento | Para construir el mapa de oportunidades |

### Configuración Inicial

Cree una tabla con estas columnas:

| Tarea | Valor esperado | Información necesaria | Riesgo | Qué verificar | Decisión |
|---|---|---|---|---|---|

---

## Paso 1: Inventario de oportunidades

### Objetivo

Identificar tareas propias que sean repetitivas, intensivas en texto, análisis, síntesis, comparación o ideación.

### Instrucciones

1. Escriba entre cinco y ocho tareas frecuentes de su puesto.
2. No incluya todavía nombres de clientes, empleados, proveedores ni datos reales.
3. Utilice como guía estas categorías:
   - redactar;
   - resumir;
   - transformar;
   - analizar;
   - comparar;
   - idear.
4. Ejemplos por perfil:

   **Administración**
   - convertir notas en minuta;
   - estructurar un reporte semanal.

   **Comercial**
   - preparar preguntas para una reunión;
   - adaptar un mensaje a distintos perfiles de cliente.

   **Finanzas**
   - explicar un reporte en lenguaje ejecutivo;
   - convertir observaciones en lista de validaciones.

   **Recursos Humanos**
   - preparar una guía de preguntas para entrevista;
   - resumir una política para comunicación interna.

   **Operaciones**
   - convertir incidencias en una lista de acciones;
   - comparar dos alternativas operativas.

5. Seleccione tres tareas que considere de mayor valor y márquelas como A, B y C.

### Salida Esperada

Una lista de al menos cinco tareas, con tres oportunidades priorizadas.

### Verificación

- Las tareas corresponden al trabajo real del participante.
- No contienen información sensible real.
- Las tres seleccionadas pueden formularse como solicitudes concretas.

---

## Paso 2: Probar una instrucción básica

### Objetivo

Observar qué ocurre cuando la necesidad se expresa con poco contexto.

### Instrucciones

1. Elija la tarea A.
2. Escriba una solicitud básica. Ejemplo:

```text
Ayúdame a preparar una minuta de reunión.
```

3. Revise la respuesta.
4. Registre:
   - qué supuso Copilot;
   - qué información faltó;
   - qué partes serían poco útiles;
   - qué riesgo existe si la respuesta se usa sin revisar.

5. Complete la fila correspondiente en su mapa.

### Salida Esperada

Una primera respuesta que permita observar limitaciones por falta de contexto.

### Verificación

- Se registró al menos un supuesto introducido por la herramienta.
- Se identificó información faltante.
- Se documentó qué tendría que verificarse.

---

## Paso 3: Mejorar la solicitud

### Objetivo

Añadir objetivo, contexto, formato y restricciones para obtener un resultado más controlado.

### Instrucciones

1. Use este patrón:

```text
Objetivo:
[qué necesito]

Contexto:
[para quién y para qué]

Información disponible:
[datos que sí puedo proporcionar]

Genera:
[formato deseado]

Restricciones:
[qué no debe inventar, longitud, tono u otras reglas]
```

2. Ejemplo para una minuta:

```text
Objetivo:
Convertir notas de una reunión en una minuta breve.

Contexto:
La minuta será enviada a un equipo interno de operaciones.

Información disponible:
- Se revisó el avance del proyecto Alfa.
- El proveedor entregará una actualización el viernes.
- El equipo de operaciones revisará dos incidencias abiertas.
- La fecha de la siguiente reunión aún no está definida.

Genera:
- objetivo de la reunión;
- acuerdos;
- pendientes;
- información por confirmar.

Restricciones:
No inventes responsables, fechas ni decisiones que no aparezcan en las notas.
Máximo 200 palabras.
```

3. Compare la nueva respuesta con la obtenida en el paso anterior.
4. Registre dos mejoras observables.

### Salida Esperada

Una respuesta más útil, estructurada y limitada por la información disponible.

### Verificación

- La salida sigue el formato solicitado.
- No añade responsables o fechas inexistentes.
- El participante identifica al menos dos mejoras respecto del prompt inicial.

---

## Paso 4: Aplicar el semáforo de riesgo

### Objetivo

Determinar qué información puede utilizarse, qué debe anonimizarse y qué debería excluirse.

### Instrucciones

1. Para las tareas A, B y C, enumere la información que normalmente usaría.
2. Clasifique cada dato:
   - verde;
   - amarillo;
   - rojo.
3. Elimine de su prompt cualquier dato que no sea imprescindible.
4. Cuando sea posible, sustituya valores por marcadores:

```text
[CLIENTE]
[ÁREA]
[IMPORTE]
[FECHA]
[PROYECTO]
```

5. Si una tarea exige información que no debería incluirse sin autorización, márquela como **“Escalar / validar política”**.

### Salida Esperada

Tres tareas con una decisión explícita sobre qué información utilizar y qué información excluir o anonimizar.

### Verificación

- Cada tarea tiene una clasificación de riesgo.
- No se utilizan datos reales sensibles.
- Las tareas condicionadas indican el control requerido.

---

## Paso 5: Definir criterios de verificación

### Objetivo

Establecer qué debe comprobarse antes de reutilizar una respuesta.

### Instrucciones

1. Para cada tarea seleccionada, defina al menos tres puntos de control.
2. Utilice esta guía:

```text
Antes de utilizar la respuesta debo comprobar:
1. Que los nombres y cifras provienen de mi fuente.
2. Que no se agregaron compromisos o fechas.
3. Que el tono es apropiado para la audiencia.
4. Que las conclusiones están respaldadas.
5. Que la información utilizada puede compartirse.
```

3. Añada los controles a la columna **Qué verificar**.
4. Marque la decisión final:
   - Usar.
   - Usar con condiciones.
   - No usar / escalar.

### Salida Esperada

Un mapa completo de oportunidades con utilidad, datos requeridos, riesgo, controles y decisión.

### Verificación

- El mapa contiene al menos tres tareas evaluadas completamente.
- Cada tarea tiene controles de verificación.
- Ninguna decisión depende únicamente de la respuesta de Copilot.
- El participante puede explicar por qué una tarea es segura, condicionada o no recomendada.

---
