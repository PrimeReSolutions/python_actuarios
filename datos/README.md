# Datos del curso (v2)

Extraídos una sola vez de Google Drive con `herramientas/descargar_datos.py` (2026-07-20).
Los notebooks v2 leen SOLO de esta carpeta; no hay dependencias de Drive ni pickles entre sesiones.

| Archivo | Uso en el curso | Procedencia |
|---|---|---|
| `auto.csv` | Preparación y día 1, bloque 1 (pandas) | CAS Loss Reserve Database (`clrd.csv` de chainladder 0.8.24): West Bend Mut Ins Grp, ppauto y comauto, ocurrencia 1988 a 1997, triángulo superior. incurred = IncurLoss menos BulkLoss; paid = CumPaidLoss. Miles de USD |
| `nuevas_lineas.csv` | Día 1, bloque 1 (ejercicio integrador) | Mismo origen y grupo que `auto.csv`: wkcomp (WorkersComp) y othliab (OtherLiability) |
| `cierre_hogar.xlsx` | Día 1, bloque 2 (Excel y Python) | Sintético (fuentes/datos/generar_cierre_hogar.py, semilla fija): cartera de Hogar de 3 000 pólizas, siniestros con filas de título antes de la cabecera y 3 siniestros sin póliza a propósito, hoja de parámetros en B3:C7. Cierre 31/12/2024, euros |
| `primas_hogar.csv` | Día 1, bloque 2 (Excel y Python) | Sintético, mismo origen: nueva producción 2024 por mes y producto, exportada con formato español (`;`, coma decimal, punto de miles, dd/mm/aaaa). Cuadra con la cartera |
| `hogar_extraccion.xlsx` | Día 1, bloques 3 y 4 (manejo y calidad de datos) | Sintético (fuentes/datos/generar_manejo_datos.py, semilla fija): 20 042 pólizas de Hogar con incidencias controladas (textos, provincias, primas como texto, vacías y negativas, no vigentes, duplicados, tasas anómalas). Cálculo a 31/12/2024 |
| `vida_polizas.csv` | Día 1, bloques 3 y 4 | Sintético, mismo origen: 8 020 pólizas de Vida riesgo en cp1252, separador `;`, formato español; incidencias de sexo, fechas, capitales, vigencia y duplicados |
| `vida_siniestros.xlsx` | Día 1, bloques 3 y 4 | Sintético: 29 fallecimientos, 25 de pólizas de la cartera |
| `provincias.csv` | Día 1, bloques 3 y 4 | Catálogo de las 52 provincias con código INE y comunidad autónoma |
| `berqsherm.csv` | Práctica IBNR (triángulo Berquist-Sherman) | chainladder 0.8.24, solo MedMal. Se eliminó la línea "Auto" del paquete, cuyo incurrido duplica el de MedMal |
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
