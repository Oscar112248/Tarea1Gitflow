# Informe - Actividad No. 1 Gitflow con Streamlit

## Integrantes

| Nombre |
| --- |
| Oscar Maldonado |
| Daniel Alquinga |

## Objetivo

Desarrollar una aplicación Streamlit para cargar, validar y analizar el archivo `penguins.csv`, aplicando el flujo de trabajo Gitflow mediante ramas de desarrollo, funcionalidades, release y tag de versión.

## Descripción Del Proyecto

El proyecto consiste en un dashboard web construido con Streamlit que permite analizar el dataset `penguins.csv`. La aplicación valida que el archivo exista, comprueba que el conjunto de datos no esté vacío y verifica que las columnas requeridas estén presentes antes de mostrar métricas, gráficos y una visualización tabular filtrable.

## Procedimiento Realizado

1. Se verificó la instalación de Git con `git --version`.
2. Se verificó la instalación de Python con `python --version`.
3. Se creó la estructura del proyecto con carpetas `src`, `tests` y `docs`.
4. Se incorporó el archivo `penguins.csv` al repositorio.
5. Se creó el archivo `requirements.txt` con las dependencias necesarias.
6. Se implementaron las validaciones en `src/validators.py`.
7. Se desarrolló la aplicación principal en `app.py` usando Streamlit.
8. Se implementó la visualización tabular en `src/data_view.py`.
9. Se agregaron pruebas unitarias en `tests/test_validators.py`.
10. Se documentó el proyecto en `README.md` e `INFORME.md`.
11. Se aplicó Gitflow mediante ramas `main`, `develop`, ramas `feature` y rama `release/v1.0.0`.
12. Se generó el tag `v1.0.0` para identificar la versión entregable.

## Ramas Gitflow Utilizadas

| Rama | Descripción |
| --- | --- |
| `main` | Rama estable donde queda publicada la versión final |
| `develop` | Rama de integración de funcionalidades |
| `feature/validaciones` | Desarrollo de funciones para validar archivo, columnas y datos |
| `feature/app-streamlit` | Desarrollo de la aplicación principal en Streamlit |
| `feature/visualizacion-tabular` | Desarrollo de filtros, tabla y resumen estadístico |
| `feature/pruebas-pytest` | Desarrollo de pruebas automatizadas con pytest |
| `release/v1.0.0` | Preparación de la versión final del proyecto |

No se utilizó rama `hotfix` y no se realizó resolución de conflictos.

## Evidencias De Ejecución

### Aplicación Principal

<img width="921" height="352" alt="image" src="https://github.com/user-attachments/assets/60e6c026-735c-4841-a982-b38e4d3e830b" />



### Visualización Tabular

Insertar captura de la sección de filtros, vista previa, tabla y resumen estadístico:

![Visualización tabular](docs/visualizacion-tabular.png)

### Pruebas Con Pytest

Insertar captura de la ejecución exitosa de `pytest`:

![Pruebas pytest](docs/pytest.png)

## Comandos Principales Utilizados

```bash
git branch -M main
git checkout -b develop
git checkout -b feature/validaciones
git checkout develop
git merge feature/validaciones --no-ff
git checkout -b feature/app-streamlit
git checkout develop
git merge feature/app-streamlit --no-ff
git checkout -b feature/visualizacion-tabular
git checkout develop
git merge feature/visualizacion-tabular --no-ff
git checkout -b feature/pruebas-pytest
git checkout develop
git merge feature/pruebas-pytest --no-ff
git checkout -b release/v1.0.0
git checkout main
git merge release/v1.0.0 --no-ff
git tag -a v1.0.0 -m "Release version 1.0.0"
git checkout develop
git merge release/v1.0.0 --no-ff
```

## Conclusiones Técnicas

1. Gitflow permitió separar el desarrollo funcional en ramas independientes, reduciendo el riesgo de afectar la rama principal durante la construcción de la aplicación.
2. La rama `develop` funcionó como punto de integración para validar las funcionalidades antes de preparar una versión estable en la rama de release.
3. El uso de tags facilitó la identificación de una versión entregable de la aplicación, permitiendo conservar trazabilidad entre código, pruebas y documentación.

## Datos Del Entregable

| Integrante | Repositorio |
| --- | --- |
| Oscar Maldonado | https://github.com/Oscar112248/Tarea1Gitflow |
| Daniel Alquinga | Pendiente de colocar URL del repositorio individual |
