# Python para Actuarios

Datos e imágenes del curso Python para Actuarios: 11, 12 y 13 de noviembre de 2026.

Este repositorio no contiene los notebooks del curso; el equipo docente los facilita por separado.

## Cómo se usa en Google Colab

La celda de **preparación del entorno** de cada notebook descarga este repositorio en Colab y sitúa la sesión en su carpeta, de modo que el notebook lee los datos de `datos/`. No hay que hacer nada más.

1. Abre el notebook en Colab y guarda una copia en tu Drive (*Archivo > Guardar una copia en Drive*).
2. Ejecuta la celda de preparación del entorno antes que cualquier otra.
3. Si Colab reinicia el entorno, vuelve a ejecutar la preparación del entorno y las celdas anteriores.

## Instalación local (opcional)

Requiere Python 3.11 o 3.12.

```bash
git clone https://github.com/PrimeReSolutions/python_actuarios.git
cd python_actuarios
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
```

Guarda los notebooks del curso dentro de la carpeta `python_actuarios`, junto a la carpeta `datos`. En Mac o Linux, la activación del entorno es `source .venv/bin/activate`.

## Estructura

1. `datos/`: conjuntos de datos e imágenes de apoyo (ver `datos/README.md`).
2. `requirements.txt`: versiones de las librerías para la instalación local.
