# Avance del proyecto y pendientes

[Volver a NÉMESIS](../README.md). Corte:8 de noviembre de2026.

Los avances describen alcances respaldados, no porcentajes globales ni capacidades completas.

| Área | Avance demostrado | Qué queda por desarrollar o comprobar |
| --- | --- | --- |
| **Sala IA** | Conversación individual, coordinación doble, interfaz y memoria por proyecto. | Historial completo persistente y capacidades nuevas. |
| **Orquestador** | Coordinación del recorrido probado, control de contexto y muestra de repetibilidad. | Más rutas, cargas y concurrencia. |
| **ORÁCULO y motor** | Cuatro operaciones aritméticas en casos concretos supervisados. | Otros programas y dominios requieren comprobaciones propias. |
| **Memorias** | Guardado y recuperación según cada recorrido. | Búsqueda semántica y memoria avanzada. |
| **Equipo doméstico** | Pruebas documentadas y GPU con modelos concretos. | Instalación reproducible en otros equipos y mediciones comparables. |
| **Programación y otros usos** | Pruebas iniciales de modelos. | Programación general, imágenes y búsqueda documental. |

## Límites que acompañan lo demostrado

- Los modelos pueden equivocarse. En C05, el recorrido doble se completó, pero la respuesta no hizo la comparación solicitada. Es un límite conocido de contenido, no una exigencia de volver infalibles a los modelos.
- El recorrido externo del Orquestador es SUMAR AUTO/P06; no se extiende automáticamente a las cuatro operaciones. Contexto y repetibilidad conservan el alcance de sus muestras.
- La aceptación estática de ORÁCULO y el cálculo real del motor son evidencias distintas. Recuperar un resultado tampoco demuestra un recálculo.
- La memoria conversacional guarda un mensaje elegido por el usuario y lo recupera automáticamente. No guarda cada turno; la lista de chats de la ventana sigue en RAM.
- La GPU se documentó para Qwen3 Instruct y Gemma4 IT-QAT en casos y versiones concretos; no se promete uso total de GPU o el mismo rendimiento en otros modelos.

## Qué reúne esta primera muestra

La preparación documental reunió avances, ejemplos de Sala, conexiones, verificación/cálculo, memorias y equipo doméstico. Esta carpeta es la selección curada de esa preparación, con privacidad y derechos revisados en su alcance documental.

No incluye el repositorio interno de trabajo, los expedientes completos o un instalador. Una publicación documental no cambia la aceptación técnica del producto ni cierra sus pendientes de distribución.

[Ver evidencia y alcance](evidencia-y-alcance.md) · [Ver condiciones del equipo](equipo-domestico.md).
