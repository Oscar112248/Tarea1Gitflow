# Penguins Analytics Dashboard

Aplicación de análisis de datos construida con **Python**, **Streamlit**, **pandas** y **pytest**, desarrollada bajo un flujo de trabajo **Gitflow**. El proyecto permite validar, explorar y visualizar el dataset `penguins.csv` mediante una interfaz web simple, clara y orientada a la toma de decisiones.

---

## Resumen Ejecutivo

| Elemento | Descripción |
| --- | --- |
| Proyecto | Dashboard Streamlit para análisis del dataset Penguins |
| Objetivo | Cargar, validar y visualizar información relevante del archivo `penguins.csv` |
| Enfoque técnico | Desarrollo por ramas con Gitflow, pruebas automatizadas y documentación formal |
| Versión entregable | `v1.0.0` |
| Autores | Oscar Maldonado, Daniel Alquinga |

---

## Propósito

El propósito del proyecto es entregar una aplicación reproducible para analizar datos de pingüinos, incorporando controles básicos de calidad sobre el archivo de entrada y una visualización tabular que permita inspeccionar la información por especie e isla.

La solución demuestra buenas prácticas de control de versiones, separación funcional del código, validación de datos y pruebas unitarias.

---

## Funcionalidades

- Carga automática del archivo `penguins.csv`.
- Validación de existencia del archivo.
- Validación de columnas obligatorias del dataset.
- Validación de que el dataset no esté vacío.
- Métricas generales: registros, columnas, especies e islas disponibles.
- Gráfico de distribución por especie.
- Visualización tabular con filtros por especie e isla.
- Vista previa y tabla completa de datos.
- Resumen estadístico de columnas numéricas.
- Pruebas unitarias con `pytest`.

---

## Tecnologías Utilizadas

| Tecnología | Uso |
| --- | --- |
| Python | Lenguaje principal del proyecto |
| Streamlit | Construcción del dashboard web |
| pandas | Carga, validación y análisis de datos |
| matplotlib | Generación del gráfico principal |
| pytest | Pruebas unitarias |
| Git / Gitflow | Control de versiones y organización del desarrollo |

---

## Estructura Del Proyecto

```text
Tarea1Gitflow/
├── app.py
├── penguins.csv
├── requirements.txt
├── README.md
├── INFORME.md
├── .gitignore
├── docs/
│   └── .gitkeep
├── src/
│   ├── __init__.py
│   ├── validators.py
│   └── data_view.py
└── tests/
    ├── __init__.py
    └── test_validators.py
```

---

## Instalación

Desde la carpeta del proyecto:

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

---

## Ejecución De La Aplicación

```bash
streamlit run app.py
```

La aplicación cargará el archivo `penguins.csv`, ejecutará validaciones y mostrará el dashboard con métricas, gráfico y tabla filtrable.

---

## Ejecución De Pruebas

```bash
pytest
```

Las pruebas verifican la existencia del archivo, la validez estructural del dataset, el manejo de DataFrames vacíos y la carga de archivos CSV temporales.

---

## Gitflow Aplicado

| Rama | Propósito |
| --- | --- |
| `main` | Contiene la versión estable del proyecto |
| `develop` | Integra las funcionalidades antes del release |
| `feature/validaciones` | Implementa las funciones de validación del dataset |
| `feature/app-streamlit` | Construye la aplicación principal en Streamlit |
| `feature/visualizacion-tabular` | Agrega filtros, tabla y resumen estadístico |
| `feature/pruebas-pytest` | Incorpora pruebas unitarias con pytest |
| `release/v1.0.0` | Prepara la versión estable para entrega |

Tag de versión: `v1.0.0`

No se utilizó rama `hotfix` y no se realizó resolución de conflictos.

---

## Evidencias Sugeridas

Cuando se capturen las pantallas finales, guardarlas en la carpeta `docs/` con estos nombres:

| Evidencia | Archivo sugerido |
| --- | --- |
| Aplicación principal | `docs/app-principal.png` |
| Visualización tabular | `docs/visualizacion-tabular.png` |
| Pruebas pytest | `docs/pytest.png` |

---

## Autores

| Integrante | Rol |
| --- | --- |
| Oscar Maldonado | Desarrollo, documentación y control de versiones |
| Daniel Alquinga | Validación funcional, revisión y evidencias |
