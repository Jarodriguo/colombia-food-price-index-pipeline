# Reglas de limpieza aplicadas

Filas de entrada: **61,690**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 891 | 1.444% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.83% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 8,449 | 13.696% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 383 | 0.621% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,764 | 7.722% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 12,545 | 20.336% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.