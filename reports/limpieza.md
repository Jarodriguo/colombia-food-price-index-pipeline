# Reglas de limpieza aplicadas

Filas de entrada: **63,082**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 914 | 1.449% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.812% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 8,674 | 13.75% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 412 | 0.653% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,764 | 7.552% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 12,841 | 20.356% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.