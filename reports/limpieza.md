# Reglas de limpieza aplicadas

Filas de entrada: **46,728**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 677 | 1.449% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 1.096% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 6,378 | 13.649% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 288 | 0.616% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 3,740 | 8.004% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 9,657 | 20.666% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.