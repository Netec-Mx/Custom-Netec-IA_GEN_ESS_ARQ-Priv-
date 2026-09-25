# Demostración guiada 1.1. Primera conversación controlada: recorrer Microsoft 365 Copilot Chat (Licenciamiento Básico), formular una necesidad de negocio, probar una respuesta y marcar qué partes requieren verificación.

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 32 minutos |
| Tipo de actividad | Demostración guiada |
| Tecnología | Microsoft 365 Copilot Chat (Licenciamiento Básico) |
| Nivel | Básico |

## Descripción General

En esta actividad realizarás una primera conversación controlada con Microsoft 365 Copilot Chat. Aprenderás a formular una necesidad de negocio, observar cómo responde la herramienta y distinguir qué partes de la respuesta puedes utilizar y cuáles debes verificar antes de usarlas.

## Objetivos de Aprendizaje

Al finalizar podrás:

- formular una solicitud de negocio clara;
- reconocer cuándo una solicitud es demasiado vaga;
- revisar la respuesta generada;
- identificar información que requiere validación;
- aplicar el principio: **pedir → revisar → verificar → refinar**.

## Prerrequisitos

### Conocimiento Requerido

| Concepto | Nivel |
|---|---|
| Uso básico de navegador | Básico |
| Redacción de instrucciones | Básico |
| Revisión de información de trabajo | Básico |

### Acceso Requerido

- Cuenta corporativa con Microsoft 365 Copilot Chat.
- Navegador web.
- Conexión a Internet.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador web y conexión estable a Internet.

### Software Requerido

| Software / servicio | Requisito |
|---|---|
| Microsoft 365 Copilot Chat | Licenciamiento Básico |
| Navegador web | Requerido |

### Configuración Inicial

1. Inicia sesión con tu cuenta corporativa.
2. Abre Microsoft 365 Copilot Chat.
3. Inicia una conversación nueva.
4. Ten disponible un bloc de notas para registrar observaciones.

---

## Paso 1: Identificar una necesidad de negocio

### Objetivo

Reconocer qué información necesita Copilot para ayudarte de forma útil.

### Instrucciones

1. Escribe esta solicitud:

```text
Ayúdame con mi reporte semanal.
```

2. Observa la respuesta.
3. Identifica qué información tuvo que asumir la herramienta.
4. Anota al menos tres datos que faltan, por ejemplo:
   - audiencia;
   - objetivo;
   - información disponible;
   - formato esperado;
   - restricciones.

### Salida Esperada

Debes observar que la respuesta es genérica y depende de supuestos.

### Verificación

- Identificaste al menos tres datos faltantes.
- Puedes explicar por qué la solicitud inicial es ambigua.

---

## Paso 2: Crear una solicitud más controlada

### Objetivo

Mejorar la instrucción añadiendo contexto y restricciones.

### Instrucciones

Utiliza estos datos ficticios:

```text
Actividades de la semana:
- Actualización del inventario: completada.
- Revisión de contratos con proveedores: 8 de 10 revisados.
- Capacitación interna: reprogramada para el jueves siguiente.
- Incidencias operativas: 3 abiertas.
- Presupuesto del área: revisión preliminar terminada; falta aprobación del gerente.
```

Envía este prompt:

```text
Necesito preparar un resumen semanal para mi gerente.

Utiliza únicamente la información proporcionada.

Genera:
- tres avances principales;
- dos pendientes;
- un riesgo;
- acciones para la próxima semana.

Máximo 180 palabras.

No inventes fechas, responsables, montos ni causas que no aparezcan en la información.
```

### Salida Esperada

Una respuesta estructurada con avances, pendientes, riesgo y acciones.

### Verificación

- La respuesta contiene las secciones solicitadas.
- No aparecen datos inexistentes.
- El resultado se basa únicamente en la información proporcionada.

---

## Paso 3: Verificar la respuesta

### Objetivo

Distinguir hechos, inferencias y afirmaciones no sustentadas.

### Instrucciones

Envía:

```text
Revisa tu respuesta anterior contra la información proporcionada.

Clasifica cada afirmación importante como:
- Sustentada directamente.
- Inferida.
- No sustentada.

Para cada una indica qué dato la respalda.
```

Después envía:

```text
Reescribe el resumen eliminando cualquier afirmación no sustentada.
```

### Salida Esperada

Una versión más controlada y verificable.

### Verificación

- Las afirmaciones importantes están respaldadas.
- Las inferencias están claramente diferenciadas.
- No quedan datos inventados.

---

## Validación y Pruebas

Realiza estas verificaciones finales antes de considerar terminada la actividad:

- [ ] Completaste todos los pasos de la actividad.
- [ ] Puedes diferenciar información proporcionada, inferencias y contenido no sustentado.
- [ ] No utilizaste datos sensibles reales durante la práctica.
- [ ] Aplicaste revisión humana antes de considerar válido el resultado.
- [ ] Puedes explicar qué información debe verificarse antes de reutilizar una respuesta.

Si alguna comprobación no se cumple, vuelve al paso correspondiente y corrige el resultado antes de continuar.

---

## Solución de Problemas

### Problema 1: La respuesta es demasiado genérica

**Síntoma:** La respuesta es demasiado genérica.

**Causa probable:** Falta contexto, audiencia, formato o restricciones.

**Solución:** Agrega esos elementos y vuelve a ejecutar el prompt.
### Problema 2: Copilot agrega información que no proporcionaste

**Síntoma:** Copilot agrega información que no proporcionaste.

**Causa probable:** La fuente no quedó suficientemente delimitada.

**Solución:** Añade: “Utiliza únicamente la información proporcionada. Si falta un dato, indícalo”.
### Problema 3: No sabes si una solicitud es segura

**Síntoma:** No sabes si una solicitud es segura.

**Causa probable:** Falta contexto sobre sensibilidad o políticas internas.

**Solución:** Minimiza los datos, utiliza marcadores y valida la política de tu organización antes de continuar.

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
| Necesidad | Definiste una tarea concreta. |
| Interacción | Probaste y refinaste una solicitud. |
| Riesgo | Evaluaste qué información puede utilizarse. |
| Verificación | Revisaste la respuesta antes de usarla. |

### Conceptos Clave Reforzados

- Una respuesta convincente no equivale a una respuesta correcta.
- Minimizar datos reduce exposición sin eliminar necesariamente la utilidad.
- Las inferencias deben distinguirse de los hechos.
- La revisión humana forma parte del uso responsable de IA generativa.

### Recursos Adicionales

- [Introducción a Microsoft Copilot Chat](https://support.microsoft.com/es-es/microsoft-365-copilot/get-started-with-microsoft-365-copilot-chat)
- [Cómo escribir mejores prompts en Microsoft Copilot](https://support.microsoft.com/en-us/microsoft-365-copilot/write-a-great-prompt-in-microsoft-365-copilot)
