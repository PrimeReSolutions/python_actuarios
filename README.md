# Python para Actuarios

Material del curso Python para Actuarios: 11, 12 y 13 de noviembre de 2026.

## Notebooks

| Día | Bloque | Contenido | Abrir |
|---|---|---|---|
| Antes del curso | Preparación | Entorno de trabajo en Colab, primer contacto con pandas y comprobación de Python en Excel | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/dia0_preparacion.ipynb) |
| 1 | 1 | Introducción a Python, NumPy y pandas | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/dia1_01_introduccion_python.ipynb) |
| 1 | 2 | Excel y Python: lectura y escritura de libros, CSV en formato español, tablas dinámicas, triángulos y cruces con control | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/dia1_02_excel_python.ipynb) |
| 1 | 3 y 4 | Manejo de datos | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_02_calidad_datos.ipynb) |
| 2 | 2 | Simulación | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_05_simulacion.ipynb) |
| 2 | 3 | Reservas no vida | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_03_triangulos_ibnr.ipynb) |
| 2 | 4 | Reservas vida | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_04_reservas_vida.ipynb) |
| 3 | 1 | Riesgos no vida | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_06_riesgo_solvencia.ipynb) |

Los notebooks pendientes de adaptar al nuevo formato conservan por ahora su nombre anterior.

## Cómo trabajar en Google Colab

1. Pulsa el botón *Open in Colab* del notebook. Necesitas haber iniciado sesión con una cuenta de Google.
2. Guarda una copia en tu Drive (*Archivo > Guardar una copia en Drive*) y trabaja siempre sobre ella.
3. Ejecuta la celda de **preparación del entorno** al inicio del notebook: descarga los datos del curso y, cuando hace falta, instala librerías adicionales.
4. Si Colab reinicia el entorno, vuelve a ejecutar la preparación del entorno y las celdas anteriores.

El código que debes completar está marcado con `***`.

## Instalación local (opcional)

Requiere Python 3.10, 3.11 o 3.12.

```bash
git clone https://github.com/PrimeReSolutions/python_actuarios.git
cd python_actuarios
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
```

En Mac o Linux, la activación del entorno es `source .venv/bin/activate`.

## Estructura

1. `notebooks/`: un notebook por bloque del curso.
2. `datos/`: conjuntos de datos e imágenes de apoyo (ver `datos/README.md`).
3. `requirements.txt`: versiones de las librerías para la instalación local.
