# Reglas de limpieza aplicadas

Filas de entrada: **45,527**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 652 | 1.432% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 1.125% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 6,195 | 13.607% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 254 | 0.558% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 3,740 | 8.215% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 9,433 | 20.72% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.