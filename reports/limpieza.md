# Reglas de limpieza aplicadas

Filas de entrada: **53,287**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 772 | 1.449% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.961% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 7,302 | 13.703% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 327 | 0.614% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,080 | 7.657% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 10,989 | 20.622% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.