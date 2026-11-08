# Sala IA: una entrada sencilla a modelos locales

[Volver a NÉMESIS](../README.md).

La Sala reúne conversación individual, coordinación doble y un antecedente elegido por proyecto. La versión presentada es **Sala Chat UI R002 con interfaz simplificada R001**; la primera prueba individual práctica se hizo enR001. Los documentos conservan esas versiones, sin presentar todos los resultados como un único ensayo.

## Conversación individual

Eliges un modelo, escribes tu pregunta y recibes su respuesta. Puedes continuar en el mismo chat.

El usuario elige un modelo y envía su mensaje. Las pruebas inicialesC01 registraron respuestas de Qwen3.5 4B y Gemma3 4B. C02 comprobó cinco turnos relacionados con datos y correcciones en casos ficticios, con versiones y salvedades diferenciadas. No son pruebas de calidad universal.

En la prueba prácticaC05 se recibió una respuesta individual de Gemma4E2B. La captura de esta muestra enseña el aspecto de la Sala posterior, no esa respuesta concreta.

## Conversación doble

Gemma 4 E2B prepara la respuesta, Granite 3.3 8B la revisa y Gemma puede ajustarla. Cuando el recorrido se completa, recibes una sola respuesta. No se alternan automáticamente los modelos entre mensajes.

El cierreC03 acepta la integración técnica: transmitir pregunta y contexto, coordinar las etapas y devolver el resultado con gestión de fallos. Los errores de razonamiento de los modelos se evalúan como tales, sin exigir infalibilidad a la integración.

En C05 hubo tres solicitudes HTTP200 y una publicación final. Su contenido fue insuficiente: no realizó la comparación/recomendación pedida y solicitó datos presentes. Se conserva ese resultado, sin mostrar una respuesta retocada como si fuera del modelo.

## Memoria del proyecto

Tú eliges un mensaje tuyo para conservar. La Sala lo recupera automáticamente en otra conversación del mismo proyecto y muestra su origen.

**Tú eliges qué recordar. La Sala lo recupera para tu proyecto.**

Después de recibir una respuesta, el usuario puede elegir **su propio mensaje** mediante «Recordar para este proyecto». Se conserva ese USER original, con procedencia. Otra conversación del mismo proyecto lo recupera automáticamente como dato de contexto.

En la muestra práctica, el antecedente sobre una reunión permitió identificar seis personas y la mañana en otro chat individual. Otro proyecto mostró «Sin recuerdo» en el panel; ese negativo fue solo de interfaz, sin pregunta nueva al modelo.

Hay un antecedente activo por proyecto, máximo500 caracteres y hasta256 registros históricos. El guardado es elegido, no ocurre por cada turno. El recuerdo está en disco; la lista de chats de la ventana permanece enRAM. Una huella no certifica que lo guardado sea verdadero.

## Alcance aceptado

C05 recoge la aceptación práctica de claridad y utilidad de la interfaz, en el alcance probado y con las limitaciones de los modelos registradas. No certifica toda conversación doble, otras capacidades futuras o memoria semántica general.

[Respaldo y fechas](evidencia-y-alcance.md) · [Avances y pendientes](avance-y-pendientes.md).
