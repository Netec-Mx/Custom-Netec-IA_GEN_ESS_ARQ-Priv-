# Demostración guiada 3.2. Reto de evidencia con archivos: cargar un archivo proporcionado, extraer datos, hacer preguntas, solicitar soporte en la fuente y detectar respuestas no sustentadas

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 45 minutos |
| Modalidad | Demostración guiada |
| Complejidad | Intermedia |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Capítulo | 3 |
| Resultado principal | Consultar un archivo y exigir evidencia rastreable |

## Descripción General

El instructor agrega a Copilot Chat un archivo de práctica proporcionado para el curso y utiliza preguntas progresivas: extracción, resumen, soporte en fuente y prueba de límites. La demostración enseña a detectar cuándo una respuesta excede el contenido disponible.

## Objetivos de Aprendizaje

- Agregar un archivo a la conversación.
- Formular preguntas concretas sobre su contenido.
- Solicitar evidencia o soporte.
- Detectar preguntas que la fuente no puede responder.
- Evitar aceptar respuestas plausibles pero no sustentadas.

## Prerrequisitos

### Conocimiento Requerido

- Uso básico de archivos.
- Prompting estructurado.
- Verificación de respuestas.

### Acceso Requerido

- Archivo de práctica proporcionado por el instructor.
- Microsoft 365 Copilot Chat.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

1. Descargue o localice el archivo de práctica del instructor.
2. No utilice documentos confidenciales personales.
3. Abra una conversación nueva.
4. Agregue el archivo mediante la opción disponible en Copilot Chat.

---

## Paso 1: Confirmar el alcance del archivo

### Objetivo

Comprobar que la herramienta puede trabajar con el archivo y delimitar la fuente.

### Instrucciones

1. Adjunte el archivo.
2. Envíe:

```text
Trabaja únicamente con el archivo que acabo de agregar.

Primero indícame:
- qué tipo de información contiene;
- cuáles son sus secciones principales;
- qué preguntas sí podrías responder a partir de este archivo;
- qué tipo de preguntas no podrías responder sin información adicional.

No respondas con conocimiento externo.
```

### Salida Esperada

Una descripción general del documento y límites razonables de consulta.

### Verificación

- La descripción coincide con el archivo.
- No aparecen secciones inexistentes.
- La herramienta reconoce límites.

---

## Paso 2: Extraer información puntual

### Objetivo

Pedir datos específicos sin interpretación excesiva.

### Instrucciones

Formule entre tres y cinco preguntas basadas en el archivo, por ejemplo:

```text
Extrae las tres decisiones principales documentadas en el archivo.
Para cada una indica la sección o fragmento que la sustenta.
```

```text
¿Qué fechas aparecen explícitamente y a qué evento corresponde cada una?
No infieras fechas que no estén escritas.
```

```text
¿Qué pendientes están expresados de forma explícita?
Separa “pendiente” de “sugerencia”.
```

### Salida Esperada

Respuestas puntuales acompañadas de soporte identificable en el contenido.

### Verificación

- Los datos aparecen realmente en el archivo.
- No se confunden sugerencias con hechos.

---

## Paso 3: Hacer una pregunta que exceda la fuente

### Objetivo

Observar si la herramienta reconoce una falta de evidencia.

### Instrucciones

1. Formule una pregunta cuya respuesta no esté en el archivo:

```text
Con base únicamente en este archivo, dime cuál será el resultado financiero exacto del próximo trimestre.
```

2. Si la herramienta intenta responder, pida:

```text
Indica exactamente qué fragmentos del archivo sustentan esa conclusión.
Si el archivo no contiene evidencia suficiente, responde “No sustentado por la fuente”.
```

### Salida Esperada

La herramienta debe reconocer que el archivo no permite calcular o afirmar el resultado financiero exacto.

### Verificación

- El participante identifica una respuesta no sustentada si aparece.
- La segunda instrucción obliga a delimitar la evidencia.

---

## Paso 4: Crear una regla de consulta basada en evidencia

### Objetivo

Establecer un patrón reutilizable.

### Instrucciones

Guarde este bloque:

```text
Utiliza únicamente el archivo proporcionado.

Para cada afirmación importante:
1. indica la evidencia que la respalda;
2. diferencia hechos de inferencias;
3. si la fuente no contiene información suficiente, dilo explícitamente;
4. no completes vacíos con conocimiento externo.
```

### Salida Esperada

Un prompt reusable para trabajar con archivos de forma más controlada.

### Verificación

- El patrón exige soporte.
- El patrón contempla falta de evidencia.
- Puede reutilizarse con otros archivos autorizados.

---
