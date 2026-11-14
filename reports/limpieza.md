# Reglas de limpieza aplicadas

Filas de entrada: **60,221**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 867 | 1.44% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.85% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 8,233 | 13.671% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 357 | 0.593% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,422 | 7.343% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 12,409 | 20.606% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.