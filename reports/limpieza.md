# Reglas de limpieza aplicadas

Filas de entrada: **56,510**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 820 | 1.451% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.906% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 7,718 | 13.658% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 332 | 0.588% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,080 | 7.22% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 11,663 | 20.639% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.