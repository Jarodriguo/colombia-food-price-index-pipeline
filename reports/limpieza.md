# Reglas de limpieza aplicadas

Filas de entrada: **63,508**

| Regla | Qué corrige | Filas | % | Acción |
|---|---|---:|---:|---|
| R1 | Plazas con dos nombres (Ibagué La 21, Pereira La 41) | 914 | 1.439% | corrige |
| R2 | Etiquetas de grupo inconsistentes (7 -> 3) | 512 | 0.806% | corrige |
| R3 | Precio fuera de [100, 100,000] | 0 | 0.0% | marca |
| R4 | Precio idéntico 3+ días seguidos | 8,747 | 13.773% | marca |
| R5 | Atípico dentro de su serie (|z MAD| > 5.0) | 411 | 0.647% | marca |
| R6 | Día posterior a un puente (>3 días sin publicación) | 4,764 | 7.501% | marca |
| R7 | Serie con cobertura >= 95% (panel fijo) | 12,915 | 20.336% | marca |

> Las reglas marcadas como *marca* no eliminan filas: agregan una columna booleana para que el análisis decida.