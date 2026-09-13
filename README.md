[README.md](https://github.com/user-attachments/files/32150172/README.md)
# Mini-Projeto 2 — Pipeline Preditivo Multiclasse

**Autor:** Fábio Rodrigues Spiazzi

## Objetivo
Construir, treinar, validar, comparar e testar um pipeline de classificação de dígitos manuscritos utilizando o dataset **MNIST (`mnist_784`)**.

## Conteúdo do notebook
O projeto está organizado nas seguintes fases:

1. **Carregamento e pré-processamento**
   - Download do MNIST via `scikit-learn`;
   - Separação entre entradas (`X`) e rótulos (`y`);
   - Verificação das dimensões e do balanceamento das classes;
   - Visualização de exemplos dos dígitos.

2. **Divisão e normalização dos dados**
   - Divisão estratificada em treino, validação e teste;
   - Normalização dos pixels para a escala `[0, 1]`;
   - Justificativa da importância do escalonamento.

3. **Treinamento dos modelos**
   - Random Forest;
   - XGBoost;
   - Rede neural MLP;
   - Busca de hiperparâmetros e treinamento com os melhores parâmetros.

4. **Avaliação comparativa**
   - Matrizes de confusão;
   - Relatórios de classificação;
   - Análise das maiores confusões entre dígitos;
   - Comparação das métricas e identificação do modelo de melhor desempenho.

5. **Testes de generalização**
   - Treinamento com classes ocultadas (*class masking*);
   - Teste com classes ausentes no treinamento (*out-of-distribution*);
   - Inferência em imagens manuscritas próprias.

## Como executar

1. Clone ou baixe este repositório.
2. Crie um ambiente virtual Python.
3. Instale as dependências:

```bash
pip install -r requirements.txt
```

4. Abra o notebook:

```bash
jupyter notebook MiniProjeto_2_SCTEC_Fábio_R_Spiazzi.ipynb
```

Também é possível executar o arquivo diretamente no Google Colab. Execute as células na ordem apresentada, pois as etapas dependem dos objetos criados anteriormente.

## Observações
- O dataset MNIST é baixado durante a execução.
- O treinamento de XGBoost e da rede neural pode exigir mais tempo e memória.
- Para reproduzir os resultados, mantenha as mesmas divisões dos dados e os parâmetros definidos no notebook.
- Link de apresentação: https://drive.google.com/file/d/1B3fh-0RwrR1be7QGirclD-M_BT9MkxiD/view?usp=sharing
