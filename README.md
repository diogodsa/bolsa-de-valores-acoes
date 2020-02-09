# Descrição do projeto
Código Python para análise de correlação. Utilizando uma técnica de análise multivariada que identifica um número menor de fatores que podem representar relações entre variáveis que estão inter relacionadas.

# PCA - Principal Component Analisys 
Variáveis que apresentam correlação expressiva compartilham algum fator em comum que pode substituí-las, preservando um bom percentual da variabilidade dos dados originais. O PCA aplica-se apenas para variáveis numéricas.

# Bibliotecas
import numpy as np
import pandas as pd
import scipy

import matplotlib.pyplot as plt
import seaborn as sns
sns.set()

from sklearn.preprocessing import StandardScaler

from scipy.cluster.hierarchy import dendrogram, linkage
from sklearn.cluster import KMeans
from sklearn.decomposition import PCA

# Importando os dados
df_segmentation = pd.read_excel('balanco-ativos-b3.xlsx', index_col = 0)

# Explorando os dados
df_segmentation.head()

https://colab.research.google.com/drive/1IUSDlNFBCjLUqsKTAKrEqGJaaeOsnl3I#scrollTo=1EjyJlSCX6HM
