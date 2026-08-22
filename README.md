# 📊 YouTube en LATAM y su relación con la felicidad

Análisis exploratorio de datos (EDA) que cruza el uso de YouTube en países de Latinoamérica
con el World Happiness Report 2024 y datos de uso general de redes sociales, para responder:

1. ¿Cómo varía el uso de YouTube entre los países de LATAM?
2. ¿Hay relación entre la penetración de YouTube y el puntaje de felicidad de un país?
3. ¿Qué países tienen alto potencial pero baja penetración de YouTube frente al uso general de redes? (Índice de Oportunidad Digital)

## 🖼️ Vista previa

| Uso de YouTube en LATAM | Penetración vs. Felicidad | Índice de Oportunidad Digital |
|---|---|---|
| `outputs/figures/01_youtube_latam.png` | `outputs/figures/02_penetracion_vs_felicidad.png` | `outputs/figures/03_indice_oportunidad_digital.png` |

*(Las imágenes se generan al correr el notebook; no están versionadas en el repo.)*

## 📁 Estructura del proyecto

```
youtube-latam-happiness/
├── README.md                     <- este archivo
├── requirements.txt               <- librerías necesarias
├── data/
│   └── README.md                  <- de dónde descargar los datasets
├── notebooks/
│   └── 01_analisis_youtube_latam.ipynb   <- notebook principal
└── outputs/
    └── figures/                   <- gráficos exportados (se generan al correr el notebook)
```

## 🚀 Cómo correrlo

1. Cloná el repositorio:
   ```bash
   git clone https://github.com/TU-USUARIO/youtube-latam-happiness.git
   cd youtube-latam-happiness
   ```

2. Creá un entorno virtual e instalá las dependencias:
   ```bash
   python -m venv venv
   source venv/bin/activate   # En Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Descargá los datasets siguiendo las instrucciones de [`data/README.md`](data/README.md)
   y colocalos dentro de la carpeta `data/`.

4. Abrí el notebook:
   ```bash
   jupyter notebook notebooks/01_analisis_youtube_latam.ipynb
   ```

## 🛠️ Tecnologías usadas

- Python 3.10+
- pandas, numpy
- matplotlib, seaborn
- scikit-learn (MinMaxScaler)

## 📈 Principales hallazgos

- La penetración de YouTube varía considerablemente entre países de LATAM, sin relación
  directa con el tamaño poblacional.
- Correlación de Pearson de **~0.52** entre penetración de YouTube y felicidad (Life Ladder):
  relación positiva moderada, no necesariamente causal.
- El Índice de Oportunidad Digital identifica países con buen desarrollo socioeconómico pero
  relativamente baja penetración de YouTube — posibles mercados con espacio de crecimiento.

## 📄 Fuentes de datos

- [YouTube Users by Country 2025](https://www.kaggle.com/datasets/arpitsinghaiml/youtube-user-by-country-2025) — Kaggle
- [World Happiness Report 2024](https://www.kaggle.com/datasets/jainaru/world-happiness-report-2024-yearly-updated) — Kaggle
- [Social Media Users by Country](https://www.kaggle.com/datasets/edissoniiguez/social-media-users) — Kaggle

## ✍️ Autor

Proyecto realizado originalmente en Kaggle como ejercicio de análisis exploratorio de datos.

## 📜 Licencia

Este proyecto se comparte bajo licencia MIT (ver `LICENSE`). Los datasets utilizados conservan
sus licencias originales de Kaggle — revisá cada una antes de redistribuirlos.
