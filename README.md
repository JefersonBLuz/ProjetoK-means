# Implementação e Análise do Algoritmo de K-means
Reconhecimento de Atividade Humana com Dados de Smartphones


## 📋Objetivo do Projeto

Este projeto tem como objetivo implementar o algoritmo de agrupamento K-means para análise e reconhecimento de padrões no dataset Human Activity Recognition Using Smartphones. O foco está em aplicar técnicas de redução de dimensionalidade, agrupar as atividades humanas com base nas variáveis fornecidas e avaliar a performance do modelo por meio de métricas adequadas.

## 🛠️ Instruções para Executar o Código

### 1. Carregue o Arquivo Notebook
Faça upload do arquivo ProjetoTIC36_KMeans.ipynb para o Google Drive.
Abra o notebook diretamente no Colab ou faça o upload do arquivo local para o ambiente Colab.

### 2. Certifique-se de que você tem o Python e os pacotes necessários instalados.

Requisitos:

    Python 3.7+
    Pandas
    NumPy
    Matplotlib
    Seaborn
    Scikit-learn
    SciPy

##### 3. Instale as Bibliotecas Necessárias (se necessário)

No Colab, você pode instalar as bibliotecas necessárias executando o seguinte comando no início do notebook:

    !pip install numpy pandas matplotlib seaborn scikit-learn scipy gdown

### 4. Baixe e extraia o dataset.

O código já está configurado para baixar automaticamente o dataset do Google Drive:

    !gdown '1Q_2S28BQRsGAm105ORcqXDGR0spydsCq' --output 'UCI HAR Dataset.zip'
    !unzip 'UCI HAR Dataset.zip'

### 5. Execute as Células do Notebook

Siga as seções do notebook para:
    Importar bibliotecas.
    Realizar a análise exploratória dos dados.
    Implementar o algoritmo K-means.
    Avaliar o modelo com gráficos de dispersão, curvas de inércia e Silhouette Score.
    
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

Jeferson Braga Luz,

Rafael Rodrigues Souza

## 📌 Dicas Adicionais para o Google Colab

Caso deseje salvar o notebook com os resultados no seu Google Drive, selecione Arquivo > Salvar uma cópia no Drive.
Para baixar arquivos, use o comando:

    from google.colab import files
    files.download('Relatorio_KMeans_HAR.pdf')
