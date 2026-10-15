# Reglas de limpieza aplicadas

Filas de entrada: **52,463**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 749 | 1.428% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.976% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 7,194 | 13.713% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 329 | 0.627% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,080 | 7.777% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 10,839 | 20.66% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.