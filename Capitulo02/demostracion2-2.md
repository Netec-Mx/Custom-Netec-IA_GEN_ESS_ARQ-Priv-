# Demostración guiada 2.2. Experimento controlado: resolver una misma tarea con zero-shot, one-shot y few-shot; imponer formatos y restricciones y comparar los resultados

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 42 minutos |
| Tipo | Demostración guiada |
| Nivel | Intermedio |

## Descripción General

Resolverás una misma tarea con zero-shot, one-shot y few-shot para observar cuándo los ejemplos ayudan realmente.

## Objetivos de Aprendizaje

- diferenciar las tres técnicas;
- usar ejemplos para orientar formato;
- decidir cuándo un ejemplo aporta valor.

## Prerrequisitos

Conocimiento básico de prompting.

### Acceso Requerido

Microsoft 365 Copilot Chat.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

Utiliza este escenario:

```text
Incidencia: retraso en entrega de reporte mensual.
Impacto: el comité no contará con la versión final.
Estado: análisis completado; falta validar dos cifras.
Acción siguiente: revisión con Finanzas.
```

---

## Paso 1: Zero-shot

### Objetivo

Resolver sin ejemplos.

### Instrucciones

Envía:

```text
Convierte la información en una actualización ejecutiva.

Formato:
- Situación
- Impacto
- Estado
- Siguiente acción

Máximo 80 palabras.
No inventes responsables, fechas ni cifras.
```

### Salida Esperada

Una actualización con las cuatro secciones.

### Verificación

- Respeta el formato.
- No agrega datos.

---

## Paso 2: One-shot

### Objetivo

Usar un ejemplo como patrón.

### Instrucciones

Añade:

```text
Ejemplo:

Situación: El proveedor entregó parcialmente la documentación.
Impacto: La validación no puede cerrarse.
Estado: Se revisó la información disponible.
Siguiente acción: Confirmar los documentos faltantes.

Usa este ejemplo únicamente como patrón de estructura.
No copies sus hechos.
```

### Salida Esperada

Una salida más consistente en estructura.

### Verificación

- No copia hechos del ejemplo.

---

## Paso 3: Few-shot

### Objetivo

Usar varios ejemplos para reforzar consistencia.

### Instrucciones

Añade dos ejemplos más y pide:

```text
Usa los ejemplos solo como patrón.

Genera la actualización del caso original con:
- una frase por sección;
- lenguaje ejecutivo;
- máximo 70 palabras.
```

### Salida Esperada

Una respuesta consistente.

### Verificación

- Mantiene el formato.
- No transfiere hechos de otros ejemplos.

---

## Paso 4: Comparar

### Objetivo

Decidir qué técnica conviene.

### Instrucciones

Compara A, B y C:

| Criterio | A | B | C |
|---|---|---|---|
| Formato correcto | | | |
| Tono consistente | | | |
| Información sustentada | | | |
| Supuestos | | | |

### Salida Esperada

Una conclusión basada en el tipo de tarea.

### Verificación

- Puedes explicar cuándo usar zero-shot, one-shot o few-shot.

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
