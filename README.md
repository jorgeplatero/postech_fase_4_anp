# DataViz com Preço de Combustíveis Ofertados nos Postos Brasileiros

## Descrição do Projeto

Este projeto consiste em um dashboard que reune indicadores referentes ao preço dos combutíveis praticado em postos brasileiros e publicados pela ANP (Agência Nacional do Petróleo, Gás Natural e Biocombustíveis).

## Arquitetura do projeto

### Banco de dados

A tabela abaixo foi criada para comportar os dados.

```sql
CREATE TABLE anp.preco_combustivel(
	regiao 				varchar(255)
	,estado				varchar(255)
	,municipio			varchar(255)
	,revenda			varchar(255)
	,cnpj				varchar(255)
	,nome_rua			varchar(255)	
	,numero_rua			varchar(255)
	,complemento		varchar(255)
	,bairro				varchar(255)
	,cep				varchar(255)
	,produto			varchar(255)
	,data_coleta		date
	,valor_venda		float
	,unidade_medida		varchar(255)
	,bandeira			varchar(255)

)
```

### ETL dos dados

Os dados foram inseridos por meio da ferramenta de ETL KNIME.<br/>

O fluxo do ETL foi construído na aplicação conforme ilustrado:

## Tecnologias Utilizadas

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original-wordmark.svg" width="50" height="50"/> 

## Fontes de Dados

Link para a base de dados: <a style="text-decoration:none;" href="https://www.gov.br/anp/pt-br/centrais-de-conteudo/dados-abertos/serie-historica-de-precos-de-combustiveis">link</a>.

Utilizou-se os últimos 5 anos da base de dados.

## Link para a Aplicação

Dashboard Power BI: <a style="text-decoration:none;" href="https://app.powerbi.com/view?r=eyJrIjoiNGJlOTY3ZmYtZjZlMS00ZTEzLWJiMmMtMWRjYjJiZTBlYTAzIiwidCI6IjFmZTA1YTY2LWNhMjYtNGJmZC1hZDlkLWQzMDRhZGViMjIwNSJ9" target="_blank">link</a>.
