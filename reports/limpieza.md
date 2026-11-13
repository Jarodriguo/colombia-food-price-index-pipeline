# Reglas de limpieza aplicadas

Filas de entrada: **59,799**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 867 | 1.45% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.856% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 8,166 | 13.656% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 389 | 0.651% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,422 | 7.395% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 12,335 | 20.627% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.