# 🎵 OracleIA - Predictor de Popularidad Musical 

Un análisis completo de machine learning para predecir la popularidad de canciones y detectar hits de verano utilizando datos de Spotify.

##  Descripción 

**OracleIA** es un proyecto de ciencia de datos que implementa múltiples modelos de machine learning para analizar y predecir la popularidad de canciones musicales. El proyecto incluye dos enfoques principales:

1. **Predicción de Popularidad General**: Modelos de regresión y clasificación para predecir qué tan popular será una canción
2. **Predictor de Hits de Verano**: Modelo especializado en identificar canciones con potencial para convertirse en éxitos durante el verano

## ¿Qué hemos hecho? 
1º Hemos **comparado 8 modelos candidatos** para ser usados en el modelo final, saliendo vencedores el Gradient Boosting Classifier (Random Search) (mejor clasificador) (Accuracy: 82.82%) y el Random Forest Regressor (Grid Search) (mejor regresor) (MAE: 10.6494). Estos resultados son de pruebas anteriores, por lo que pueden variar ligeramente del resultado en el cuaderno, también hemos decidido usar el Gradient Boosting Classifier, porque en pruebas anteriores fue superior al Random Forest Classifier.

2º Luego hemos usado **los 2 modelos ganadores en nuestra IA para predecir hits del verano**, y la hemos entrenado. También hemos identificado las características claves para un hit del verano. 

![imagen](https://github.com/user-attachments/assets/098b4292-415e-4c7a-9d11-c1dcce51aa2d)


![imagen](https://github.com/user-attachments/assets/f9a499a1-016d-4a5b-9500-0162f6196e99)


3º Hemos **corregido algunos parámetros y ajustado la precisión** del modelo. 

4º Hemos hecho una **batería de pruebas** para testear su funcionamiento.

## 📊 Métricas de Evaluación

### Para Clasificación
- **Accuracy**: Precisión general del modelo
- **Precision**: Precisión de predicciones positivas
- **Recall**: Cobertura de casos positivos
- **F1-Score**: Media armónica de precision y recall

### Para Regresión
- **MAE (Mean Absolute Error)**: Error absoluto medio
- **MSE (Mean Squared Error)**: Error cuadrático medio
- **RMSE (Root Mean Squared Error)**: Raíz del error cuadrático medio

## Características Principales

###  Análisis de Popularidad Musical
- Análisis exploratorio completo de datos musicales
- Procesamiento de características de audio de Spotify
- Comparación de múltiples algoritmos de machine learning
- Visualizaciones interactivas y análisis estadístico

###  Predictor de Hits de Verano
- Modelo especializado para identificar canciones de verano
- Características personalizadas basadas en patrones estacionales
- Análisis de factores que contribuyen al éxito estival
- Métricas de evaluación específicas para hits de verano

##  Modelos Implementados

### Modelos de Clasificación
- **Random Forest Classifier** (Grid Search y Random Search)
- **Gradient Boosting Classifier** (Grid Search y Random Search)

### Modelos de Regresión
- **Random Forest Regressor** (Grid Search y Random Search)
- **Gradient Boosting Regressor** (Grid Search y Random Search)

## 🛠️ Tecnologías Utilizadas

```python
- pandas          # Manipulación de datos
- scikit-learn    # Machine learning
- matplotlib      # Visualización
- seaborn         # Visualización estadística
- numpy           # Operaciones numéricas
```


## 📈 Resultados del Análisis

### 🏆 Mejores Modelos Encontrados

#### Clasificación (Predicción Binaria de Popularidad)
- **Mejor Modelo**: Gradient Boosting Classifier (Random Search)
- **Accuracy**: 82.8%
- **Precision**: 82.8%

#### Regresión (Predicción Continua de Popularidad)
- **Mejor Modelo**: Random Forest Regressor (Grid Search)
- **MAE**: 10.65 puntos
- **RMSE**: 15.28 puntos

#### Predictor de Hits de Verano
- **Modelo**: Gradient Boosting Classifier optimizado
- **Accuracy**: 97.2%
- **Precision**: 96.9%
- **F1-Score**: 60.9%

###  Características Más Importantes

1. **track_genre_encoded** (18.25%) - Género musical
2. **summer_index** (13.20%) - Índice de verano personalizado
3. **acousticness** (6.78%) - Nivel acústico
4. **duration_ms** (6.13%) - Duración de la canción
5. **loudness** (6.11%) - Volumen/intensidad

##  Funcionalidades Destacadas

###  Análisis Exploratorio
- Distribución de popularidad por géneros
- Correlaciones entre características musicales
- Visualizaciones interactivas de patrones

###  Características de Verano Personalizadas
- **summer_index**: Índice compuesto para hits de verano
- **energy_valence_ratio**: Relación energía/valencia
- **dance_energy_combo**: Combinación danceabilidad-energía
- **positive_dance_factor**: Factor de positividad bailable
- **radio_friendly_duration**: Duración amigable para radio

###  Optimización de Hiperparámetros
- **Grid Search**: Búsqueda exhaustiva de parámetros
- **Random Search**: Búsqueda aleatoria optimizada
- **Cross-Validation**: Validación cruzada de 5 folds

##  Visualizaciones Incluidas

-  Histogramas de distribución de popularidad
-  Gráficos de correlación entre características
-  Comparación de rendimiento de modelos
-  Heatmaps de importancia de características
-  Análisis de hits de verano vs canciones regulares


