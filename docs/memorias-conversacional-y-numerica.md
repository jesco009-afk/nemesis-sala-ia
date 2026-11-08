# Memorias conversacional y numérica

Documentación original de **Jean y equipo NÉMESIS** · **[CC BY 4.0](https://github.com/jesco009-afk/nemesis-sala-ia/blob/main/LICENSE.txt)**.

[Volver a NÉMESIS](https://github.com/jesco009-afk/nemesis-sala-ia).

NÉMESIS conserva información mediante dos recorridos. Uno permite volver a usar un mensaje que elegiste; el otro conserva resultados del cálculo aceptado. La memoria pertenece al sistema y se entrega como contexto identificado: no significa que los modelos aprendan permanentemente cada conversación.

## Dos memorias con reglas diferentes

| | Conversacional | Numérica |
| --- | --- | --- |
| **Para qué sirve** | Reutilizar un antecedente elegido para un proyecto. | Conservar un resultado del recorrido de cálculo aceptado. |
| **Qué guarda** | Un mensaje original del usuario y su procedencia. | Operación, operandos, resultado, veredictos y referencias al contrato y a los recibos. |
| **Cómo se guarda** | Tú lo eliges con **Recordar para este proyecto**. | Automáticamente dentro del recorrido numérico probado, después de sus controles de aceptación. |
| **Cómo se recupera** | En otra conversación del mismo proyecto, con su origen. | Por identidad de operación, operandos, tarea y contrato. |
| **Qué no sustituye** | Guardar un antecedente no conserva automáticamente todo el historial. | Recuperar un resultado no demuestra un cálculo nuevo. |

## Un antecedente disponible en otra conversación

En la prueba práctica del **7 de noviembre de 2026**, el usuario eligió guardar su propio mensaje sobre una reunión para **seis personas por la mañana**. Otro chat individual de Sala R002, con **Gemma 4 E2B**, recibió ese antecedente con su origen y respondió identificando ambos datos.

> **Elegir el mensaje** → **Guardar por proyecto** → **Recuperar en otro chat** → **Entregar contexto con origen**.

El sistema conservó el mensaje original del usuario, no una respuesta del modelo. En la versión documentada admite **un antecedente activo por proyecto, hasta 500 caracteres y hasta 256 registros históricos**. Un guardado posterior sustituye el antecedente activo y conserva el histórico.

El antecedente se conserva en disco. La lista de chats de la ventana permanece en RAM: son persistencias diferentes. Los nombres equivalentes normalizados comparten memoria por proyecto; el nombre no se presenta como una frontera universal de seguridad.

Otro proyecto sin antecedente mostró **«Sin recuerdo»** en el panel. Esa comprobación fue de interfaz, sin una pregunta nueva al modelo; no demuestra qué habría respondido sin contexto.

La recuperación práctica descrita fue **individual**. Las pruebas técnicas anteriores incluyeron transporte simulado y un ensayo doble limitado; no se presentan como una recuperación real integral demostrada con ambos modelos.

## Un resultado calculado que puede recuperarse

El **6 de noviembre de 2026**, la ruta numérica AUTO documentó **SUMAR 23 + 16 = 39**, con Ollama **0.40.15**:

1. Recuperó un resultado anterior de esa operación y lo identificó como **histórico**, separado del resultado actual.
2. Después de la propuesta de Qwen, la revisión de Gemma y la aceptación estática de ORÁCULO, el motor registró **un cálculo nuevo: 39, de tipo entero**.
3. El flujo guardó **un resultado nuevo**, enlazado con su contrato, veredictos, recibo del motor y huellas de integridad.
4. Dos lecturas posteriores recuperaron registros y una precarga posterior eligió el nuevo. Esas lecturas **no generaron respuestas ni recalcularon**.

> **Recuperar un antecedente histórico** → **Calcular de nuevo** → **Guardar el resultado nuevo** → **Recuperarlo después**.

La recuperación usa la identidad del caso, no una búsqueda por parecido textual. Este guardado automático pertenece al recorrido numérico probado; no convierte cada respuesta del chat o cada error en un resultado aceptado.

## Alcance de lo demostrado

La memoria conversacional no guarda automáticamente todos los turnos. La numérica mostrada corresponde al caso 23 y 16, no a todos los operandos o condiciones. Ninguna de estas pruebas demuestra una memoria única universal o búsqueda semántica de todos los documentos.

Entregar un antecedente como contexto no demuestra cuánto influyó en el modelo ni garantiza una respuesta correcta. Una huella ayuda a cotejar integridad; no convierte lo guardado en verdad. Las copias de evidencia conservadas en el mismo PC tampoco constituyen por sí solas un respaldo externo.

Respaldo: **C04 INF-000381 / REG-000660** y **C05 INF-000383 / REG-000662** para la memoria conversacional; **INF-000352 / REG-000631** para la numérica. Son evidencias históricas; esta presentación no ejecuta nuevas consultas o cálculos.

[Conversación en Sala](https://github.com/jesco009-afk/nemesis-sala-ia/blob/main/docs/sala-ia.md) · [ORÁCULO y motor](https://github.com/jesco009-afk/nemesis-sala-ia/blob/main/docs/oraculo-y-motor-de-calculo.md) · [Evidencia y alcance](https://github.com/jesco009-afk/nemesis-sala-ia/blob/main/docs/evidencia-y-alcance.md) · [Licencia y atribución](https://github.com/jesco009-afk/nemesis-sala-ia/blob/main/AVISOS.md).
