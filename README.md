# Análise Climática das Capitais Brasileiras  

## Sobre o Projeto  
Este projeto tem como objetivo analisar as condições climáticas de diversas capitais brasileiras ao longo dos anos e meses, utilizando dados fornecidos pelo Instituto Nacional de Meteorologia (INMET). O processo envolveu etapas de extração, transformação, visualização e análise, resultando em insights valiosos sobre padrões sazonais, extremos climáticos e tendências de longo prazo.

---

## Etapas do Projeto  

### 1. **Coleta de Dados**  
Os dados foram extraídos diretamente da plataforma do INMET, contendo informações meteorológicas como:  
- **Temperatura** (mínima, máxima e média)  
- **Precipitação** (volume de chuva)  
- **Umidade relativa do ar**  
- **Velocidade do vento**    

### 2. **Transformação dos Dados**  
O pré-processamento foi realizado em **Python** utilizando a biblioteca **Pandas**, seguindo as etapas:  
- **Limpeza de Dados**: Remoção de valores duplicados e preenchimento de valores ausentes.  
- **Conversão de Formatos**: Padronização de datas e unidades de medida.  
  

### 3. **Carregamento e Visualização**  
Os dados transformados foram carregados no **Power BI** para a criação de um dashboard interativo.  

#### Painéis Criados:  
- **Gráfico de linhas**: Gráficos que mostram a evolução dos indicadores climáticos por anos e meses, a partir da temperatura media, maxima e minima.  
- **Gráfico de treemap interativo**: Representação por cada cidade do dataset, modificado em razão de datas e indicadores como (dias de seca, dias de chuva, temperatura máxima,...).  
- **Gráfico de colunas empilhadas e linhas**: Relatório que mostra como se comparta a humidade relativa do ar em decorrência das chuvas  


### 4. **Insights Extraídos**  
- É possível verificar que a humidade relativa do ar tem valores mais baixos quando a menos chuvas.  
- Tempos mais quentes, provocam mais ocorrências de chuvas.
- A temperatura média das capitais ao longo de 2020 a 2022 devido a pandemia se estabilizaram abaixo que o ano de 2023.
- Maior predominância de chuvas na região do norte, verificado a partir de 1 mm de precipitação.
- Maior predominância de secas na região do Centro-Oeste/Nordeste, verificado a partir de precipitações abaixo de 1 mm.

---

## Ferramentas Utilizadas  
- **Python**: Pré-processamento e transformação dos dados (Pandas, NumPy).  
- **Power BI**: Criação do dashboard interativo e relatórios visuais.  
- **GitHub**: Versionamento e compartilhamento do projeto.  

---

## Estrutura do Repositório  

```plaintext
/
├── .venv/                     # Pasta com o ambiente python
├── DadosClimaticos/           # Dados brutos do INMET.
├── main.ipynb                 # Scripts em Python no Jupyter Notebook para o processo de ETL
├── DadosClimaticosTransformados.csv  # Dados transformados
├── README.md                  # Detalhes do projeto.
└── ClimateChanges.pbix        # Arquivo do Power BI (projeto do dashboard).

```

## 🔧 **Instalação**
1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/preco-monitoramento.git
   cd preco-monitoramento
   ```

2. Crie e ative um ambiente virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows, use venv\Scripts\activate
   ```

3. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
