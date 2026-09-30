# Reglas de limpieza aplicadas

Filas de entrada: **48,845**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 700 | 1.433% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 1.048% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 6,680 | 13.676% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 301 | 0.616% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 3,740 | 7.657% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 10,089 | 20.655% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.