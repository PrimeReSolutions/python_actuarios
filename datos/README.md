# Datos del curso (v2)

Extraídos una sola vez de Google Drive con `herramientas/descargar_datos.py` (2026-07-20).
Los notebooks v2 leen SOLO de esta carpeta; no hay dependencias de Drive ni pickles entre sesiones.

| Archivo | Uso en el curso | Procedencia |
|---|---|---|
| `auto.csv` | Sesión 1 (pandas básico) | Carpeta Drive del curso |
| `berqsherm.csv` | Sesión 1 y práctica IBNR (triángulo Berquist-Sherman) | Carpeta Drive / repo casact |
| `prism.csv` | Sesión 3 (chainladder) | GitHub casact/chainladder-python |
| `base_rrc.xlsx` | Sesión 2 (calidad RRC) y sesión 4 (cálculo RRC/pnc) | Drive id 13GYIQ… (=`clase_rrc.xlsx`) |
| `base_rmat.csv` | Sesión 2 (calidad RM), sesiones 3-4 (reservas) | **Sustituto**: derivado de `rmat_ejercicio_final.xlsx` (el CSV original, Drive id 1xyJ7…, ya no existe). Columnas renombradas: Prima→`monto prima`, suma asegurada→`suma_asegurada` |
| `siniestros.xlsx` | Sesión 2 (marcar pólizas siniestradas) | Drive id 1yPvF… |
| `siniestros_dirty.xlsx` | Triángulos con datos "sucios" (2 217 movimientos) | Carpeta Drive |
| `base_siniestros.xlsx` | Sesión 3 / práctica IBNR (785 movimientos) | Carpeta Drive |
| `rmat_ejercicio_final.xlsx` | Capstone (calidad de datos + reservas) | Drive id 1mkJ43… |
| `tabla_qx.xlsx` | Sesiones 4 y capstone (mortalidad qx / caídas cx) | Drive id 1Eu1tL… (=`rmat_tabla.xlsx`) |
| `vector_tasas_descuento.xlsx` | Sesiones 4 y capstone (curva de descuento) | Drive id 1kztXY… (=`rmat_vtd.xlsx`) |
| `factor_nivelacion.xlsx` | Anexo factor de nivelación | Drive id 1E-Xgx… (=`datos_FN.xlsx`) |
| `exposicion.xlsx` | Expuestos por póliza (24 269 filas) | Carpeta Drive |
| `rprima.csv` | Sesión 6 (riesgo de prima) | Carpeta Drive |
| `img/` | Figuras de teoría (flujos nominal/probabilizado/financiero, esquema pólizas, logo) | Carpeta Drive |

## Archivos originales perdidos (los IDs de Drive devuelven 404)

- `base_rmat.csv` (id 1xyJ7…) → sustituido como se indica arriba.
- Base del día 3 (id 1ByfRz…) → era la base para el cálculo de RRC; se usa `base_rrc.xlsx`.
- `rmat_dia4.csv` (id 1wxyff…) → se usa el mismo `base_rmat.csv`.

Si el instructor conserva copias de los originales, puede reemplazarlos aquí con esos mismos nombres.
