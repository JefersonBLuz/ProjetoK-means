# Implementação e Análise do Algoritmo de K-means
Reconhecimento de Atividade Humana com Dados de Smartphones


## 📋Objetivo do Projeto

Este projeto tem como objetivo implementar o algoritmo de agrupamento K-means para análise e reconhecimento de padrões no dataset Human Activity Recognition Using Smartphones. O foco está em aplicar técnicas de redução de dimensionalidade, agrupar as atividades humanas com base nas variáveis fornecidas e avaliar a performance do modelo por meio de métricas adequadas.

## 🛠️ Instruções para Executar o Código

### 1. Clone ou baixe este repositório.

    git clone https://github.com/seuprojeto/kmeans-har.git
    cd kmeans-har

### 2. Certifique-se de que você tem o Python e os pacotes necessários instalados.

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

### 3. Execute o notebook ou script Python.

    jupyter notebook projeto_kmeans_har.ipynb

### 4. Baixe e extraia o dataset.

O código já está configurado para baixar automaticamente o dataset do Google Drive:

    !gdown '1Q_2S28BQRsGAm105ORcqXDGR0spydsCq' --output 'UCI HAR Dataset.zip'
    !unzip 'UCI HAR Dataset.zip'

## 📊 Principais Conclusões e Considerações

#### Distribuição e Correlação dos Dados:
As variáveis apresentam padrões específicos que foram explorados por meio da análise de distribuição e matriz de correlação.
A redução dimensional com PCA permitiu visualizar melhor os agrupamentos iniciais.

#### Definição do Número de Clusters:
O número ideal de clusters foi definido como k=6 com base no método do cotovelo e no Silhouette Score.
Os clusters apresentaram uma separação satisfatória em 2D, indicando que as atividades humanas podem ser agrupadas de maneira coerente com base nas   características do dataset.

#### Avaliação de Performance:
O Silhouette Score final obteve um valor satisfatório, sugerindo que os agrupamentos formados possuem boa coesão interna e separação externa.
A repetição do K-means várias vezes confirmou a estabilidade dos agrupamentos.

#### Limitações:
O dataset foi reduzido para duas dimensões com PCA, o que pode simplificar demais a complexidade dos dados originais.
Algumas atividades podem ter sobreposição em 2D, sugerindo que outras técnicas de clustering e mais componentes principais podem melhorar os resultados.

### 👥 Autores

Grupo 24

Jeferson Braga Luz
Rafael Rodrigues Souza
