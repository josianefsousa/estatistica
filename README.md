# 📊 Introdução à Estatística Descritiva com Python

Este projeto documenta o início dos meus estudos práticos de **Estatística Descritiva** aplicados à **Análise de Dados**, integrando a manipulação de dados em Python, análise exploratória, visualizações gráficas e interpretação analítica de métricas.

O objetivo do script é analisar uma base de dados de alunos (`alunos.csv`), explorando medidas de **tendência central**, **posição** e **dispersão** para compreender o comportamento, o desempenho e a variabilidade das notas da turma.

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

* **Python 3** — Linguagem principal para análise de dados.
* **Pandas & NumPy** — Estruturação de dados (`DataFrame`), cálculos numéricos e estatísticos.
* **Seaborn & Matplotlib** — Visualização de dados (histogramas, gráficos de frequência e linhas de referência).
* **Google Colab & Pathlib** — Montagem do Google Drive, gestão automática de diretórios e envio de ficheiros.

---

## 📐 Conceitos e Métricas Exploradas

### 1️⃣ Estrutura e Dimensão dos Dados
* Verificação inicial da quantidade de registros e variáveis na base (`dados.shape`).

---

### 2️⃣ Medidas de Tendência Central

* **Média ($\bar{x}$):** Soma de todos os valores dividida pelo total de alunos ($n$).
  * *Exploração:* Cálculo passo a passo com amostragem de 5 alunos e aplicação direta com `.mean()`.
* **Mediana:** Valor central que divide os dados ordenados ao meio (50% acima e 50% abaixo).
  * *Exploração:* Demonstração manual para conjuntos ímpares e pares, comparada com a função `.median()`.
* **Moda:** Valor ou categoria com maior frequência de ocorrência.
  * *Exploração:* Identificação do turno mais frequente, nota mais comum e número de faltas via `.mode()` e `countplot`.

---

### 3️⃣ Análise de Assimetria (*Skewness*)

Análise do formato da distribuição das notas em relação ao centro:
* **Coeficiente de Assimetria:** **$-0,04$**
* **Conclusão Analítica:** Como o valor é extremamente próximo de zero (entre $-0,5$ e $0,5$), a distribuição das notas é **praticamente simétrica**, indicando um equilíbrio entre os dados em torno da média, sem caudas longas para os extremos.

---

### 4️⃣ Medidas de Dispersão e Variabilidade

* **Amplitude ($A = x_{máx} - x_{mín}$):** Diferença entre a maior e a menor nota ($5,9$ pontos). Indica uma amplitude considerável de desempenho entre os alunos.
* **Variância ($s^2$):** Medida da distância ao quadrado de cada valor em relação à média.
  * *Exploração:* Tabela manual de desvios e quadrados dos desvios, diferenciando variância populacional ($\div N$) e amostral ($\div (n-1)$).
* **Desvio Padrão ($s = \sqrt{s^2}$):** Raiz quadrada da variância, retornando à unidade de medida original (pontos).
  * *Conclusão Analítica:* O desvio padrão aproximado de $1,78$ ponto mostra que as notas se afastam moderadamente da média, concentrando a maior parte da turma perto do centro da distribuição.

---

## 🎨 Visualizações Gráficas Desenvolvidas

1. **Histograma de Distribuição de Notas:**
   * Exibição das frequências de notas com destaque visual para a **Média** (linha vermelha) e **Mediana** (linha verde pontilhada), evidenciando a simetria da turma.
2. **Gráfico de Contagem de Faltas (*Count Plot*):**
   * Representação em colunas da moda e frequência do número de faltas entre os alunos.

---

## 📌 Próximos Passos (Em Desenvolvimento)

* 🔍 **Análise de Outliers:** Identificação de valores discrepantes e impacto na média vs. mediana.
* 📐 **Quartis, Percentis e Amplitude Interquartil (IQR):** Divisão dos dados em partes proporcionais para análise de caixa (*Boxplot*).
* ⚔️ **Estudo de Caso Prático:** Análise comparativa entre o turno da **Manhã** e o turno da **Noite** para suporte à tomada de decisões da coordenação pedagógica.

---
*Desenvolvido durante o Bootcamp de Análise de Dados da Generation Brasil por **Josiane Sousa**.*
