# Reglas de limpieza aplicadas

Filas de entrada: **55,486**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 795 | 1.433% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.923% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 7,616 | 13.726% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 334 | 0.602% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,080 | 7.353% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 11,438 | 20.614% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.