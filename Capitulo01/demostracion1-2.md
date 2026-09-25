# Demostración guiada 1.2. Semáforo de riesgos: clasificar solicitudes seguras, condicionadas y no recomendadas; anonimizar datos y reescribir prompts para reducir exposición.

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 38 minutos |
| Tipo de actividad | Demostración guiada |
| Tecnología | Microsoft 365 Copilot Chat |
| Nivel | Básico |

## Descripción General

En esta actividad aprenderás a clasificar solicitudes según su nivel de riesgo y a reducir la exposición de información mediante anonimización y reformulación de prompts.

## Objetivos de Aprendizaje

- distinguir solicitudes de bajo, medio y alto riesgo;
- identificar datos innecesarios;
- anonimizar información;
- reconocer cuándo detenerte y consultar políticas internas.

## Prerrequisitos

### Conocimiento Requerido

Uso básico de Copilot Chat y criterios básicos de seguridad de la información.

### Acceso Requerido

Microsoft 365 Copilot Chat y navegador web.

## Entorno del Laboratorio

### Hardware Mínimo

Equipo con navegador e Internet.

### Software Requerido

Microsoft 365 Copilot Chat.

### Configuración Inicial

Usarás este semáforo:

- **Verde:** bajo riesgo.
- **Amarillo:** requiere anonimización o revisión.
- **Rojo:** no debe utilizarse sin autorización o implica una decisión que no debe delegarse.

---

## Paso 1: Clasificar tres solicitudes

### Objetivo

Aplicar el semáforo a situaciones reales.

### Instrucciones

Clasifica cada caso:

**Caso A**

```text
Crea cinco asuntos para un correo interno sobre una capacitación.
```

**Caso B**

```text
Mejora este correo de cobranza.
Cliente: Empresa Delta.
Saldo: 248,700.
Contacto: Laura Hernández.
Teléfono: 55-0000-0000.
```

**Caso C**

```text
Analiza esta lista de empleados con salario, evaluación y observaciones médicas e indica quién debería ser despedido.
```

### Salida Esperada

- Caso A: verde.
- Caso B: amarillo.
- Caso C: rojo.

### Verificación

- Puedes justificar cada clasificación.
- Identificaste datos innecesarios en B y C.

---

## Paso 2: Anonimizar una solicitud

### Objetivo

Mantener el objetivo de negocio sin exponer datos reales.

### Instrucciones

Utiliza:

```text
Ayúdame a mejorar la redacción de un correo de seguimiento de cobranza.

Contexto:
- Es un cliente empresarial.
- Existe un saldo vencido.
- Ya se envió un primer recordatorio.

Genera:
- asunto;
- cuerpo del mensaje;
- cierre.

No inventes fechas, compromisos ni importes.
Utiliza los marcadores [CLIENTE], [SALDO] y [FECHA].
```

### Salida Esperada

Un borrador reutilizable sin datos identificables.

### Verificación

- No aparecen nombres reales.
- No aparecen cifras reales.
- El objetivo del mensaje se conserva.

---

## Paso 3: Reformular una solicitud de alto riesgo

### Objetivo

Convertir una solicitud riesgosa en una tarea de apoyo.

### Instrucciones

Utiliza:

```text
Ayúdame a crear criterios neutrales para revisar un proceso de desempeño.

Incluye:
- cumplimiento de objetivos;
- evidencia documentada;
- consistencia;
- acciones de mejora;
- información que debe validar una persona responsable.

No evalúes empleados ni recomiendes decisiones laborales.
```

### Salida Esperada

Una lista de criterios generales, sin decidir sobre personas.

### Verificación

- La herramienta no clasifica empleados.
- La decisión permanece en manos humanas.

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
