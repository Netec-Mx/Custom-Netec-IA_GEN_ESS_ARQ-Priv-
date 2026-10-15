# Laboratorio 2. Clínica de prompts: construir, probar y refinar un conjunto de prompts reutilizables para situaciones reales del trabajo, incorporando criterios de calidad y verificación

## Descripción General

Construirás y refinarás prompts reutilizables para situaciones reales de trabajo.

## Objetivos de Aprendizaje

- construir prompts estructurados;
- añadir restricciones;
- refinar respuestas;
- crear criterios de calidad.

## Prerrequisitos

### Acceso Requerido

Microsoft 365 Copilot Chat y documento de notas.

### Configuración Inicial

Abre un bloc de notas en tu equipo, copia y pega el siguiente contenido. 

```jsonl
{"prompt": "Clasifica el siguiente documento y da una recomendación de tratamiento.\n\nDocumento: 'Informe preliminar de la auditoría fiscal externa 2026, señalando posibles inconsistencias graves en la contabilidad y riesgo inminente de sanción por parte de la DIAN.'", "completion": "{\n  "clasificacion": "Crítico",\n  "recomendacion": "Restringir el acceso exclusivamente al Comité Directivo y equipo legal. Almacenar en repositorio cifrado de extremo a extremo, prohibir su reenvío por correo externo y aplicar destrucción segura tras el cierre del caso."\n}"}
{"prompt": "Clasifica el siguiente documento y da una recomendación de tratamiento.\n\nDocumento: 'Propuesta comercial detallada con tarifas preferenciales y condiciones contractuales exclusivas negociadas para el cliente clave Banco de Bogotá.'", "completion": "{\n  "clasificacion": "Confidencial",\n  "recomendacion": "Compartir únicamente con el equipo comercial asignado y los tomadores de decisiones del cliente. Asegurar el uso de acuerdos de confidencialidad (NDA) vigentes y evitar su almacenamiento en dispositivos personales."\n}"}
{"prompt": "Clasifica el siguiente documento y da una recomendación de tratamiento.\n\nDocumento: 'Cronograma y lineamientos generales para el evento de integración de fin de año de los empleados de la sucursal de Bogotá.'", "completion": "{\n  "clasificacion": "Información interna",\n  "recomendacion": "Distribuir a través de los canales de comunicación interna habituales de la compañía (intranet o correo corporativo). No requiere medidas de cifrado estrictas, pero no debe compartirse con personas ajenas a la organización."\n}"}
{"prompt": "Clasifica el siguiente documento y da una recomendación de tratamiento.\n\nDocumento: 'Nota de prensa oficial anunciando el lanzamiento de nuestra nueva línea eco-amigable de productos disponible para todo público en la web corporativa.'", "completion": "{\n  "clasificacion": "Público",\n  "recomendacion": "Apto para distribución libre y masiva en canales externos, redes sociales y medios de comunicación. No requiere restricciones de acceso ni medidas especiales de protección."\n}"}
```

Luego en el Bloc de Notas haz clic en Archivo - Guardar como... - 

* **Nombre:** ClasificadorDocumentosFewShot.jsonl
* **Tipo:** Todos los archivos (*.*)

---

## Paso 1: Usa las mejores prácticas de Ingeniería de prompt

Imagina que eres un líder de equipo que quiere usar un asistente de IA para preparar material motivacional y organizativo después de terminar un proyecto importante. Al inicio, tu prompt es muy básico, pero progresivamente lo vamos refinando.

Ingresa a Microsoft 365 Copilot en tu navegador `https://m365.cloud.microsoft`

1. Prompt sin contexto. El usuario pide algo genérico, sin dar detalles.

Prompt: `Escribe un mensaje motivador.`

Problema: La IA no sabe para quién, ni en qué situación, ni qué tono usar.

3. Añadir contexto Se especifica quién eres y en qué situación estás.

Prompt: `Soy líder de un equipo que acaba de terminar un proyecto importante. Escribe un mensaje motivador para ellos.`

Mejora: Ahora la IA entiende el rol y el escenario.

4. Definir objetivo. Se aclara qué se busca lograr con el mensaje.

Prompt: `Soy líder de un equipo que acaba de terminar un proyecto importante. Escribe un mensaje motivador para agradecerles y reforzar la confianza en futuros proyectos.`

Mejora: La IA sabe que debe incluir agradecimiento y proyección.

4. Ubicación del contenido. Se indica dónde se usará el resultado (correo, presentación, etc.).

Prompt: `Soy líder de un equipo que acaba de terminar un proyecto importante. Escribe un mensaje motivador para agradecerles y reforzar la confianza en futuros proyectos. El mensaje será enviado por correo electrónico.`

Mejora: La IA ajusta tono y extensión al canal.

5. Tipo de salida. Se define el formato esperado (párrafo, lista, tabla, etc.).

Prompt: `Soy líder de un equipo que acaba de terminar un proyecto importante. Escribe un mensaje motivador para agradecerles y reforzar la confianza en futuros proyectos. El mensaje será enviado por correo electrónico y debe estar en un solo párrafo breve.`

