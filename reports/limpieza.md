# Reglas de limpieza aplicadas

Filas de entrada: **53,662**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 772 | 1.439% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.954% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 7,389 | 13.77% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 324 | 0.604% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,080 | 7.603% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 11,063 | 20.616% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.