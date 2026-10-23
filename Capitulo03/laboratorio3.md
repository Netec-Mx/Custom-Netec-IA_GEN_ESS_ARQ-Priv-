# Laboratorio 3. Usa Microsoft 365 Copilot evaluando y probando cada una de sus capacidades

## Descripción General

Usa Microsoft 365 Copilot evaluando y probando cada una de sus capacidades
---

## Paso 1: Generar la investigación base

1. Ingresa a `https://m365.cloud.microsoft`

2. Envía el siguiente prompt:

```
Realiza una investigación completa sobre los fundamentos de la Inteligencia Artificial Generativa (IA Gen). El objetivo es explicar de manera clara y técnica sus principios básicos, incluyendo conceptos clave, procesos de entrenamiento y aplicaciones prácticas. El contexto es un curso de formación para profesionales de TI que necesitan comprender cómo la IA Gen se diferencia del aprendizaje automático tradicional y de los sistemas basados en reglas. Utiliza fuentes confiables como documentación académica, artículos técnicos, papers recientes, blogs especializados en IA y publicaciones oficiales de proveedores de nube (Microsoft, AWS, Google). El formato de salida debe incluir:

Un resumen ejecutivo en 4–5 párrafos claros y estructurados.

Una lista con los 10 conceptos fundamentales (ejemplo: LLM, prompting, RLHF, alucinaciones, RAG, etc.).

Una tabla comparativa entre IA Generativa, ML tradicional y sistemas basados en reglas.

Un ejemplo práctico breve (máx. 5 líneas) de un caso de uso empresarial.
```

3. Observa el resultado.

4. Guarda el prompt para reutilizarlo después con otros temas. Hazlo pasando el curso sobre el prompt enviado y haciendo clic en la opción identificada con el ícono de la etiqueta 🔖 (Guardar Indicación).

5. Al final de la respuesta haz clic en los tres puntos horizontales (...), luego en **Editar en Pages** y finalmente en **Agregar a la nueva página**.

---

## Paso 2: Trabaja con Copilot Pages y Notebooks

1. En Pages, solicita a Copilot del lado izquierdo que reestructure el documento.

```
Reestructura la investigación sobre los fundamentos de la Inteligencia Artificial Generativa (IA Gen) en formato de ensayo académico. El objetivo es transformar el contenido previamente generado (resumen ejecutivo, lista de conceptos, tabla comparativa y ejemplo práctico) en un texto cohesivo y narrativo. El contexto es un curso de formación para profesionales de TI, por lo que el ensayo debe mantener un tono técnico, claro y didáctico. Utiliza fuentes confiables como documentación académica, artículos técnicos, papers recientes y publicaciones oficiales de proveedores de nube (Microsoft, AWS, Google). El formato de salida debe ser un ensayo estructurado con:

Introducción que presente la relevancia de la IA Gen.

Desarrollo que explique los fundamentos, conceptos clave y comparaciones con otros paradigmas.

Inclusión fluida de los 10 conceptos fundamentales dentro del cuerpo del texto.

Integración narrativa de la tabla comparativa en forma de explicación textual.

Ejemplo práctico empresarial como ilustración dentro del desarrollo.

Conclusión que sintetice los aportes y perspectivas futuras de la IA Gen.
```

2. Observa el cambio y el resultado. Haz clic en los tres puntos horizontales del costado superior derecho (...) y luego en **Versión anterior**.

3. Deberías ver la estructura inmediatamente anterior. Decides que estaba mejor antes, por lo cual haces clic en el botón **Restaurar**.

4. Elimina manualmente todo lo que no corresponde al documento, como los comentarios de Copilot.

5. Cuando esté listo, haz clic nuevamente en los tres puntos horizontales del costado superior derecho (...) y luego en **Ingresar al bloc de notas**

6. Recuerda que los Notebooks en Copilot se usan para agregar contenido de diferentes fuentes en un mismo lugar.

7. En la ventana emergente haz clic en **Nuevo bloc de notas**.

8. Se abrirá una nueva pestaña donde te pedirá la creación del Notebook. Sólo agrega el título **Investigación IA Gen** y haz clic en **Crear**.

9. Regresa a la pestaña anterior y nuevamente selecciona a **Ingresar al bloc de notas** como lo hiciste en el punto 5 de este ejercicio.

10. Agrega la página al Notebook **Investigación IA Gen** que acabas de crear.

11. Dirígete a tus cuadernos desde el menú izquierdo.

12. Abre el Notebook que creaste previamente.

13. Del costado derecho verás la página que acabaste de crear.

14. En la parte central aparece el espacio para consultar a Copilot, úsala para enviar el siguiente prompt:

``` 
¿Para mi cargo/rol en la empresa, cuáles son los principales beneficios de usar IA Gen?
```

15. Copilot contestará, y la respuesta quedará almacenada en el historial del chat.

16. (Opcional) Si tu empresa te ha compartido algún documento acerca del buen uso de la IA Gen y/o Copilot, agrégalo al cuaderno haciendo clic en **📎 Agregar referencias** ubicado en el costado derecho de ty Notebook.

17. Finalmente, haz clic en el botón **Infografía** del costado derecho.

18. Observa el resultado de la infografía.

## Paso 3: Trabajar con Agentes en Copilot

1. Selecciona **Agentes** del costado izquierdo y luego en **Nuevo agente**.

2. En la nueva página selecciona la plantilla **Asesor de aprendizaje de IA** en el costado inferior.

3. Observa que todos los campos se completan.

4. Lee la sección **Instrucciones**. Posiblemente requiera algunos cambios de acuerdo a tu criterio, puedes hacerlos libremente. Para hacerlo debes hacer clic en el ícono del lápiz en esta sección.

5. En la sección **Conocimiento**, sólo estará disponible fuente de web (esto depende de la licencia que estemos usando).

6. Haz clic en **+ Agregar conocimiento** y agrega ```https://support.microsoft.com/es-es/microsoft-365-copilot/learning/changes-microsoft-copilot-app``` y luego en **+** del frente.

7. Del costado superior haz clic en **Configuración** y cambia a **Vista previa**

8. Haz la siguiente consulta: ```¿Qué es SAP?```.

9. Observa que el agente devuelve la respuesta, esto no debería ser así. Regresa a la configuración haciendo clic en **Vista previa** del costado superior y cambiando a **Configuración**.

10. Dirígete a la sección **Instrucciones**, haz clic en el ícono del lápiz para editarlo. Busca en las instrucciones las restricciones, de no existir puedes agregar la sección tú:

```
## Restricciones
- **Fuera del ámbito:** Si alguien pregunta algo diferente al propósito principal que es aprendizaje en IA, responderás: "Lo siento, no puedo ayudarte"*
```

11. Regresa a la **Vista previa** como lo hiciste en el punto 7 de este ejercicio.

12. Vuelve a preguntar algo fuera del contexto, por ejemplo: `¿Existen los extraterrestres?`

13. Observa la respuesta.

14. Haz clic en **+ Nuevo chat** y selecciona uno de los prompts sugeridos que aparecen al inicio. Recuerda que estos los puedes agregar, quitar o editar desde la vista de configuración.


**¡Felicitaciones!** 🥳 Has terminado tu laboratorio correctamente. 

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
