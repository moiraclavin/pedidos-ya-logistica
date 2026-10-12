# Pedidos Ya – Logística (ITBA)

Análisis exploratorio para el caso *Delivery y tecnología – PedidosYa*. El problema de la consigna: la tasa de aceptación de órdenes ronda el 70% (Mercado A) y los un-dispatch (el rider acepta y luego no finaliza) son ~2%.

## Estructura

| Archivo | Contenido |
|---|---|
| `EDA_PedidosYa_v3.ipynb` | Versión vigente del EDA (secciones 1 a 12) |
| `EDA_PedidosYa_v2.ipynb`, `EDA_PedidosYa.ipynb` | Versiones anteriores |
| `notebook.ipynb` | Notebook auxiliar |

Las bases (`Base de Pedidos`, `Base de Riders`, `Base de Turnos`) no se versionan: son datos reales, el repositorio es público y `Base de Pedidos.csv` pesa ~429 MB. Están en `.gitignore`.

## Contenido del EDA (v3)

1. Carga y calidad de datos
2. Construcción de variables
3. Tendencias temporales
4. Relaciones entre variables (pedidos)
5. Riders
6. Turnos y oferta vs demanda
7. Productividad (pedidos × turnos × riders) y UTR
8. Relación entre turnos, riders y pedidos
9. Un-dispatch: tasas oficiales y nivel de servicio
10. Escenarios de impacto (nivel de servicio, UTR y CPO)
11. Validación de hipótesis
12. Hallazgos

## Decisiones metodológicas

| Decisión | Detalle |
|---|---|
| Unidad de la tabla de pedidos | Una fila por transición (1.217.343 filas, 329.196 pedidos) |
| Tasas de un-dispatch | Definiciones de la profesora, sobre todas las filas de `pedidos` |
| UTR | Σ pedidos entregados / Σ horas conectadas (turno real dentro del período común de turnos y pedidos) |
| Escenarios | Expresados en % o minutos, no en valores absolutos |

## Estado

| Entregable | Estado |
|---|---|
| EDA (v3) | En curso |
| Meta numérica de las hipótesis | **[revisar]** |

## Registro de cambios

### 2026-10-12
- Subido `EDA_PedidosYa_v3.ipynb` al repositorio.
- Agregados los notebooks restantes, este README y `.gitignore` para las bases de datos.
