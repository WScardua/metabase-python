# Metabase Analytics com Python
Analytics


## Motivação
Falta de painéis de indicadores das diversas áreas de negócio interagindo entre sí para uma tomada rápida de decisões estratégicas

## Desafio
* Banco de dados origem sem qualquer tipo de mecanismo de otimização devido as caracterísca do ERP;
* 150.000+ linhas de dados bruto;
* Tipos de dados básicos (char e number) para todas as colunas de todas as tabelas do ERP;
* Desejável que se tenha o menor 'gap' possível entre os pipelines.
 
## Abordagem
Desenvolver ETL's que busque dados no ERP em produção, trate/transforme o dado bruto em informação útil e a transporte para um banco de dados exclusivo e otimizado para a criação de dashboards de negócio

1. Modelagem e construção de uma estrutura de banco de dados otimizado para DW;
2. Carga de dados do ERP de Produção;
3. Tratamento e Transformação dos dados;
4. Carga das informações para o banco DW;
5. Criação de dashboards de negócio.

## Solução
1. Modelagem de estruturas de tabela otimizadas em um novo schema de banco de dados Oracle de forma a suportar a carga e a performance exigida por uma solução de analytics
	- SQL
	- Oracle

2. Desenvolvimentos de ETL's em Python que conectam ao schema do banco de dados Oracle do ERP de produção e fazem todo o tratamento e conversão dos diversos tipos de dados para carga em um outro schema de banco de dados também em Oracle otimizado para trazer uma performance satisfatória
	- Python
	- Oracle
	- SQL

3. Desenvolvimento de dashboard sob a plataforma Metabase que aborda diversas métricas de negócio utilizando filtros dinâmicos para refinar as visualizações 
	- SQL
	- Metabase
	
## Resumo da Estruturação da Solução
<p align="center">
	<img src="estruutra-etl-metabase.jpg" height="50%" width="50%">
</p>

## Resultado
A área de negócio passa a ter uma visão global, precisa e dinâmica de diversos indicadores de negócio que interagem entre sí, tais como: Posição de Compras, Previsão de Recebimento, Previsão de Vendas, Indicadores de Estoque, etc.

Com decisões baseadas em informações  é possível tomar melhores decisões e um direcionamento mais competitivo.

<p align="center">
	<img src="Dashboard-VisaoGeral.PNG" height="50%" width="50%">
</p>

<p align="center">** Por questões de privacidade este dashboard está baseado em dados fictícios **</p>

