# Reglas de limpieza aplicadas

Filas de entrada: **59,097**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 844 | 1.428% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.866% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 8,069 | 13.654% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 374 | 0.633% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,422 | 7.483% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 12,187 | 20.622% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.