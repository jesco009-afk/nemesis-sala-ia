# ORÁCULO y el motor de cálculo

Documentación original de **Jean y equipo NÉMESIS** · **[CC BY 4.0](https://github.com/jesco009-afk/nemesis-sala-ia/blob/main/LICENSE.txt)**.

[Volver a NÉMESIS](https://github.com/jesco009-afk/nemesis-sala-ia).

Una propuesta de un modelo, una aceptación de ORÁCULO y un resultado calculado son evidencias diferentes. En el recorrido numérico de NÉMESIS se conservan por separado para distinguir qué se revisó y qué llegó a calcularse.

## Qué hace cada pieza

| Pieza | Su función en el ejemplo SUMAR |
| --- | --- |
| **ORÁCULO** | Comprueba sin ejecutar que la propuesta cumple un contrato: las reglas concretas exigidas al código. |
| **Motor de cálculo** | Ejecuta el cálculo del caso admitido y registra su resultado en un recibo separado. |

## Un caso aceptado con cálculo real

El **6 de noviembre de 2026**, en una sesión nueva de **Sala numérica AUTO** con Ollama **0.40.15**, Qwen propuso el candidato y Gemma lo revisó. El contenido del bloque Python era:

```python
def sumar(a, b):
    return a + b
```

El contrato exigía esa función y expresión, sin imports, llamadas o instrucciones adicionales. Su inferencia supone enteros Python estrictos; excluye booleanos y subclases. La API estática no recibe los operandos: las comprobaciones de entradas y límites operativos corresponden a otras capas.

> **Candidato y contrato** → **ORÁCULO: aceptación estática** → **Motor: cálculo nuevo** → **Recibo: 39 entero**.

| Evidencia | Resultado registrado |
| --- | --- |
| Revisión de Gemma | `APPROVED`; no sustituye al veredicto de ORÁCULO. |
| Verificación de ORÁCULO | `accepted=true`, sin errores; **inferencia estática condicionada**. |
| Cálculo del motor | `CALCULATED`, **23 + 16 = 39**, tipo entero. |
| Registro final | Resultado nuevo enlazado al recibo del motor y al recuerdo guardado. |

Recuperar un 39 anterior no sustituyó este cálculo nuevo. La referencia esperada se construyó desde los operandos con el mismo operador Python; la coincidencia observada no acredita independencia algorítmica.

## Un rechazo en un control aislado

El **5 de noviembre de 2026**, otro ensayo presentó un candidato **sintético**, preparado para el control:

```python
def sumar(a, b):
    return a - b
```

La **API estática real** respondió `accepted=false` con `RETURN_MUST_BE_A_PLUS_B`: se exigía suma y la propuesta restaba. El driver registró `STOP_SIN_REINTENTO` y el productor, `STOP_SIN_GUARDAR`.

Los contadores documentaron que el control se detuvo antes de las fronteras instrumentadas de cálculo y guardado aceptado. Transporte, modelos y otras capas eran dobles de prueba: **no fue un error real de Qwen o Gemma ni una segunda prueba integral de producción**. Tampoco demuestra un aislamiento independiente del sistema operativo.

## Alcance de lo demostrado

El positivo acredita un cálculo real concreto. El negativo acredita el rechazo del verificador y la parada de un control aislado. Son ensayos históricos distintos; esta presentación no los ejecuta nuevamente.

Este perfil utiliza una gramática cerrada de SUMAR. No demuestra corrección de cualquier programa, todos los operandos, concurrencia o seguridad universal. El adaptador y los recibos enlazan la procedencia; ORÁCULO no la certifica por sí solo. El chat gráfico de conversación libre conserva su propia ruta.

Respaldo: **INF-000352 / REG-000631** para el positivo y **O3, INF-000341 / REG-000620** para el rechazo. Los expedientes originales permanecen bajo custodia del proyecto.

[Evidencia y alcance](https://github.com/jesco009-afk/nemesis-sala-ia/blob/main/docs/evidencia-y-alcance.md) · [Conexión entre componentes](https://github.com/jesco009-afk/nemesis-sala-ia/blob/main/docs/conexiones-sala-orquestador-oraculo.md) · [Licencia y atribución](https://github.com/jesco009-afk/nemesis-sala-ia/blob/main/AVISOS.md).
