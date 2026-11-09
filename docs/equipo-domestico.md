# NÉMESIS en un PC de casa

© 2026 **Jean y equipo NÉMESIS** · [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.es)

Las pruebas de NÉMESIS se hicieron en un PC doméstico con Windows, 32 GB de RAM declarados y una GTX 1050 Ti de 4 GB. Esta ficha distingue la configuración que usamos de los requisitos que todavía debemos validar para otros equipos.

## El equipo de referencia

| Componente | Dato de las pruebas |
| --- | --- |
| Procesador | Intel Core i7-8700, según la descripción del usuario. |
| Memoria RAM | 32 GB declarados. El diagnóstico de Ollama registró 31,9 GiB de memoria total. |
| Tarjeta gráfica | NVIDIA GeForce GTX 1050 Ti discreta, con 4096 MiB de memoria de vídeo y controlador 582.78 en el diagnóstico. |
| Sistema | Windows. La edición y la compilación exactas quedan por confirmar. |

## Qué hizo la tarjeta gráfica

Con Ollama 0.40.14 y CUDA 12, una consulta de diagnóstico de Qwen descargó 32 de 37 capas a la GPU. En las pruebas numéricas de Sala y Orquestador se registró uso de GPU con `qwen3:4b-instruct-2507-q4_K_M` y `gemma4:e2b-it-qat`. También se probó el regreso explícito a CPU. El trabajo de los modelos puede repartirse entre CPU y GPU.

Esos ensayos del 4 de noviembre de 2026 cubren las variantes indicadas. La aceleración en los modelos del chat, la velocidad con cada configuración y la capacidad con varias tareas simultáneas siguen por medir. El cierre del diagnóstico y la integración se documentaron en los registros del proyecto (INF-000324, INF-000326 e INF-000328).

## Qué necesita cada recorrido

| Recorrido | Piezas que se usaron |
| --- | --- |
| Sala de conversación | Navegador, servidor local de Sala con Python y sus módulos, Ollama y los modelos de la modalidad elegida. |
| Verificación y cálculo | Ollama y los modelos de la ruta numérica, Orquestador, adaptador, ORÁCULO, motor y almacenamiento de resultados. Esta ruta tiene su propia configuración y dependencias. |
| Memorias | Almacenamiento local para los antecedentes elegidos o los resultados verificados, según el recorrido. |

El espacio depende del software y de los modelos elegidos. La memoria disponible, el contexto y la concurrencia influyen en cuánta carga admite el equipo. Los requisitos del proveedor se consultan aparte de las pruebas de NÉMESIS. [Ollama en Windows](https://docs.ollama.com/windows) · [GPU compatibles](https://docs.ollama.com/gpu) · [Preguntas frecuentes de Ollama](https://docs.ollama.com/faq).

## Qué falta comprobar en otro PC

1. Empaquetar los módulos y fijar las versiones de los programas que necesita cada recorrido. La instalación de referencia usa rutas propias de ese equipo.
2. Medir disco, RAM y memoria de vídeo con una selección concreta de modelos, tanto en CPU como en el modo automático.
3. Probar una instalación limpia en otro PC con datos ficticios y registrar el resultado, incluido el retorno a CPU.

Los mínimos de hardware y la instalación reproducible siguen pendientes. Esta entrega documenta las pruebas realizadas en el equipo de referencia.

[Volver a NÉMESIS](../README.md) · [Evidencia y alcance](evidencia-y-alcance.md)
