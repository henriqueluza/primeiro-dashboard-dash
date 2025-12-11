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

## Visualização

O dashboard apresenta um gráfico de pizza (pie chart) mostrando a proporção de grupos de distância por número de voos, utilizando uma amostra aleatória de 500 pontos do dataset original.

## Como Executar

```bash
python3 dash_basics.py
```

Acesse o dashboard no navegador através do endereço fornecido no terminal (geralmente `http://127.0.0.1:8050/`).

## Tecnologias Utilizadas

- Python
- Pandas
- Plotly Express
- Dash
