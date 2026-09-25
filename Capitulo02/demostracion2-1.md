# Demostración guiada 2.1. Anatomía del prompt: convertir solicitudes vagas en prompts estructurados y comparar cómo cambia la calidad, precisión y formato de la respuesta

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 35 minutos |
| Tipo | Demostración guiada |
| Nivel | Básico–intermedio |

## Descripción General

Aprenderás a convertir una solicitud vaga en un prompt estructurado y a observar cómo cambia la calidad de la respuesta.

## Objetivos de Aprendizaje

- reconocer los componentes de un buen prompt;
- reducir ambigüedad;
- controlar formato y tono;
- limitar supuestos.

## Prerrequisitos

Uso básico de Copilot Chat.

### Acceso Requerido

Microsoft 365 Copilot Chat.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

Abre una conversación nueva.

---

## Paso 1: Probar una solicitud vaga

### Objetivo

Observar una respuesta genérica.

### Instrucciones

Envía:

```text
Haz un correo sobre el cambio de proceso.
```

Anota qué tuvo que asumir Copilot.

### Salida Esperada

Un correo genérico.

### Verificación

- Detectaste al menos cuatro supuestos.

---

## Paso 2: Estructurar el prompt

### Objetivo

Añadir los elementos que faltan.

### Instrucciones

Envía:

```text
Redacta un correo para comunicar un cambio de proceso.

Objetivo:
Que el personal conozca el nuevo procedimiento.

Audiencia:
Personal administrativo.

Cambio:
A partir de la próxima semana las solicitudes internas deberán registrarse mediante un formulario antes de enviarse a revisión.

Incluye:
- asunto;
- explicación breve;
- tres acciones;
- cierre.

Máximo 170 palabras.

No inventes enlaces, responsables ni fechas.
Tono profesional y claro.
```

### Salida Esperada

Un correo más preciso y útil.

### Verificación

- Tiene asunto.
- Tiene tres acciones.
- No inventa datos.

---

## Paso 3: Comparar resultados

### Objetivo

Identificar mejoras concretas.

### Instrucciones

Envía:

```text
Compara la primera respuesta con la segunda.

Evalúa:
- claridad;
- relevancia;
- precisión;
- adecuación a la audiencia;
- formato;
- supuestos.

No asignes una calificación global.
```

### Salida Esperada

Una comparación basada en criterios.

### Verificación

- Puedes identificar qué componente mejoró cada aspecto.

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
