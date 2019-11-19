# Python with Metabase Analytics Project
Analytics


## Motivação
Após o amadurecimento da solução de ERP decidi levar mais inteligencia a tomada de decisões estratégicas da companhia, derivada de dados tratados e relevantes numa visualização de fácil entendimento, performática que seja escalável e sem um custo elevado.
 
## Desafio

* Banco de dados origem sem qualquer tipo de mecanismo de otimização devido as caracteriscas do ERP;
* 150.000+ linhas de dados bruto;
* Tipos de dados básicos (char e number) para todas as colunas de todas as tabelas do ERP;
* Desejável que se tenha o menor 'gap' possível entre os pipelines.
 
## Abordagem
Desenvolver ETL's buscassem informações no ERP, tratassem a informação e a transportassem para um banco de dados exclusivo e otimizado para a criação de dashboards de negócio

1. Modelagem e construção de uma estrutura de banco de dados otimizado para DW;
2. Carga de dados do ERP de Produção;
3. Tratamento e Transformação dos dados;
4. Carga dos dados tratados para o banco DW
5. Criação de dashboards de negócio.

## Solução

1. Modelagem de estuturas de tabela otimizadas em um novo schema de banco de dados Oracle de forma a suportar a carga e a performance exigida por uma solução de analytics
	- SQL
	- Oracle

2. Desenvolvimentos de ETL's em Python que conectam ao schema do banco de dados Oracle do ERP de produção e fazem todo o tratamento e conversão dos diversos tipos de dados para carga em um outro schema de banco de dados também em Oracle otimizado para trazer uma performance satisfatoria
	- Python
	- Oracle
	- SQL

3. Desenvolvimento de dashboard sob a plataforma Metabase que aborda diversas métricas de negócio utilizando filtros dinamicos para refinar as visualizações 
	- SQL
	- Metabase
	
## Resumo da Estruturação da Solução
<p align="center">
	<img src="estruutra-etl-metabase.jpg" height="50%" width="50%">
</p>

## Resultado
A área de negócio passa a ter uma visão global, precisa e dinâmica de diversos indicadores de negócio, tais como: Posição de Compras, Previsão de Recebimento, Previsão de Vendas, Indicadores de Estoque, etc. 
Com decisões baseadas em dados é possível tomar melhores decisões e um direcionamento mais competitivo.

<p align="center">
	<img src="Dashboard-VisaoGeral.PNG" height="50%" width="50%">
</p>

###### *Por questões de privacidade as informações estão baseadas em dados ficticios {align=center}

