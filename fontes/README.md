# Curadoria de fontes

Esta pasta apresenta as fontes utilizadas para a construção do caderno temático sobre **AWS e Pipelines de Dados** no NotebookLM.

As fontes foram selecionadas priorizando documentações oficiais, materiais abertos e conteúdos relacionados aos principais serviços utilizados na construção de pipelines de dados na AWS.

## Fontes selecionadas

### 1. Amazon S3

**Documentação:**
https://docs.aws.amazon.com/pt_br/AmazonS3/latest/userguide/Welcome.html

O Amazon Simple Storage Service — Amazon S3 — é um serviço de armazenamento de objetos.

Dentro de um pipeline de dados, pode ser utilizado para armazenar:

* dados brutos;
* arquivos CSV, JSON e Parquet;
* dados processados;
* resultados de consultas;
* logs;
* artefatos de modelos.

### 2. AWS Glue

**Documentação:**
https://docs.aws.amazon.com/pt_br/glue/latest/dg/what-is-glue.html

O AWS Glue é um serviço de integração de dados utilizado para descoberta, preparação, transformação e movimentação de dados.

Pode ser utilizado para:

* executar processos de ETL;
* criar crawlers;
* identificar esquemas;
* catalogar tabelas;
* processar dados com Apache Spark;
* integrar diferentes fontes de dados.

### 3. AWS Glue Data Catalog

**Documentação:**
https://docs.aws.amazon.com/pt_br/glue/latest/dg/catalog-and-crawler.html

O AWS Glue Data Catalog funciona como um catálogo central de metadados.

Ele permite registrar informações como:

* nomes das tabelas;
* nomes e tipos das colunas;
* localização dos dados;
* formato dos arquivos;
* partições;
* bancos de dados.

### 4. Amazon Athena

**Documentação:**
https://docs.aws.amazon.com/pt_br/athena/latest/ug/what-is.html

O Amazon Athena permite consultar dados armazenados no Amazon S3 utilizando SQL.

Ele pode ser usado para:

* analisar arquivos no S3;
* consultar tabelas catalogadas;
* validar resultados de processamento;
* gerar bases para relatórios;
* investigar problemas de qualidade.

### 5. AWS Step Functions

**Documentação:**
https://docs.aws.amazon.com/pt_br/step-functions/latest/dg/welcome.html

O AWS Step Functions é um serviço de orquestração de fluxos de trabalho.

Ele permite:

* definir a sequência das etapas;
* controlar dependências;
* executar tarefas em paralelo;
* configurar tentativas automáticas;
* tratar falhas;
* acompanhar o status das execuções.

## Critérios utilizados na curadoria

As fontes foram selecionadas considerando os seguintes critérios:

* documentação oficial;
* acesso gratuito;
* conteúdo relacionado ao tema;
* possibilidade de utilização no NotebookLM;
* presença de conceitos técnicos e exemplos;
* relevância para pipelines de dados.

## Processo de utilização no NotebookLM

As fontes foram adicionadas ao NotebookLM para apoiar:

* geração de resumos;
* explicação de conceitos;
* comparação entre serviços;
* criação de arquiteturas;
* elaboração de perguntas de revisão;
* identificação de boas práticas.

## Observação

As respostas geradas pelo NotebookLM devem ser verificadas com base nas referências apresentadas pela própria ferramenta.

A Inteligência Artificial foi utilizada como apoio ao aprendizado, e não como substituta da documentação oficial.
