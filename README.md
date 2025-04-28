# Risk Prediction Project

Este proyecto predice la probabilidad de **default** de préstamos utilizando un modelo de **Regresión Logística** y analiza las variables más importantes mediante gráficos **SHAP**.

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
```

## Cómo correr el proyecto

1. Abre el archivo `notebooks/predict_risk.ipynb`.
2. Ejecuta las celdas paso a paso.
3. El modelo entrenará una regresión logística y generará gráficos de importancia de variables.
4. Los gráficos se guardarán automáticamente en la carpeta `images/`.

## Archivos importantes generados

- `images/shap_summary_plot.png`: Gráfico resumen de variables SHAP.
- `images/shap_dependence_plot_monthly_income.png`: Gráfico de dependencia de SHAP para "monthly_income".

