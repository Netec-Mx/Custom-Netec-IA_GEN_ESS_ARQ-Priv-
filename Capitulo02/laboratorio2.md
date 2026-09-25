# Laboratorio 2. Clínica de prompts: construir, probar y refinar un conjunto de prompts reutilizables para situaciones reales del trabajo, incorporando criterios de calidad y verificación

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 76 minutos |
| Tipo | Laboratorio |
| Nivel | Intermedio |

## Descripción General

Construirás y refinarás prompts reutilizables para situaciones reales de trabajo.

## Objetivos de Aprendizaje

- construir prompts estructurados;
- añadir restricciones;
- refinar respuestas;
- crear criterios de calidad.

## Prerrequisitos

Capítulos 1 y 2.

### Acceso Requerido

Microsoft 365 Copilot Chat y documento de notas.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

Crea esta plantilla:

```text
Nombre:
Tarea:
Versión inicial:
Versión estructurada:
Versión refinada:
Criterios de calidad:
Qué debo verificar:
```

---

## Paso 1: Seleccionar tres tareas

### Objetivo

Elegir tareas repetibles.

### Instrucciones

Selecciona tres:
- comunicación;
- resumen;
- análisis;
- comparación;
- ideación.

### Salida Esperada

Tres tareas concretas.

### Verificación

- Cada tarea produce un entregable claro.

---

## Paso 2: Crear la versión inicial

### Objetivo

Registrar tu primera forma de pedir la tarea.

### Instrucciones

Ejemplo:

```text
Resume este reporte.
```

Ejecuta tus tres prompts.

### Salida Esperada

Tres respuestas iniciales.

### Verificación

- Identificaste qué faltó en cada una.

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
