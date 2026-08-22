# Datasets

Los archivos CSV **no están incluidos** en este repositorio (por tamaño y para respetar las
licencias originales de Kaggle). Descargalos manualmente y colocalos en esta carpeta con estos
nombres exactos, para que el notebook los encuentre sin modificar rutas:

| Archivo esperado en `data/` | Fuente |
|---|---|
| `youtube-users-by-country-2025.csv` | [Kaggle: YouTube Users by Country 2025](https://www.kaggle.com/datasets/arpitsinghaiml/youtube-user-by-country-2025) |
| `world-happiness-report-updated_2024.csv` | [Kaggle: World Happiness Report 2024](https://www.kaggle.com/datasets/jainaru/world-happiness-report-2024-yearly-updated) |
| `usuarios-de-redes-sociales-por-pais-en-2026.csv` | [Kaggle: Social Media Users by Country](https://www.kaggle.com/datasets/edissoniiguez/social-media-users) |

## Cómo descargar desde Kaggle

1. Necesitás una cuenta de Kaggle (gratis).
2. Entrá al link del dataset y hacé clic en **Download**.
3. Descomprimí el `.zip` si hace falta y movés el `.csv` a esta carpeta `data/`.

### Alternativa: usando la API de Kaggle (opcional, más rápido)

```bash
pip install kaggle
# Configurá tu kaggle.json (ver https://www.kaggle.com/docs/api)
kaggle datasets download -d arpitsinghaiml/youtube-user-by-country-2025 -p data/ --unzip
kaggle datasets download -d jainaru/world-happiness-report-2024-yearly-updated -p data/ --unzip
kaggle datasets download -d edissoniiguez/social-media-users -p data/ --unzip
```

> ⚠️ Los nombres de archivo que trae cada dataset pueden variar levemente; renombralos según
> la tabla de arriba si es necesario.
