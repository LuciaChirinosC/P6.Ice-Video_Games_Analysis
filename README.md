# Ice-Video_Games_Analysis-P6

## 🎮 Ice Video Games Analysis 
### 🧾 Descripción

Proyecto integrado que reúne lo aprendido: análisis de ventas de videojuegos (datos hasta 2016) para identificar patrones de éxito, preparar datos y construir análisis estadísticos y pruebas de hipótesis. Trabajo realizado en Jupyter Notebook.

### 📁 Dataset

Archivo: /datasets/games.csv
Columnas principales: name, platform, year_of_release, genre, na_sales, eu_sales, jp_sales, other_sales, critic_score, user_score, rating.

### 🎯 Objetivos

  - Limpiar y preparar el dataset (tipos, valores ausentes, TBD).

  - Calcular ventas totales por juego.

  - Analizar evolución por año y por plataforma.

  - Investigar relación entre reseñas (critic/user) y ventas.

  - Crear perfiles por región (NA, EU, JP).

  - Probar hipótesis estadísticas sobre ratings.

### 🛠 Estructura del notebook (resumida)

  - Carga y revisión: lectura de /datasets/games.csv, head(), info().

#### Preprocesamiento:

  - Normalizar nombres de columnas (minúsculas).

  - Convertir tipos (fechas numéricas, scores).

  - Manejar TBD y missing: documentar decisión.

  - Crear columna global_sales = na_sales + eu_sales + jp_sales + other_sales.

#### Análisis exploratorio:

  - Juegos por año; elegir periodo relevante para modelar 2017.

  - Ventas por plataforma (top plataformas, evolución temporal).

  - Boxplots y histogramas por plataforma.

#### Correlación:

  - Scatter plot y coeficiente entre critic_score/user_score y global_sales.

#### Perfiles regionales (NA, EU, JP):

  - Top 5 plataformas y géneros por región; comparar cuotas.

  - Impacto de rating por región.

#### Pruebas de hipótesis:

  - H1: medias de user_score en Xbox One vs PC (nula/alternativa, α).

  - H2: medias de user_score en géneros Acción vs Deportes.

  - Documentar método (t-test, o no paramétrico) y conclusiones.

Conclusión: resumen ejecutivo y recomendaciones (marketing / plataformas a priorizar).

📎 Sugerencias rápidas

Tratar user_score que sea 'TBD' o missing como NaN y justificar por qué imputas o eliminas.

Para años con pocos datos (ej. 2016), documentar si se excluyen del modelo.

Usar muestras y visualizaciones limpias para la presentación final.