Mejora: La IA entrega exactamente el formato deseado.

✨ **Resultado del ejercicio**
Con este flujo, se ve cómo un prompt pasa de ser ambiguo a ser preciso y útil, gracias a la inclusión progresiva de:

📌 Contexto → quién eres y situación

🎯 Objetivo → qué quieres lograr

🗂️ Ubicación del contenido → dónde se usará

📝 Tipo de salida → formato esperado


## Paso 2: Experimenta one-shot, few-shot y CTO en un escenario empresarial

1. Usemos one-shot. 
---



## Paso 3: Estructurar cada prompt

### Objetivo

Mejorar control.

### Instrucciones

Incluye:
- objetivo;
- contexto;
- fuente;
- formato;
- restricciones;
- tono.

Ejemplo:

```text
Resume este documento para un gerente de operaciones.

Incluye:
- tres hallazgos;
- dos riesgos;
- acciones pendientes.

Máximo 180 palabras.
Usa solo información de la fuente.
```

### Salida Esperada

Tres prompts mejorados.

### Verificación

- Cada uno define formato y límites.

---

## Paso 4: Probar ejemplos

### Objetivo

Determinar si one-shot mejora el resultado.

### Instrucciones

Añade un ejemplo pequeño a uno de tus prompts.

### Salida Esperada

Comparación entre versión con y sin ejemplo.

### Verificación

- Puedes justificar si el ejemplo aportó valor.

---

## Paso 5: Refinar conversacionalmente

### Objetivo

Mejorar sin empezar de cero.

### Instrucciones

Prueba:

```text
Reduce la respuesta a 120 palabras.
```

Después:

```text
Revisa si introdujiste información que no aparezca en la fuente.
```

### Salida Esperada

Una respuesta más controlada.

### Verificación

- El refinamiento corrige problemas reales.

---

## Paso 6: Crear criterios de calidad

### Objetivo

Documentar cuándo una respuesta es aceptable.

### Instrucciones

Completa:

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

### Salida Esperada

Tres prompts reutilizables y verificados.

### Verificación

- Cada prompt tiene criterios de calidad y revisión.

---

## Validación y Pruebas

Realiza estas verificaciones finales antes de considerar terminada la actividad:

- [ ] Completaste todos los pasos de la actividad.
- [ ] Tu prompt define con claridad el objetivo.
- [ ] Incluiste contexto, formato y restricciones cuando fueron necesarios.
- [ ] Comparaste resultados usando criterios concretos.
- [ ] El prompt final puede reutilizarse sin depender excesivamente del historial de la conversación.

Si alguna comprobación no se cumple, vuelve al paso correspondiente y corrige el resultado antes de continuar.

---

## Solución de Problemas

### Problema 1: La respuesta no sigue el formato solicitado

**Síntoma:** La respuesta no sigue el formato solicitado.

**Causa probable:** El formato se expresó de manera ambigua.

**Solución:** Enumera explícitamente las secciones, columnas o elementos que debe contener.
### Problema 2: La respuesta cambia demasiado entre intentos

**Síntoma:** La respuesta cambia demasiado entre intentos.

**Causa probable:** El prompt deja abiertas demasiadas decisiones.

**Solución:** Añade restricciones, prioridades y criterios de salida.
### Problema 3: Los ejemplos contaminan la respuesta

**Síntoma:** Los ejemplos contaminan la respuesta.

**Causa probable:** No quedó claro que son solo un patrón.

**Solución:** Indica que Copilot debe imitar la estructura o el tono, pero no copiar hechos de los ejemplos.

---

## Limpieza

1. Cierra la conversación de práctica si ya no la necesitas.
2. Elimina o evita conservar datos de práctica que no deban reutilizarse.
3. Conserva únicamente prompts, tablas o patrones que puedan reutilizarse de forma segura.
4. Si trabajaste con un archivo proporcionado, sigue las políticas de tu organización para su almacenamiento o eliminación.

> **Nota:** estas actividades no requieren desinstalar software ni eliminar configuraciones del equipo. La limpieza se enfoca en conversaciones, archivos y datos utilizados durante la práctica.

---

## Resumen

| Fase | Logro |
|---|---|
| Solicitud | Partiste de una necesidad de trabajo. |
| Estructura | Añadiste objetivo, contexto, expectativas y fuente. |
| Experimentación | Probaste variantes y refinamientos. |
| Reutilización | Construiste un prompt más consistente. |

### Conceptos Clave Reforzados

- Un prompt útil puede combinar objetivo, contexto, expectativas y fuente.
- Formato y restricciones ayudan a reducir ambigüedad.
- Los ejemplos orientan, pero no siempre son necesarios.
- Un prompt reutilizable debe poder entenderse fuera de la conversación original.

### Recursos Adicionales

- [Introducción a la escritura de prompts en Microsoft Copilot](https://support.microsoft.com/en-us/microsoft-365-copilot/get-started-writing-prompts-in-microsoft-365-copilot)
- [Cómo escribir mejores prompts en Microsoft Copilot](https://support.microsoft.com/en-us/microsoft-365-copilot/write-a-great-prompt-in-microsoft-365-copilot)
