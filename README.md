# TFG -- Análisis de los factores socioeconómicos, familiares y culturales del éxito escolar en España

**Autora:** María Duque
**Grado:** Business Analytics
**Año Académico:** 2025-2026

---

## Sobre el proyecto

El sistema educativo presenta diferencias estructurales entre Comunidades Autónomas derivadas de factores económicos, sociales y demográficos.
Este Trabajo de Fin de Grado analiza dichas diferencias mediante un enfoque cuantitativo basado en:

•⁠  ⁠Modelos econométricos de datos de panel  
•⁠  ⁠Técnicas de segmentación no supervisada  
•⁠  ⁠Análisis exploratorio de datos  

El objetivo es identificar los principales determinantes del éxito escolar y clasificar las regiones según su perfil educativo.

## Objetivos

•⁠  ⁠Analizar la *tasa de graduación en ESO*
•⁠  ⁠Construir un *Índice de Éxito Escolar*
•⁠  ⁠Evaluar el impacto de:
  - renta per cápita
  - nivel educativo de la población
  - género
•⁠  ⁠Identificar *clusters de comunidades autónomas*

## Metodología
El análisis se estructura en dos enfoques complementarios:
### Modelos supervisados 
•⁠  ⁠MCO Agrupado  
•⁠  ⁠Efectos Fijos  
•⁠  ⁠Efectos Aleatorios  
•⁠  ⁠Test de Hausman  
### Modelos no supervisados
•⁠  ⁠K-Means  
•⁠  ⁠Clustering jerárquico (Ward, Complete, Single)  
•⁠  ⁠PCA (reducción dimensional)  

---

## Estructura del repositorio

DATOS_TFG/
│
├── raw/                     # Datos originales (INE, EducaBase)
├── processed/               # Datos limpios y transformados (Se encuentran las bases finales para el análisis)
│
├── Notebook/
│   ├── IngenieriaDatos/     # Limpieza y construcción de datasets
│   ├── AnalisisDatos/       # Modelos supervisados y no supervisados
│   ├── graficos_EDA1/       # Análisis exploratorio de la Base 1 (Dataset Longitudinal de Rendimiento escolar)
│   ├── graficos_EDA2/.      # Análisis exploratorio de la Base 2 (Dataset Estructural por CCAA)
│   └── graficos_clustering/ # Resultados de los modelos no supervisados
│
├── README.md
└── .gitignore

---

## Tecnologías

•⁠  ⁠*Python 3.11*
•⁠  ⁠*Análisis de datos:* pandas, numpy  
•⁠  ⁠*Visualización:* matplotlib, seaborn  
•⁠  ⁠*Econometría:* statsmodels, linearmodels  
•⁠  ⁠*Machine learning:* scikit-learn  
•⁠  ⁠*Reducción dimensional:* PCA  
•⁠  ⁠*Control de versiones:* Git + GitHub  

---

## Instalación
```bash
git clone https://github.com/mariaduquelaredo/TFG---Maria-Duque
cd DATOS_TFG
python -m venv .venv         # Crear entorno virtual
source .venv/bin/activate    # Activar entorno para MAC/Linux
.venv\Scripts\activate       # Activar entorno para Windows
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels linearmodels # Instalar dependencias
```
---

## Orden de ejecución

1. Ingeniería de datos          # Genera los dataset limpios en processed
•⁠  ⁠IngenieriaDatosBase1.ipynb
•⁠  ⁠⁠IngenieriaDatosBase2.ipynb 

2. Análisis de datos
•⁠  ⁠ModelosSupervisadosBase1.ipynb      # Modelos de panel + validación econométrica
•⁠  ⁠⁠ModelosNoSupervisadosBase2.ipynb    # K-Means, Clustering Jerárquico y PCA

---

## Resultados Principales
•⁠  ⁠Relación positiva entre renta y rendimiento educativo
•	Impacto significativo del nivel educativo de la población
•	El género es el factor más determinante
•	Identificación de clusters regionales diferenciados
•	Evidencia de desigualdad territorial estructural

---

## Control de versiones

Se ha gestionado con GitHub permitiendo: 
•⁠  ⁠Seguimiento del desarrollo mediante commits
•⁠  ⁠⁠Control de versiones del código
•⁠  ⁠Transparencia del proceso

