# Reglas de limpieza aplicadas

Filas de entrada: **52,150**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 749 | 1.436% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.982% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 7,158 | 13.726% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 328 | 0.629% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,080 | 7.824% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 10,764 | 20.64% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.