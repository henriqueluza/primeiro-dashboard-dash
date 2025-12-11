# Airline Dashboard - IBM Data Science Course

Este projeto é uma atividade prática do curso **IBM Data Science** focada em visualização de dados e criação de dashboards interativos.

## Sobre o Projeto

O dashboard foi desenvolvido utilizando **Dash** e **Plotly** para visualizar dados de companhias aéreas dos Estados Unidos.

## Dataset

O projeto utiliza o dataset `airline_data.csv` fornecido pela IBM, que contém informações sobre voos de companhias aéreas americanas, incluindo:

- **Flights**: Número de voos
- **DistanceGroup**: Grupos de distância (intervalos de 250 milhas)
- Informações sobre aeroportos de desvio (Div1Airport, Div2Airport)
- Números de cauda das aeronaves (TailNum)

O dataset é carregado diretamente do IBM Cloud Object Storage e pode ser acessado através do link: `https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0101EN-SkillsNetwork/Data%20Files/airline_data.csv`

## Visualizações

### 1. Dashboard Básico (`dash_basics.py`)

O primeiro dashboard apresenta um gráfico de pizza (pie chart) mostrando a proporção de grupos de distância por número de voos, utilizando uma amostra aleatória de 500 pontos do dataset original.

### 2. Dashboard Interativo de Atrasos de Voo (`flight_delay.py`)

Dashboard interativo que permite analisar estatísticas de tempo de atraso de voos por ano. O usuário pode inserir um ano específico e visualizar cinco gráficos de linha diferentes mostrando:

- **Carrier Delay**: Tempo médio de atraso causado pela companhia aérea
- **Weather Delay**: Tempo médio de atraso causado por condições climáticas
- **NAS Delay**: Tempo médio de atraso causado pelo Sistema Nacional de Espaço Aéreo (National Airspace System)
- **Security Delay**: Tempo médio de atraso causado por questões de segurança
- **Late Aircraft Delay**: Tempo médio de atraso causado por aeronaves atrasadas

Cada gráfico exibe a evolução mensal dos atrasos, diferenciando as companhias aéreas por cores. O dashboard utiliza **callbacks** do Dash para criar uma experiência interativa e dinâmica, atualizando todos os gráficos automaticamente quando o ano é modificado.

## Como Executar

**Dashboard Básico:**
```bash
python3 dash_basics.py
```

**Dashboard de Atrasos:**
```bash
python3 flight_delay.py
```

Acesse o dashboard no navegador através do endereço fornecido no terminal (geralmente `http://127.0.0.1:8050/`).

## Tecnologias Utilizadas

- Python
- Pandas
- Plotly Express
- Dash
