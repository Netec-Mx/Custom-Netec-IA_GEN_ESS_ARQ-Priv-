# Demostración guiada 3.1. Cadena de transformación: partir de un texto fuente y producir resumen ejecutivo, correo, tabla y lista de acciones, verificando que no se agreguen hechos no sustentados

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 35 minutos |
| Tipo | Demostración guiada |
| Nivel | Intermedio |

## Descripción General

Transformarás una misma fuente en varios formatos sin cambiar los hechos.

## Objetivos de Aprendizaje

- resumir;
- adaptar a otra audiencia;
- estructurar en tabla;
- extraer acciones;
- validar contra fuente.

## Prerrequisitos

Prompting estructurado.

### Acceso Requerido

Microsoft 365 Copilot Chat.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

Usa este texto:

```text
Durante la revisión mensual se confirmó que 18 de 20 actividades fueron completadas. Dos validaciones siguen abiertas. La capacitación se realizó con 24 participantes. Se identificaron tres dudas recurrentes. El equipo acordó preparar una guía de preguntas frecuentes. La fecha de cierre no está confirmada.
```

---

## Paso 1: Crear un resumen ejecutivo

### Objetivo

Reducir la información sin perder hechos.

### Instrucciones

Envía:

```text
Resume el texto para un gerente.

Incluye:
- avance;
- pendiente;
- hecho relevante;
- información no confirmada.

Máximo 100 palabras.
```

### Salida Esperada

Resumen sustentado.

### Verificación

- No inventa fechas.

---

## Paso 2: Convertir en correo

### Objetivo

Cambiar formato sin cambiar hechos.

### Instrucciones

Envía:

```text
Convierte el resumen en un correo interno.

Incluye:
- asunto;
- avances;
- pendientes;
- cierre.

No agregues compromisos ni responsables.
```

### Salida Esperada

Correo breve.

### Verificación

- Conserva los mismos hechos.

---

## Paso 3: Transformar en tabla

### Objetivo

Organizar para revisión rápida.

### Instrucciones

Envía:

```text
Crea una tabla:
Elemento | Estado | Evidencia | Requiere seguimiento
```

### Salida Esperada

Tabla basada en la fuente.

### Verificación

- Cada fila puede rastrearse al texto original.

---

## Paso 4: Extraer acciones

### Objetivo

Distinguir acciones explícitas de sugerencias.

### Instrucciones

Envía:

```text
Extrae únicamente las acciones explícitas.
No propongas acciones nuevas.
```

### Salida Esperada

Lista de acciones reales.

### Verificación

- No aparecen recomendaciones inventadas.

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
