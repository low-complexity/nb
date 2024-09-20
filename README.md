## Análise de Dados Neurofisiológicos em Tarefas em Qualidade de Código

Notebook Jupyter com código em R para análise de dados neurofisiológicos coletados durante a realização de tarefas de análise de código. O objetivo principal é investigar a influência do uso de LLMs (Modelos de Linguagem Ampla) e de blends (misturas de diferentes tipos de informação) no desempenho e nas respostas neurofisiológicas dos participantes.

**Dataset:**

O notebook utiliza dois datasets:

* **Tarefas de Baixa Complexidade:** Contém dados de participantes realizando tarefas de análise de código relativamente simples.
* **Tarefas de Alta Complexidade:** Contém dados de participantes realizando tarefas de análise de código mais complexas.

**Análises Realizadas:**

O notebook realiza as seguintes análises:

1. **Normalização de Dados:** As variáveis neurofisiológicas (duração da fixação ocular, contagem da fixação ocular, amplitude do movimento sacádico e diâmetro da pupila) são normalizadas para evitar o efeito de escalas diferentes.
2. **Visualização de Dados:**
    * **Gráficos de Densidade:** Comparação da distribuição das variáveis neurofisiológicas entre as diferentes condições experimentais (com/sem LLM e com/sem blend).
    * **Boxplots:** Comparação da distribuição das variáveis neurofisiológicas e das escalas de ansiedade e autoeficácia entre as diferentes condições experimentais.
    * **Mapas de Calor:** Visualização da média das variáveis neurofisiológicas para cada combinação de condição experimental.
    * **Matriz de Correlação:**  Exibe a correlação entre todas as variáveis (neurofisiológicas, de desempenho nas tarefas e escalas), com ajuste de p-values para identificar correlações estatisticamente significativas.
3. **ANOVA:**  Realiza uma análise de variância (ANOVA) de dois fatores (LLM e blend) para cada tarefa, a fim de verificar se há diferenças significativas no desempenho entre as condições experimentais. O exemplo fornecido demonstra a ANOVA para a primeira tarefa.
4. **Tamanho do Efeito:** Calcula o tamanho do efeito (eta-quadrado) para a ANOVA, a fim de quantificar a magnitude do efeito das variáveis independentes na variável dependente.

**Observações:**

* O código está bem documentado e organizado em funções para facilitar a compreensão e reutilização.
* O notebook inclui a instalação dos pacotes R necessários para a análise.
* O código é flexível e pode ser facilmente adaptado para analisar outros datasets com estrutura similar.

**Próximos Passos:**

* Realizar análises estatísticas mais aprofundadas, como testes post-hoc para identificar as diferenças específicas entre as condições experimentais.
* Investigar a relação entre as variáveis neurofisiológicas e o desempenho nas tarefas, utilizando técnicas como regressão.
* Explorar outras variáveis e fatores que podem influenciar o desempenho e as respostas neurofisiológicas dos participantes.

**Contribuições:**

Contribuições para este repositório são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com sugestões de melhorias ou novas análises.
