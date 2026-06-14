# 📊 Análise Exploratória de Dados: Customer Churn em Telecomunicações

Este projeto aplica técnicas de **Ciência de Dados** e **Análise Exploratória (EDA)** utilizando Python para investigar o fenômeno de evasão de clientes (*Churn*) em uma grande empresa de telecomunicações. O objetivo principal é identificar padrões de comportamento dos clientes que cancelam o serviço e gerar *insights* acionáveis para estratégias de retenção.

## 🚀 Tecnologias e Ferramentas Utilizadas
* **Linguagem:** Python 3.13
* **Ambiente:** VS Code & Jupyter Notebooks
* **Manipulação de Dados:** Pandas, NumPy
* **Visualização de Dados:** Matplotlib, Seaborn

## 🔍 Principais Insights do Negócio
A partir das análises estatísticas e gráficas desenvolvidas no projeto, foram descobertos três padrões críticos:
1. **Impacto do Tipo de Contrato:** Clientes com contratos mensais (*Month-to-month*) concentram a esmagadora maioria dos cancelamentos. Contratos de longo prazo (1 ou 2 anos) apresentam retenção quase perfeita.
2. **Janela Crítica de Cancelamento:** O pico de *churn* ocorre de forma agressiva nos primeiros **5 meses** de relacionamento com o cliente. Clientes que ultrapassam essa barreira tendem a atingir altos níveis de fidelidade (acima de 60 meses).
3. **Padrão Financeiro:** A maioria dos clientes que evadem gera um faturamento acumulado baixo devido ao curtíssimo tempo de permanência, embora tenham sido detectados *outliers* de alto valor que também cancelaram o serviço.

## 🛠️ Tratamento e Higienização de Dados
Durante o desenvolvimento, foi identificada uma inconsistência crítica na coluna `TotalCharges`, que estava mapeada como texto (`object`) devido a espaços em branco ocultos.
* Os espaços em branco foram convertidos em valores nulos (`NaN`).
* A coluna foi tipada corretamente para numérica (`float64`).
* Linhas nulas correspondentes a novos clientes (com tempo de casa igual a zero) foram tratadas e removidas para garantir a integridade dos cálculos.

## 📁 Estrutura do Repositório
* `analise_exploratoria.ipynb`: Notebook Jupyter contendo todo o código de importação, limpeza e geração dos gráficos estatísticos (Boxplot, KDE de Densidade e Countplots).
* `WA_Fn-UseC_-Telco-Customer-Churn.csv`: Base de dados original utilizada no estudo.

---
Projetado e desenvolvido por **Fabiana Alves Ferreira** 👩‍💻  
*Estudante de Ciência de Dados na UNIVESP*
