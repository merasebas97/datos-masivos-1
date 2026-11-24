# Datos Masivos I

Prácticas, notebooks y tareas de la asignatura **Datos Masivos I** · Licenciatura en Ciencia de Datos · FES Acatlán, UNAM · Semestre 2026-2
Autor: **Gonzalo Sebastián Mera Montiel**

El curso cubre los fundamentos del procesamiento de datos masivos: las características del Big Data, el modelo **MapReduce** con **PySpark**, la búsqueda de elementos similares (Kd-Trees, ANN) y los algoritmos para **flujos de datos** (muestreo y filtros probabilísticos).

---

## Notebooks

| # | Notebook | Tema | Qué se implementa |
|---|---|---|---|
| 01 | [`01_muestreo_presa_bernoulli.ipynb`](notebooks/01_muestreo_presa_bernoulli.ipynb) | Flujos de datos: muestreo | Muestreo de presa (*reservoir sampling*) y muestreo de Bernoulli sobre los jugadores de FIFA 20 |
| 02 | [`02_filtro_bloom.ipynb`](notebooks/02_filtro_bloom.ipynb) | Flujos de datos: filtrado | Filtro de Bloom con MD5 en lugar de MurmurHash y análisis de falsos positivos |
| 03 | [`03_busqueda_binaria.ipynb`](notebooks/03_busqueda_binaria.ipynb) | Búsqueda | Búsqueda binaria sobre texto con validaciones, y su alternativa distribuida con filtros en PySpark |

## Prácticas (reportes)

| # | Práctica | Tema | Modalidad |
|---|---|---|---|
| 1 | [Probabilidad y eventos esperados](practicas/P1_Bonferroni_probabilidad.pdf) | Principio de Bonferroni | En equipo* |
| 2 | [ANOVA y falsos positivos](practicas/P2_Bonferroni_ANOVA.pdf) | Principio de Bonferroni | En equipo* |
| 3 | [MapReduce en álgebra lineal](practicas/P3_MapReduce_algebra_lineal.pdf) | Multiplicación matriz-vector y matriz-matriz con RDD | En equipo* |
| 4 | [Índice invertido con `flatMapValues`](practicas/P4_indice_invertido_PySpark.pdf) | RDD de (palabra, canciones) con PySpark | Individual |

\* Prácticas 1 a 3 en equipo con **Diego Rafael Moctezuma Ramírez** y **Jesús Eduardo Rodarte Rosales**.

## Tareas de investigación

| # | Tarea | Unidad |
|---|---|---|
| 1 | [ISO 8000 y las 12 V del Big Data](tareas/T01_ISO8000_y_12V.pdf) | 1. Datos masivos |
| 2 | [El filtro burbuja](tareas/T02_filtro_burbuja.pdf) | 1. Datos masivos |
| 3 | [Cómputo en la nube y cómputo cuántico](tareas/T03_nube_y_computo_cuantico.pdf) | 2. Almacenamiento y procesamiento |
| 4 | [RDD: acciones y transformaciones](tareas/T04_RDD.pdf) | 2. MapReduce |
| 5 | [MapReduce para álgebra relacional](tareas/T05_MapReduce_algebra_relacional.pdf) | 2. MapReduce |
| 6 | [Árbol Kd: partición y vecino más cercano](tareas/T06_arbol_Kd.pdf) | 3. Elementos similares |
| 7 | [Metric Trees, Ball Trees y Cover Trees](tareas/T07_metric_ball_cover_trees.pdf) | 3. Elementos similares |
| 8 | [Otros métodos para ANN](tareas/T08_metodos_ANN.pdf) | 3. Elementos similares |
| 9 | [*Her* y *Transcendence*: aprendizaje en línea](tareas/T09_Her_y_Transcendence.pdf) | 4. Flujos de datos |

## Estructura

```
├── notebooks/   Implementaciones en Python y PySpark (ejecutadas, con salidas)
├── practicas/   Reportes de las prácticas en PDF
├── tareas/      Tareas de investigación en PDF
└── requirements.txt
```

## Cómo ejecutar los notebooks

```bash
python -m pip install -r requirements.txt
jupyter notebook
```

- **PySpark** (notebook 03) necesita Java 8, 11 o 17. Otra opción es abrirlo en Google Colab, donde funciona directamente.
- **Datos de FIFA 20** (notebook 01): descarga `players_20.csv` del dataset [FIFA 20 complete player dataset](https://www.kaggle.com/datasets/stefanoleone992/fifa-20-complete-player-dataset) en Kaggle y colócalo en `notebooks/`. No se incluye en el repositorio.
- El notebook 02 descarga su lista de palabras de internet al ejecutarse.

## Créditos

Curso impartido por la profesora **Alondra Vanianinetl Berzunza Rodríguez**. El material de clase (apuntes y notebooks de la profesora) no se incluye en este repositorio.
