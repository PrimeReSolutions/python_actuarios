# WSP — Python aplicado a modelos actuariales

Material para participantes del curso-taller de Python para actuarios: 6 sesiones y un caso integrador (capstone).

## Sesiones

| Sesión | Contenido | Abrir |
|---|---|---|
| 0 · Preparación | Setup del entorno y primer contacto con pandas (**hacer antes del día 1**) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_00_preparacion.ipynb) |
| 1 · Fundamentos | Python básico, estructuras de datos, NumPy, pandas | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_01_fundamentos.ipynb) |
| 2 · Calidad de datos | Calidad de datos de reservas (RRC y RM) y puente Excel → pandas | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_02_calidad_datos.ipynb) |
| 3 · Triángulos e IBNR | Triángulos, factores de desarrollo e IBNR con `chainladder` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_03_triangulos_ibnr.ipynb) |
| 4 · Reservas de vida | RRC y reservas matemáticas de vida, escenarios de estrés | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_04_reservas_vida.ipynb) |
| 5 · Simulación | Distribuciones, Monte Carlo, VaR/TVaR | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_05_simulacion.ipynb) |
| 6 · Riesgo y solvencia | Riesgo de reserva (bootstrap), cópulas, solvencia | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/sesion_06_riesgo_solvencia.ipynb) |
| Capstone | Caso integrador: balance → calidad → reservas → riesgos → ratio de solvencia | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PrimeReSolutions/python_actuarios/blob/main/notebooks/capstone_ejercicio_final.ipynb) |

## Cómo trabajar en Google Colab

1. Haz clic en el botón **Open in Colab** de la sesión. Necesitas haber iniciado sesión con tu cuenta de Google.
2. **Guarda una copia en tu Drive**: `Archivo > Guardar una copia en Drive`. Trabaja siempre sobre esa copia; si no, tus respuestas se pierden al cerrar la pestaña.
3. Ejecuta la **celda de arranque** (⚙️) al inicio del notebook: descarga los datos del curso desde este repositorio y, en las sesiones que lo necesitan, instala `chainladder`.
4. Si Colab reinicia el entorno (al cerrar la sesión o tras un rato de inactividad), vuelve a ejecutar la celda de arranque.

## Cómo trabajar en local

Requiere Python 3.10, 3.11 o 3.12 (recomendado 3.12).

```bash
git clone https://github.com/PrimeReSolutions/python_actuarios.git
cd python_actuarios
python -m venv .venv
.venv\Scripts\activate          # Windows  (en Mac/Linux: source .venv/bin/activate)
pip install -r requirements.txt
jupyter lab
```

Luego abre los notebooks desde la carpeta `notebooks/`.

## Estructura

- `notebooks/` — un notebook por sesión, más el capstone. Donde veas `***` tienes que completar el código.
- `datos/` — datasets del curso e imágenes de apoyo (ver `datos/README.md`).
- `requirements.txt` — versiones de las librerías para la instalación local.
