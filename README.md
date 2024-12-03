# Implementação e Análise do Algoritmo de K-means
Reconhecimento de Atividade Humana com Dados de Smartphones
##📋Objetivo do Projeto

Este projeto tem como objetivo implementar o algoritmo de agrupamento K-means para análise e reconhecimento de padrões no dataset Human Activity Recognition Using Smartphones. O foco está em aplicar técnicas de redução de dimensionalidade, agrupar as atividades humanas com base nas variáveis fornecidas e avaliar a performance do modelo por meio de métricas adequadas.

##🛠️ Instruções para Executar o Código
###1. Clone ou baixe este repositório.

git clone https://github.com/seuprojeto/kmeans-har.git
cd kmeans-har

###2. Certifique-se de que você tem o Python e os pacotes necessários instalados.

Requisitos:

    Python 3.7+
    Pandas
    NumPy
    Matplotlib
    Seaborn
    Scikit-learn
    SciPy
    fpdf (para geração do relatório técnico)

Você pode instalar os pacotes necessários com o seguinte comando:

pip install numpy pandas matplotlib seaborn scikit-learn scipy fpdf

###3. Execute o notebook ou script Python.

jupyter notebook projeto_kmeans_har.ipynb

###4. Baixe e extraia o dataset.

O código já está configurado para baixar automaticamente o dataset do Google Drive:

!gdown '1Q_2S28BQRsGAm105ORcqXDGR0spydsCq' --output 'UCI HAR Dataset.zip'
!unzip 'UCI HAR Dataset.zip'

###5. Siga as seções do notebook para:

    Realizar a análise exploratória.
    Implementar e ajustar o algoritmo K-means.
    Avaliar os resultados com gráficos de dispersão, curvas de inércia, e Silhouette Score.
    Gerar um relatório técnico em PDF com os principais resultados.
