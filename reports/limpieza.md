# Reglas de limpieza aplicadas

Filas de entrada: **57,984**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 844 | 1.456% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.883% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 7,926 | 13.669% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 362 | 0.624% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,422 | 7.626% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 11,962 | 20.63% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.