# Google Colab
Análise de Dados Fisiológicos e Psicológicos em R

# Análise de Dados Fisiológicos e Psicológicos em R

Este notebook tem como objetivo realizar uma análise de dados fisiológicos e psicológicos, utilizando o R para realizar correlações e visualizações de dados de um estudo acadêmico. Ele foi desenvolvido para facilitar a análise de variáveis como EDA (Atividade Eletrodérmica), ECG (Frequência Cardíaca), EEG (Atividade Cerebral), além de escores de questionários como STAI e SPSES. Abaixo estão descritas as principais funcionalidades deste notebook.

## Funcionalidades

### 1. **Análise Descritiva**
O notebook realiza uma análise descritiva inicial, calculando estatísticas como média, desvio padrão, skewness e kurtosis para variáveis contínuas. Também é feita uma análise de frequência para variáveis categóricas, como *Condition* e *Participant* [[5]](https://poe.com/citation?message_id=252043470924&citation=5).

- Exibe resumo estatístico das variáveis.
- Calcula skewness e kurtosis para verificar a simetria e a curtose das distribuições.
- Gera tabelas de frequência para variáveis categóricas.

### 2. **Correlação entre Variáveis**
O notebook calcula a correlação de Pearson e Spearman entre variáveis-chave do estudo, como os escores de questionários STAI e SPSES, além de variáveis fisiológicas (EDA, ECG, EEG) [[3]](https://poe.com/citation?message_id=252043470924&citation=3).

- Cálculo da correlação de Pearson e Spearman entre variáveis contínuas.
- Exibe uma matriz de correlação entre os principais indicadores.

### 3. **Visualizações de Dados**
O notebook oferece uma variedade de visualizações para analisar a distribuição e a relação entre as variáveis. As principais visualizações incluem:

- **Gráficos de Violino:** Visualização da distribuição de variáveis contínuas (ex: EDA_mean e ECG_HR) por condição e ao longo do tempo [[2]](https://poe.com/citation?message_id=252043470924&citation=2).
- **Boxplots:** Exibição de outliers e variações nas distribuições de ECG_HR e escores de questionários por condição [[4]](https://poe.com/citation?message_id=252043470924&citation=4).
- **Gráficos de Densidade:** Visualização da distribuição de EEG Alpha e Beta ao longo do tempo e por condição [[2]](https://poe.com/citation?message_id=252043470924&citation=2).
- **Mapas de Calor:** Exibição da matriz de correlação entre variáveis fisiológicas e psicológicas [[5]](https://poe.com/citation?message_id=252043470924&citation=5).
- **Gráficos Interativos:** Gráficos de dispersão interativos com *plotly* para explorar as relações entre variáveis fisiológicas [[6]](https://poe.com/citation?message_id=252043470924&citation=6).

### 4. **Testes Estatísticos**
O notebook implementa testes estatísticos como a ANOVA de medidas repetidas para avaliar diferenças estatisticamente significativas entre as condições experimentais, utilizando pacotes como `ezANOVA` [[1]](https://poe.com/citation?message_id=252043470924&citation=1).

- Realiza ANOVA de medidas repetidas para comparar condições.
- Exibe resultados estatísticos detalhados.

### 5. **Filtros de Sinal**
Para sinalizações fisiológicas contínuas, como EEG, o notebook implementa filtros de passa-faixa para remover ruídos e isolar as frequências de interesse. Isso é especialmente útil na análise de dados EEG [[4]](https://poe.com/citation?message_id=252043470924&citation=4)[[6]](https://poe.com/citation?message_id=252043470924&citation=6).

- Aplica filtros passa-faixa para sinais fisiológicos.
- Gera sinais filtrados para análises subsequentes.

## Requisitos

Para executar este notebook, é necessário ter os seguintes pacotes instalados no seu ambiente de R:

- `dplyr`
- `ggplot2`
- `readr`
- `ez`
- `signal`
- `plotly`
- `reshape2`
- `moments`

O código para instalação dos pacotes está incluído no notebook.

## Como Usar

1. Clone este repositório para seu ambiente local.
2. Abra o notebook no Google Colab ou em um ambiente compatível com R.
3. Execute as células do notebook sequencialmente para gerar as análises e visualizações.
4. Insira seus próprios dados (substituindo o dataset fictício) para realizar a análise com seus dados experimentais.

## Estrutura dos Dados

Os dados utilizados neste notebook devem seguir o seguinte formato:

- **Participant:** Identificador único para cada participante.
- **Condition:** Condição experimental (ex: grupos de controle e experimental).
- **EDA_mean, ECG_HR, EEG_alpha, EEG_beta:** Variáveis fisiológicas coletadas ao longo do tempo.
- **STAI_score, SPSES_score:** Escores de questionários psicológicos para medir ansiedade e autoeficácia.

## Contribuições

Sinta-se à vontade para sugerir melhorias ou abrir *issues* relacionadas ao código ou à análise estatística. Pull requests são bem-vindos.
