# Risk Prediction Project

Este proyecto predice la probabilidad de **default** de préstamos utilizando un modelo de **Regresión Logística** y analiza las variables más importantes mediante gráficos **SHAP**.

Resumen Ejecutivo: https://docs.google.com/document/d/12UAflkkXJelxJ99Ocl80dAbyAUPrRQPE2qIczM49gEs/edit?usp=sharing

## Estructura del Proyecto

```
.
├── data/                  # Datos usados para entrenar el modelo (no incluidos aquí)
├── images/                # Gráficos generados automáticamente
├── models/                # Modelos entrenados (opcional)
├── notebooks/
│   └── predict_risk.ipynb # Notebook principal para entrenamiento, explicación y visualización
├── .venv/                 # Entorno virtual (recomendado usar uno)
├── pyproject.toml         # Configuración de dependencias (manejado con Poetry)
├── poetry.lock            # Archivo de bloqueo de dependencias
└── .gitignore
```

## Requisitos

- Python 3.10+
- `poetry` (para manejar dependencias)

Instalar `poetry` si no lo tienes:

```bash
pip install poetry
```

Instalar dependencias:

```bash
poetry install
```

Activar el entorno:

```bash
poetry shell
source [path-to-venv]/bin/activate
```

## Cómo correr el proyecto

1. Abre el archivo `notebooks/predict_risk.ipynb`.
2. Ejecuta las celdas paso a paso.
3. El modelo entrenará una regresión logística y generará gráficos de importancia de variables.
4. La tabla de probabilidad default para creditos vigentes se encuentra en `data/risk_probabilities.xlsx`
5. Los gráficos se guardarán automáticamente en la carpeta `images/`.

## Archivos importantes generados

- `images/shap_summary_plot.png`: Gráfico resumen de variables SHAP.
- `images/shap_dependence_plot_monthly_income.png`: Gráfico de dependencia de SHAP para "monthly_income".
- `data/risk_probabilities.xlsx`: Tabla de probabilidades default para creditos vigentes 

Nota: Se hizo uso de ChatGPT para tareas especificas: correccion de errores y esbozo del README file

