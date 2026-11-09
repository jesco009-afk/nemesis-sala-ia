# Encargo para la IA instaladora de Sala IA

© 2026 **Jean y equipo NÉMESIS** · [CC BY 4.0](../LICENSE.txt)

**Destinataria: una IA con acceso al PC Windows de destino.** Tu misión es instalar todos los componentes necesarios para el alcance indicado por el usuario, comprobar que Sala IA responde desde el navegador y dejarla corriendo para que el usuario pueda seguir usándola.

**Estado: borrador R001.** La instalación depende de que el equipo técnico entregue el paquete y su procedimiento de arranque para Windows. Ejecuta el encargo cuando el usuario del PC de destino autorice la instalación en ese equipo.

## 0. Datos que necesitas antes de instalar

Completa esta ficha con la entrega del equipo técnico y los datos del equipo de destino. Comprueba cada dato antes de usarlo.

| Dato | Qué debes obtener |
| --- | --- |
| Paquete de Sala IA | Ubicación autorizada, versión, inventario de archivos y huella del paquete. |
| Preparación de Windows | Arquitectura y versión admitidas, espacio disponible y carpeta de instalación elegida. |
| Dependencias | Versiones de Python y Ollama compatibles con el paquete, fuentes oficiales y requisitos de la aplicación. |
| Modelo individual | Etiqueta exacta, identidad o huella esperada, fuente autorizada y espacio requerido. |
| Configuración | Rutas de aplicación y de datos, puerto o forma de descubrirlo, perfil de CPU o GPU y configuración admitida. |
| Arranque y detención | Procedimiento oficial del paquete para iniciar y detener Sala IA y mantenerla disponible después de terminar la tarea. |
| Módulos | Lista de módulos adicionales que pidió el usuario, con su versión, dependencias y prueba de aceptación. |

El [repositorio público de NÉMESIS](https://github.com/jesco009-afk/nemesis-sala-ia) contiene la documentación. Si todavía falta el paquete instalable, su versión, el modelo aprobado o el procedimiento de arranque, **detente antes de instalar** e indica qué dato necesita aportar el equipo técnico. Usa los comandos que entregue el paquete para esa versión. Trata las rutas del PC original como referencias históricas.

## 1. Preparar el PC de destino

1. Revisa Windows, espacio en disco y memoria disponible. Identifica las instalaciones y procesos existentes de Python, Ollama y Sala IA. Si existe una instancia compatible y autorizada, reutilízala.
2. Verifica la procedencia y las huellas indicadas para el paquete y sus dependencias. Usa las fuentes oficiales o las que el equipo técnico haya autorizado. Instala solo los componentes faltantes del alcance.
3. Comprueba si el modelo aprobado ya está disponible y completo. Descárgalo solo si hace falta y el usuario autorizó la descarga. Conserva los demás modelos y datos del equipo.

## 2. Instalar y abrir Sala IA

1. Prepara el paquete en la carpeta de destino y aplica la configuración indicada para ese equipo. Conserva aparte los datos existentes cuando haya una instalación previa.
2. Inicia o reutiliza Ollama según el procedimiento aprobado. Comprueba desde el equipo que responde y que identifica el modelo elegido. Si aparece un conflicto de puerto o versión, registra qué proceso lo causa y resuélvelo con el método admitido por el paquete.
3. Inicia Sala IA con el procedimiento de la entrega. Registra la dirección local que devuelve y ábrela en el navegador del PC. Usa la configuración local aprobada. Cualquier requisito de administrador, exposición de red o inicio automático con Windows se consulta con el usuario del PC antes de aplicarlo.

## 3. Verificar y dejarla corriendo

1. En la interfaz de Sala IA, elige **Individual** y el modelo aprobado. Envía una pregunta breve con datos ficticios. Por ejemplo, «¿Qué puedo preparar con arroz y verduras? Dame una idea en una frase».
2. Comprueba que la respuesta aparece en la Sala y que corresponde al modelo seleccionado. Si falla, indica la etapa exacta y el error observado. Corrige dentro del alcance autorizado y repite la comprobación.
3. Comprueba que la Sala sigue accesible desde la dirección local y que su proceso y Ollama permanecen activos. Déjalos corriendo con el mecanismo aprobado y la Sala abierta en el navegador. Si el entorno cierra los procesos al terminar la tarea, informa ese impedimento y solicita el método de arranque que deba usarse en ese PC.
4. Entrega al usuario la dirección local y los pasos para detener y volver a abrir la Sala. Confirma «queda corriendo» solo después de la última comprobación.

## 4. Módulos adicionales

La instalación base se comprueba primero con una conversación individual. Añade GPU, modo doble, memorias o recorrido numérico solo si están en la lista solicitada y su entrega técnica identifica las dependencias y las pruebas. Verifica y registra cada módulo por separado. El éxito en modo individual deja abierta la validación de los módulos adicionales.

## Informe para el usuario

Registra la fecha, las versiones instaladas o reutilizadas, el modelo y la modalidad, la carpeta de instalación, la dirección local, el resultado de la prueba y el estado de los procesos al finalizar. Incluye los pasos de reinicio y detención, y las brechas que sigan pendientes. Usa datos de prueba y conserva el informe en el PC de destino.

La ficha de referencia explica qué se observó en el equipo original y qué falta validar en otro PC. [Equipos domésticos y requisitos pendientes](https://github.com/jesco009-afk/nemesis-sala-ia/blob/main/docs/equipo-domestico.md).
