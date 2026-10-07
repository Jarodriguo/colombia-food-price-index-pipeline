# Reglas de limpieza aplicadas

Filas de entrada: **50,672**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 725 | 1.431% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 1.01% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 6,933 | 13.682% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 326 | 0.643% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 3,740 | 7.381% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 10,464 | 20.65% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.