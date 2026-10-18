# Datos del curso

Los notebooks del curso leen solo de esta carpeta. Los datos sintéticos se generan con semilla fija, por lo que las cifras de los notebooks son reproducibles.

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
| `autos_frecuencia.csv` | Día 2, bloque 1 (calibración) | Sintético (fuentes/datos/generar_calibracion.py): 12 000 pólizas de Autos con su número de siniestros en 2024, binomial negativa |
| `autos_severidad.csv` | Día 2, bloque 1 (calibración) | Sintético, mismo origen: coste de 400 siniestros de daños propios, lognormal |
| `vida_cartera.csv` | Día 2, bloque 4 (provisiones de vida) | Base depurada de `vida_polizas.csv` con las reglas del día 1 (fuentes/datos/generar_vida.py) |
| `tabla_mortalidad.csv` | Día 2, bloque 4 | Tabla técnica unisex de la tarifa (Gompertz, ilustrativa); no es una tabla oficial |
| `vida_experiencia.csv` | Día 3, bloque 2 (riesgos vida) | Sintético (fuentes/datos/generar_experiencia_vida.py): expuestos y fallecidos por año (2019 a 2024), edad y sexo de toda la cartera de Vida riesgo |
| `rentas_cartera.csv` | Día 3, bloque 2 | Sintético, mismo generador: 1 500 rentas vitalicias inmediatas de pago anual anticipado |
| `autos_tarificacion.csv` | Día 3, bloques 3 y 4 (tarificación) | Sintético (fuentes/datos/generar_tarificacion.py): 40 000 pólizas de Autos con factores de riesgo, exposición, número de siniestros y coste; el color no tiene efecto, a propósito |
| `berqsherm.csv` | Día 2, bloque 3 (Berquist-Sherman) | chainladder 0.8.24, solo MedMal. Se eliminó la línea "Auto" del paquete, cuyo incurrido duplica el de MedMal |
| `prism.csv` | Día 2, bloque 3 (provisiones no vida) y día 3, bloque 1 (riesgos no vida) | GitHub casact/chainladder-python |
| `img/` | Logo del curso | Propio |
