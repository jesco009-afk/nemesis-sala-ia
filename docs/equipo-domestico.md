# El equipo de referencia

[Volver a NÉMESIS](../README.md).

NÉMESIS está orientado al uso doméstico. Su evidencia describe una configuración concreta; no una lista de mínimos garantizados o una recomendación de compra.

| Recurso | Referencia |
| --- | --- |
| CPU | i7-8700 declarado por el usuario, sin identificación independiente en las fuentes seleccionadas. |
| RAM | 31,9GiB registrados en un log histórico de Ollama;32GB declarados. |
| GPU | GTX1050Ti discreta,4096MiB, controlador582.78 en el diagnóstico. |
| Sistema | EntornoWindows documentado; edición/build y otras plataformas no certificados por esta selección. |
| Modelos/runtime | Versiones identificadas por modalidad; no basta un nombre de familia parecido. |

El cierreGPU usa Qwen3 4B Instruct y Gemma4 E2B IT-QAT bajo Ollama0.40.14. Los ejemplos posteriores usan0.40.15. Las cifras son históricas, no indicaciones de última versión recomendada ni inventario actual del PC.

Hubo reparto CPU/GPU y regreso explícito aCPU. No se promete100%GPU, una velocidad determinada ni la misma aceleración para Qwen3.5, Gemma3 o Granite. Una consulta puntual no es un benchmark.

## Antes de distribuir el software

La Sala gráfica necesita su servidorPython, navegador y módulos propios completos. El recorrido numérico usa otros componentes e intérprete. La instalación original contiene rutas ligadas al equipo; todavía no es una guía de «copiar y ejecutar» para otrosPC.

Queda preparar rutas y runtimes de destino, inventario redistribuible, licencias, almacenamiento de la selección y una instalación limpia. Las fuentes revisadas no imponen Docker/WSL/OpenProject como dependencias de estas rutas.

La documentación actual del proveedor se consulta por separado en [Windows](https://docs.ollama.com/windows), [hardware](https://docs.ollama.com/gpu) y [FAQ](https://docs.ollama.com/faq). Esas páginas no convierten los ensayos históricos en una certificación de todas las configuraciones.

Esta muestra no distribuye modelos, ejecutables o comandos de instalación. [Avances y pendientes](avance-y-pendientes.md).
