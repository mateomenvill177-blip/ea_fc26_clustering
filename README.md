# ⚽ Perfiles Tácticos en EA FC 26 — Clustering de Jugadores

## Pregunta de investigación
¿Existen perfiles tácticos diferenciados entre los jugadores de campo en EA FC 26, y qué habilidades físicas y técnicas caracterizan a cada perfil?

## Enfoque
Aprendizaje no supervisado (Clustering). No existe variable objetivo: el algoritmo descubre agrupaciones naturales a partir de 26 habilidades tácticas numéricas.

## Dataset
- **Fuente:** EA FC 26 — estadísticas de jugadores de campo
- **Filas:** 14,412 jugadores
- **Variables usadas:** 26 habilidades tácticas (velocidad, ataque, pase, regate, defensa)

## Resultados principales
Se identificaron **4 perfiles tácticos**:

| Cluster | Perfil | Ejemplos |
|---------|--------|---------|
| 0 | Atacantes Completos | Mbappé, Haaland, Salah |
| 1 | Jugadores de Bajo Perfil | Ligas menores y reservas |
| 2 | Defensores Puros | Tah, Le Normand, Min-jae Kim |
| 3 | Mediocampistas Completos | Rodri, Bellingham, Van Dijk |

**Mejor modelo:** K-Means (K=4) con Silhouette Score = 0.2011 vs Jerárquico = 0.1307

## Estructura del repositorio
```
├── ea_fc26_clustering.ipynb   # Notebook principal
├── ea_fc26_outfield.csv       # Dataset
├── requirements.txt           # Dependencias
└── README.md                  # Este archivo
```

## Cómo reproducir el análisis

### 1. Clonar el repositorio
```bash
git clone https://github.com/TU_USUARIO/TU_REPO.git
cd TU_REPO
```

### 2. Instalar dependencias
```bash
pip install -r requirements.txt
```

### 3. Abrir el notebook
```bash
jupyter notebook ea_fc26_clustering.ipynb
```

### 4. Ejecutar
En Jupyter: **Kernel → Restart & Run All**

El notebook corre de principio a fin sin errores en un entorno con Python 3.9+.

## Librerías utilizadas
`pandas` · `numpy` · `matplotlib` · `seaborn` · `scikit-learn` · `scipy`

## Autor
Proyecto final — Curso III: Modelado predictivo, automatización y proyectos inteligentes
