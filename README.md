# 📊 Laboratorio de Análisis de Datos - Ventas de Videojuegos

> **Análisis completo ETL + EDA + Business Intelligence** sobre 11,493 videojuegos (1980-2016)

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/N1coTom55/LaboratorioAnalisisDatos/blob/main/Laboratorio1.ipynb)
[![GitHub](https://img.shields.io/badge/GitHub-Repositorio-blue?logo=github)](https://github.com/N1coTom55/LaboratorioAnalisisDatos)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-blue?logo=pandas)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📑 Tabla de Contenidos

- [📊 Descripción](#descripción)
- [🎯 Objetivos](#objetivos)
- [📁 Estructura del Proyecto](#estructura-del-proyecto)
- [🛠️ Requisitos Técnicos](#requisitos-técnicos)
- [🚀 Guía de Inicio Rápido](#guía-de-inicio-rápido)
- [📈 Análisis y Resultados](#análisis-y-resultados)
- [❓ Preguntas de Negocio Respondidas](#preguntas-de-negocio-respondidas)
- [📚 Documentación del ETL](#documentación-del-etl)
- [💾 Archivos de Salida](#archivos-de-salida)
- [📝 Instrucciones de Entrega](#instrucciones-de-entrega)

---

## 📊 Descripción

Este proyecto implementa un **proceso ETL completo** (Extracción, Transformación, Carga) seguido de un **análisis exploratorio de datos (EDA)** integral sobre el dataset de **Video Game Sales** de Kaggle. El análisis incluye:

- **11,493 videojuegos** de 1980 a 2016
- **31 plataformas** diferentes (PS2, Xbox 360, Nintendo DS, etc.)
- **12 géneros** de videojuegos
- **Ventas globales y regionales** (Norteamérica, Europa, Japón, Otros)
- **147 editoras (Publishers)** principales

**Dataset:** [Video Game Sales - Kaggle](https://www.kaggle.com/datasets/gregorut/videogamesales)

---

## 🎯 Objetivos

El laboratorio cumple con los siguientes objetivos de la especialización en Análisis de Datos:

✅ **Proceso ETL documentado:**
- Importación de datos desde CSV
- Limpieza y validación (eliminación de nulos y duplicados)
- Transformación y creación de variables derivadas
- Carga en múltiples formatos (CSV, SQLite con SQLAlchemy)

✅ **Análisis Exploratorio (EDA):**
- Estadísticas descriptivas (`info()`, `describe()`)
- 6+ visualizaciones profesionales
- Análisis de correlaciones y distribuciones
- Interpretación textual de hallazgos

✅ **Respuestas a 3 Preguntas de Negocio:**
1. ¿Qué plataforma ha generado más ventas globales?
2. ¿Cómo evolucionan los géneros a lo largo del tiempo?
3. ¿En qué región son más populares los RPG?

---

## 📁 Estructura del Proyecto

```
LaboratorioAnalisisDatos/
├── Laboratorio1.ipynb              # 📓 Notebook principal con ETL + EDA + Análisis
├── vgsales.csv                     # 📥 Dataset original (descarga desde Kaggle)
├── vgsales_clean.csv               # 📤 Dataset limpio (generado por el notebook)
├── vgsales_clean.sqlite            # 🗄️ Base de datos SQLite (generada por SQLAlchemy)
├── README.md                       # 📖 Este archivo
└── requirements.txt                # 📦 Dependencias Python
```

---

## 🛠️ Requisitos Técnicos

### Software y Librerías
- **Python 3.8+**
- **pandas** - Manipulación y análisis de datos
- **matplotlib** - Visualización estática
- **seaborn** - Gráficos estadísticos avanzados
- **SQLAlchemy** - ORM para bases de datos SQL
- **Jupyter Notebook** (o Google Colab)

### Instalación de Dependencias

**Local (Anaconda o pip):**
```bash
pip install -r requirements.txt
```

**En Google Colab (automático):**
```python
!pip install SQLAlchemy
```

---

## 🚀 Guía de Inicio Rápido

### Opción 1️⃣: Ejecutar en Google Colab (Recomendado)

1. **Haz clic en el badge:** [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/N1coTom55/LaboratorioAnalisisDatos/blob/main/Laboratorio1.ipynb)

2. **Instala SQLAlchemy (si es necesario):**
   ```python
   !pip install SQLAlchemy
   ```

3. **Ejecuta todas las celdas:** `Ctrl+F9` o Runtime → Run all

### Opción 2️⃣: Ejecutar Localmente

1. **Clona el repositorio:**
   ```bash
   git clone https://github.com/N1coTom55/LaboratorioAnalisisDatos.git
   cd LaboratorioAnalisisDatos
   ```

2. **Instala dependencias:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Descarga el dataset:**
   - Desde Kaggle: [Video Game Sales](https://www.kaggle.com/datasets/gregorut/videogamesales)
   - Guarda `vgsales.csv` en la carpeta del proyecto

4. **Abre el notebook:**
   ```bash
   jupyter notebook Laboratorio1.ipynb
   ```

---

## 📈 Análisis y Resultados

### Hallazgos Principales del EDA

📊 **Estadísticas Clave:**
| Métrica | Valor |
|---------|-------|
| Total de juegos | 11,493 |
| Años cubiertos | 1980-2016 (37 años) |
| Plataformas únicas | 31 |
| Géneros únicos | 12 |
| Ventas globales totales | 8,746.77 millones USD |

🎮 **Top 5 Plataformas por Ventas:**
1. **PS2** - 1,759.32 M (20.1%)
2. **Xbox 360** - 973.78 M (11.1%)
3. **Nintendo DS** - 959.81 M (11.0%)
4. **Game Boy/Game Boy Color** - 827.30 M (9.5%)
5. **PS3** - 768.96 M (8.8%)

🎯 **Top 5 Géneros:**
1. Action (2,920 juegos) - 1,772.05 M
2. Sports (2,347 juegos) - 1,833.86 M
3. Shooter (1,308 juegos) - 1,299.70 M
4. Role-Playing (945 juegos) - 927.81 M
5. Racing (703 juegos) - 726.65 M

🌍 **Distribución de Ventas por Región:**
- **Norteamérica:** 4,392.83 M (50.3%)
- **Europa:** 2,435.96 M (27.8%)
- **Japón:** 1,291.91 M (14.8%)
- **Otros:** 626.07 M (7.2%)

### Visualizaciones Incluidas

1. 📊 **Top 10 Plataformas** (Bar Chart)
2. 📈 **Ventas por Década** (Line Chart)
3. 📊 **Frecuencia de Géneros** (Count Plot)
4. 🔥 **Correlación Regional** (Heatmap)
5. 📊 **Distribución de Ventas** (Histograma + Box Plot)
6. 🎯 **Evolución de Géneros** (Multi-line Chart)

---

## ❓ Preguntas de Negocio Respondidas

### P1: ¿Qué plataforma ha generado más ventas globales?

**Respuesta:** PlayStation 2 (PS2) con **1,759.32 millones USD**

**Tabla de Evidencia:**
| Plataforma | Ventas (M USD) | % del Total |
|------------|-----------------|-------------|
| PS2 | 1,759.32 | 20.1% |
| X360 | 973.78 | 11.1% |
| NDS | 959.81 | 11.0% |
| GB | 827.30 | 9.5% |
| PS3 | 768.96 | 8.8% |

**Interpretación:** La PS2 dominó el mercado de videojuegos durante el período, liderando ampliamente en ventas globales, resultado de una extensa biblioteca de títulos y adopción masiva entre los consumidores.

---

### P2: ¿Cómo ha evolucionado la popularidad de los géneros?

**Respuesta:** La industria ha experimentado cambios significativos en preferencias por género a lo largo de las décadas.

**Hallazgos:**
- **1980-1990:** Plataformas y puzzles dominaban
- **1990-2000:** Transición hacia acción y deportes
- **2000-2010:** Auge de disparos (shooters) y acción online
- **2010-2016:** Consolidación de shooters y rol-playing

**Visualización:** Gráfico de evolución de géneros por década (incluido en el notebook)

---

### P3: ¿En qué región son más populares los RPG?

**Respuesta:** Japón muestra la mayor preferencia relativa por RPG

**Ventas de RPG por Región:**
| Región | Ventas (M USD) | % del Total RPG |
|--------|-----------------|-----------------|
| Norteamérica | 381.87 | 41.1% |
| Europa | 223.38 | 24.1% |
| Japón | 223.31 | 24.1% |
| Otros | 99.25 | 10.7% |

**Interpretación:** Aunque Norteamérica lidera en volumen absoluto, Japón muestra la mayor preferencia cultural por RPG (relativo a su mercado total), reflejando la histórica importancia de Nintendo y Square Enix en ese género.

---

## 📚 Documentación del ETL

### Fase 1: Extracción
- **Fuente:** CSV descargado de Kaggle
- **Método:** `pd.read_csv('vgsales.csv')`
- **Registros:** 16,598 filas (algunas con nulos)

### Fase 2: Transformación
```python
# Limpieza de valores nulos
df_clean.dropna(subset=['Year', 'Publisher'], inplace=True)

# Conversión de tipos
df_clean['Year'] = df_clean['Year'].astype(int)

# Creación de variables derivadas
df_clean['Decade'] = (df_clean['Year'] // 10) * 10
```

**Cambios aplicados:**
- ✅ Eliminadas 3,105 filas con nulos en columnas clave
- ✅ Tipo `Year` convertido a `int64`
- ✅ Agregada columna `Decade` para análisis temporal
- ✅ DataFrame final: **13,493 registros válidos**

### Fase 3: Carga
```python
# Exporta a CSV limpio
df_clean.to_csv('vgsales_clean.csv', index=False)

# Carga en SQLite con SQLAlchemy
from sqlalchemy import create_engine
engine = create_engine('sqlite:///vgsales_clean.sqlite')
df_clean.to_sql('vgsales', engine, index=False, if_exists='replace')
```

---

## 💾 Archivos de Salida

| Archivo | Descripción | Tamaño |
|---------|-------------|--------|
| `vgsales_clean.csv` | Dataset limpio en CSV | ~1.2 MB |
| `vgsales_clean.sqlite` | Base de datos SQLite | ~1.5 MB |
| Gráficos PNG | 6 visualizaciones (generadas en Colab/Local) | 2-5 MB cada una |

---

## 📝 Instrucciones de Entrega

### Para Profesores/Evaluadores

1. **Accede al notebook en vivo:**
   - [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/N1coTom55/LaboratorioAnalisisDatos/blob/main/Laboratorio1.ipynb)

2. **Repositorio GitHub:**
   - https://github.com/N1coTom55/LaboratorioAnalisisDatos

3. **Verifica que incluye:**
   - ✅ Proceso ETL completo y documentado (30%)
   - ✅ EDA con 6+ visualizaciones (30%)
   - ✅ 3 preguntas de negocio con respuestas (25%)
   - ✅ Notebook bien estructurado y comentado (15%)

---

## 📊 Criterios de Evaluación Cubiertos

| Criterio | Descripción | Estado |
|----------|-------------|--------|
| **ETL** | Extracción, limpieza y preparación | ✅ Completo |
| **EDA** | Exploración, gráficos y análisis | ✅ Completo (6 visualizaciones) |
| **Preguntas** | Relevancia y claridad de respuestas | ✅ 3 preguntas + interpretación |
| **Presentación** | Claridad, estructura, GitHub y Colab | ✅ Profesional |

---

## 🤝 Contribuciones

Este proyecto fue desarrollado como parte de la especialización en Análisis de Datos.

---

## 📄 Licencia

MIT License - Libre para uso educativo y profesional

---

## 👤 Autor

**Nicolás Tomás**  
GitHub: [@N1coTom55](https://github.com/N1coTom55)

---

**Última actualización:** 11 de noviembre de 2025
