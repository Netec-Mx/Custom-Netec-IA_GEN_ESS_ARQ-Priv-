# Laboratorio 4. Reto integrador por rol: resolver una tarea real de principio a fin, refinar el prompt, validar fuentes y contenido, aplicar controles de privacidad y guardar el patrón final en una biblioteca personal

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 71 minutos |
| Tipo | Laboratorio integrador |
| Nivel | Intermedio |

## Descripción General

Resolverás una tarea de principio a fin aplicando prompting, validación, privacidad y revisión crítica.

## Objetivos de Aprendizaje

- definir una necesidad;
- construir y refinar un prompt;
- validar contenido;
- aplicar controles de privacidad;
- guardar un patrón reusable.

## Prerrequisitos

Capítulos 1 a 4.

### Acceso Requerido

Microsoft 365 Copilot Chat y material de práctica.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

Selecciona un reto:

| Perfil | Ejemplo |
|---|---|
| Administración | Reporte ejecutivo |
| Comercial | Preparación de reunión |
| Finanzas | Hallazgos y preguntas |
| RR. HH. | Comunicación de política |
| Operaciones | Seguimiento de incidencias |
| Servicio | Resumen de retroalimentación |

---

## Paso 1: Definir el reto

### Objetivo

Establecer qué necesitas resolver.

### Instrucciones

Completa:

```text
Mi rol:
Tarea:
Audiencia:
Resultado final:
Fuente:
Qué no debe hacer Copilot:
Qué revisaré:
```

### Salida Esperada

Definición concreta.

### Verificación

- Existe audiencia.
- Existe fuente.

---

## Paso 2: Revisar privacidad

### Objetivo

Reducir exposición.

### Instrucciones

Antes de enviar información, pregúntate:

- ¿Necesito nombres?
- ¿Necesito importes exactos?
- ¿Puedo usar marcadores?
- ¿Está permitido usar esta información?

Sustituye por:

```text
[CLIENTE]
[PROYECTO]
[PERSONA]
[FECHA]
[IMPORTE]
```

### Salida Esperada

Información preparada con mínimo riesgo.

### Verificación

- No usaste datos sensibles innecesarios.

---

## Paso 3: Crear el prompt

### Objetivo

Construir una primera versión completa.

### Instrucciones

Usa:

```text
Objetivo:
[resultado]

Contexto:
[rol, audiencia y propósito]

Fuente:
[texto o archivo]

Genera:
[formato]

Restricciones:
- usa únicamente la fuente;
- no inventes datos;
- identifica información faltante.
```

### Salida Esperada

Primera respuesta evaluable.

### Verificación

- El prompt define fuente y límites.

---

## Paso 4: Refinar

### Objetivo

Corregir problemas.

### Instrucciones

Prueba según necesites:

```text
Reduce la respuesta y conserva solo elementos sustentados.
```

```text
Adapta el tono para [audiencia] sin cambiar hechos.
```

```text
Señala qué información falta.
```

### Salida Esperada

Versión mejorada.

### Verificación

- Cada refinamiento corrige un problema real.

---

## Paso 5: Validar

### Objetivo

Auditar la respuesta.

### Instrucciones

Envía:

```text
Audita tu respuesta contra la fuente.

Tabla:
Afirmación | Evidencia | Sustentada / Inferida / No sustentada
```

### Salida Esperada

Tabla de validación.

### Verificación

- No quedan afirmaciones no sustentadas.

---

## Paso 6: Revisar críticamente

### Objetivo

Buscar puntos ciegos.

### Instrucciones

Envía:

```text
Revisa el resultado como crítico constructivo.

Identifica:
- un supuesto;
- una pregunta pendiente;
- una ambigüedad;
- una comprobación final humana.

No tomes la decisión por mí.
```

### Salida Esperada

Controles adicionales.

### Verificación

- La decisión sigue siendo tuya.

---

## Paso 7: Guardar el patrón

### Objetivo

Convertir el aprendizaje en un recurso reusable.

### Instrucciones

Documenta:

```text
Nombre:
Cuándo usarlo:
Fuente requerida:
Prompt final:
Variables:
Qué verificar:
Información que nunca debo incluir:
```

### Salida Esperada

Un patrón reutilizable.

### Verificación

- No contiene datos específicos innecesarios.
- Incluye controles de privacidad y revisión.

---

## Validación y Pruebas

Realiza estas verificaciones finales antes de considerar terminada la actividad:

- [ ] Completaste todos los pasos de la actividad.
- [ ] Definiste claramente el escenario o problema.
- [ ] Separaste hechos, supuestos y preguntas abiertas.
- [ ] La herramienta no tomó una decisión final por ti.
- [ ] Aplicaste una revisión crítica antes de cerrar la actividad.

Si alguna comprobación no se cumple, vuelve al paso correspondiente y corrige el resultado antes de continuar.

---

## Solución de Problemas

### Problema 1: Copilot toma una decisión final

**Síntoma:** Copilot toma una decisión final.

**Causa probable:** El prompt permite una conclusión global.

**Solución:** Indica explícitamente que debe analizar, cuestionar o proponer opciones sin decidir.
### Problema 2: Las objeciones o preguntas son genéricas

**Síntoma:** Las objeciones o preguntas son genéricas.

**Causa probable:** Falta contexto suficiente.

**Solución:** Añade propósito, restricciones y antecedentes del escenario.
### Problema 3: Las hipótesis aparecen como hechos

**Síntoma:** Las hipótesis aparecen como hechos.

**Causa probable:** No se solicitó distinguir niveles de certeza.

**Solución:** Pide separar hechos, supuestos, inferencias y preguntas abiertas.

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
| Escenario | Definiste una situación concreta. |
| Análisis | Exploraste preguntas, objeciones o supuestos. |
| Revisión | Evaluaste límites y puntos ciegos. |
| Criterio humano | Mantviste la decisión final bajo responsabilidad humana. |

### Conceptos Clave Reforzados

- Copilot puede ayudar a ampliar perspectivas sin sustituir la decisión humana.
- Los contraargumentos son insumos para investigar, no evidencia.
- Separar hechos de supuestos mejora la calidad del análisis.
- La revisión crítica debe complementar, no reemplazar, el juicio profesional.

### Recursos Adicionales

- [Crear contenido con Microsoft Copilot Chat](https://support.microsoft.com/en-us/microsoft-365-copilot/create-content-using-microsoft-365-copilot-chat)
- [Preguntas frecuentes sobre Microsoft Copilot Chat](https://support.microsoft.com/en-us/microsoft-365-copilot/frequently-asked-questions-about-microsoft-365-copilot-chat)
