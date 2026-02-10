# Problem_management
Descubrir patrones repetitivos de incidentes usando técnicas de clustering (como K-means o DBSCAN) para ayudar a un equipo de Problem Management a:  Identificar causas raíz más rápido Detectar problemas recurrentes Proponer mejoras preventivas basadas en datos
Cargar librerías y datos
Exploración (EDA) con conteos por prioridad y categoría + gráficos.
Ingeniería de características:

resolution_time_hours (horas de resolución)
Variables temporales: hora, dia_semana, es_fin_de_semana
priority_ord (mapeo P1→1, … P4→4)
One-Hot Encoding de categóricas.


Preparación y escalado con StandardScaler.
K-Means:

Selección de K con método del codo e índice silhouette.
Entrenamiento y visualización 2D (PCA).


Perfilado de clústeres:

Métricas numéricas por clúster (medianas y medias).
Top categorías / subcategorías / departamentos / grupos por clúster.


DBSCAN:

Estimación de eps (gráfico k-dist).
Entrenamiento, visualización PCA y clases (incluye ruido = -1).


Insights automáticos y recomendaciones por clúster.
Exportación de resultados:

incidentes_clusterizados_kmeans.csv
perfil_clusters_kmeans.csv
