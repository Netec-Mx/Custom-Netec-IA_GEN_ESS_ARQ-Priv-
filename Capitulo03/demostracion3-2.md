# Demostración guiada 3.2. Reto de evidencia con archivos: cargar un archivo proporcionado, extraer datos, hacer preguntas, solicitar soporte en la fuente y detectar respuestas no sustentadas

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 45 minutos |
| Tipo | Demostración guiada |
| Nivel | Intermedio |

## Descripción General

Trabajarás con un archivo proporcionado y aprenderás a pedir evidencia.

## Objetivos de Aprendizaje

- cargar un archivo;
- extraer información;
- pedir soporte;
- detectar respuestas no sustentadas.

## Prerrequisitos

Uso básico de archivos y prompting.

### Acceso Requerido

Archivo de práctica y Microsoft 365 Copilot Chat.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

Adjunta el archivo proporcionado.

---

## Paso 1: Delimitar la fuente

### Objetivo

Entender qué contiene el archivo.

### Instrucciones

Envía:

```text
Trabaja únicamente con el archivo.

Indícame:
- qué información contiene;
- sus secciones principales;
- qué preguntas puedes responder;
- qué preguntas no puedes responder.
```

### Salida Esperada

Descripción del alcance.

### Verificación

- No aparecen secciones inexistentes.

---

## Paso 2: Extraer datos

### Objetivo

Obtener hechos puntuales.

### Instrucciones

Prueba:

```text
Extrae las tres decisiones principales.
Indica qué parte de la fuente las sustenta.
```

### Salida Esperada

Hechos acompañados de evidencia.

### Verificación

- Los datos aparecen en el archivo.

---

## Paso 3: Probar los límites

### Objetivo

Detectar falta de evidencia.

### Instrucciones

Pregunta algo que no esté en el archivo y después envía:

```text
Indica qué fragmento sustenta esa conclusión.
Si no existe evidencia suficiente, responde:
“No sustentado por la fuente”.
```

### Salida Esperada

Reconocimiento del límite.

### Verificación

- Puedes identificar una respuesta no sustentada.

---

## Paso 4: Guardar un patrón reusable

### Objetivo

Crear una regla de trabajo.

### Instrucciones

Guarda:

```text
Utiliza únicamente el archivo proporcionado.
Para cada afirmación:
1. indica evidencia;
2. diferencia hechos de inferencias;
3. reconoce falta de información;
4. no completes vacíos con conocimiento externo.
```

### Salida Esperada

Prompt reusable.

### Verificación

- El patrón obliga a pedir evidencia.

---

## Validación y Pruebas

Realiza estas verificaciones finales antes de considerar terminada la actividad:

- [ ] Completaste todos los pasos de la actividad.
- [ ] La salida se basa únicamente en la fuente o archivo utilizado.
- [ ] Puedes localizar evidencia para las afirmaciones importantes.
- [ ] Diferenciaste hechos de inferencias.
- [ ] Eliminaste o corregiste cualquier afirmación no sustentada.

Si alguna comprobación no se cumple, vuelve al paso correspondiente y corrige el resultado antes de continuar.

---

## Solución de Problemas

### Problema 1: No puedes agregar el archivo

**Síntoma:** No puedes agregar el archivo.

**Causa probable:** La opción puede depender de la cuenta, formato o configuración.

**Solución:** Verifica tu cuenta y utiliza el archivo de práctica compatible proporcionado para la actividad.
### Problema 2: Copilot responde con información externa

**Síntoma:** Copilot responde con información externa.

**Causa probable:** La fuente no se delimitó.

**Solución:** Comienza el prompt con: “Trabaja únicamente con el archivo proporcionado”.
### Problema 3: La evidencia indicada no coincide con la fuente

**Síntoma:** La evidencia indicada no coincide con la fuente.

**Causa probable:** La autoevaluación de Copilot también puede contener errores.

**Solución:** Comprueba manualmente el fragmento y marca la afirmación como no verificada si no encuentras soporte.

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
| Fuente | Trabajaste con información delimitada. |
| Transformación | Generaste una salida a partir de esa fuente. |
| Evidencia | Pediste soporte para las afirmaciones. |
| Auditoría | Validaste el resultado contra la información original. |

### Conceptos Clave Reforzados

- La fuente original sigue siendo el criterio principal de validación.
- Transformar un contenido no autoriza a modificar sus hechos.
- Reconocer que falta información es mejor que completar vacíos sin evidencia.
- Adjuntar un archivo no elimina la necesidad de revisar las respuestas.

### Recursos Adicionales

- [Agregar contenido a prompts de Microsoft Copilot Chat](https://support.microsoft.com/es-es/microsoft-365-copilot/add-content-to-microsoft-365-copilot-chat-prompts)
- [Formatos de archivo compatibles con Microsoft Copilot](https://support.microsoft.com/en-us/microsoft-365-copilot/file-formats-supported-by-microsoft-365-copilot)
