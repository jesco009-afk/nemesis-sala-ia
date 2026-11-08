# Conversación y cálculo: recorridos distintos

[Volver a NÉMESIS](../README.md).

## Conversación libre

Sala recibe el mensaje y prepara el contexto para uno o dos modelos. Un antecedente elegido por el usuario puede recuperarse automáticamente dentro del proyecto. El sistema identifica su origen; el modelo lo recibe como dato y puede equivocarse al interpretarlo.

La memoria la conserva el sistema: no supone que los pesos del modelo aprendan permanentemente cada conversación. La coordinación doble no convierte su respuesta en una verificación de ORÁCULO.

## Verificación y cálculo

El ejemplo numérico de **23+16=39** corresponde a una sesión nueva de Sala numéricaAUTO del6nov2026, con Ollama0.40.15. Se distinguen estas evidencias:

1. Qwen propuso un candidatoSUMAR y Gemma lo revisó.
2. El adaptador enlazó candidato, contrato, tarea y sesión.
3. ORÁCULO aceptó mediante **inferencia estática condicionada**, sin errores.
4. El motor registró por separado `CALCULATED`, resultado39 de tipoentero.
5. La transacción guardó un resultado nuevo, con otra identidad que el antecedente histórico.

La API de ORÁCULO no certificó por sí sola la procedencia ni ejecutó el candidato. Aceptar una gramática cerrada no equivale a demostrar la corrección de cualquier programa.

Como contraste, un control aislado histórico presentó una resta sintética donde se exigía suma. La API estática real la rechazó y el instrumento registró parada antes de sus fronteras de cálculo/guardado. Modelos y otras capas eran dobles; no fue un fallo real de un modelo ni una segunda prueba integral de producción.

## Dos memorias

| | Conversacional | Numérica |
| --- | --- | --- |
| Fuente | Mensaje original elegido explícitamente por el usuario. | Resultado del recorrido numérico aceptado y calculado. |
| Guardado | Acción del usuario por proyecto. | Automático en el flujo numérico probado. |
| Recuperación | Automática en otro chat del mismo proyecto. | Por operación, operandos, tarea y contrato. |
| Origen | Dato identificado, sin autoridad para mandar al sistema. | Registro identificado como histórico, distinto del resultado actual. |

En el caso numérico se recuperó un antecedente, se calculó39 de nuevo y se guardó otro resultado. Dos lecturasCLI posteriores recuperaron histórico/nuevo y un prefetch eligió el nuevo. Esas lecturas **no recalcularon** ni generaron nuevas respuestas.

No se promete una memoria única general, recuperación semántica de todos los documentos, persistencia de toda la conversación o influencia causal interna demostrada sobre el modelo. [Fuentes y alcance](evidencia-y-alcance.md).
