# Reglas de limpieza aplicadas

Filas de entrada: **53,973**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 772 | 1.43% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.949% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 7,419 | 13.746% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 318 | 0.589% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,080 | 7.559% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 11,138 | 20.636% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.