# Reglas de limpieza aplicadas

Filas de entrada: **62,377**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 891 | 1.428% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.821% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 8,576 | 13.749% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 381 | 0.611% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,764 | 7.637% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 12,693 | 20.349% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.