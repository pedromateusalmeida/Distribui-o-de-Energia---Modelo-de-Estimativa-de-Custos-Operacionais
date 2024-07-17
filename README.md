# Distribuição de Energia - Modelo de Estimativa de Custos Operacionais

## Organização
**ANEEL - Agência Nacional de Energia Elétrica**

## Descrição do Projeto
Este repositório contém um projeto de análise de dados e modelagem preditiva com o objetivo de estimar os Custos Operacionais (PMSO) de empresas distribuidoras de energia elétrica no Brasil. Utilizamos dados médios de 52 empresas, coletados entre 2018 e 2020, abrangendo diversas variáveis relevantes para a operação dessas empresas. A análise e o modelo resultante visam apoiar a ANEEL na avaliação da eficiência operacional dessas empresas para o ano de 2023 e anos subsequentes.

## Base de Dados
O arquivo **ModeloVigente_DadosCP62_2023.xlsx** contém as seguintes variáveis:
- **Custos Operacionais (PMSO/Despesas com Pessoal, Materiais, Serviços e Outros – em R$ 1.000,00)**
- **Rede de alta tensão (Km)**
- **Rede subterrânea (Km)**
- **Rede de distribuição aérea (Km)**
- **Mercado ponderado (MWh – Mercado Atendido em termos de potência)**
- **Consumidores totais (unid)**
- **Consumidor Hora Interrompido - CHI (h – Tempo médio de consumidores sem energia)**
- **Perdas Não Técnicas - PNT (MWh – Energia perdida considerando fraudes, gatos, etc.)**

## Objetivo do Projeto
O principal objetivo deste projeto é desenvolver um modelo de regressão linear interpretável para estimar os Custos Operacionais (PMSO) com base nas demais variáveis do dataset, considerando tanto a relevância estatística das variáveis quanto a capacidade preditiva do modelo.

## Roteiro da Atividade

1. **Carregando Bibliotecas**
2. **Informações Básicas do Dataset**
    - Exibição das 5 primeiras linhas
    - Tipo de dado em cada coluna
    - Descrição estatística das colunas numéricas (contagem, média, mediana, desvio padrão)
    - Quantidade de linhas e colunas
    - Quantidade de variáveis categóricas
3. **Análise Exploratória**
    - Verificação de dados ausentes (missing)
    - Distribuição da variável PMSO
    - Scatter plot das variáveis numéricas com PMSO
    - Correlação de Pearson entre as variáveis
    - Teste de Shapiro-Wilk para normalidade
4. **Treinamento do Modelo**
    - Modelo com todas as variáveis
    - Modelo sem as variáveis com multicolinearidade
    - Modelo sem as variáveis não significativas e sem multicolinearidade
5. **Melhor Modelo**
    - Análise de resíduos
    - Análise preditiva do modelo
