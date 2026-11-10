# Reglas de limpieza aplicadas

Filas de entrada: **58,788**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 844 | 1.436% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.871% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 8,040 | 13.676% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 373 | 0.634% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,422 | 7.522% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 12,112 | 20.603% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.