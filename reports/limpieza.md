# Reglas de limpieza aplicadas

Filas de entrada: **62,064**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 891 | 1.436% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.825% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 8,534 | 13.75% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 382 | 0.615% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,764 | 7.676% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 12,619 | 20.332% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.