# AWS e Pipelines de Dados com NotebookLM

## Sobre o projeto

Este projeto foi desenvolvido para o desafio da DIO sobre o uso da Inteligência Artificial como ferramenta de aprendizagem ativa.

O tema escolhido foi AWS e pipelines de dados. O NotebookLM foi utilizado para analisar fontes oficiais, responder perguntas, comparar serviços e organizar um resumo conceitual sobre o assunto.

## Objetivo

Criar um guia introdutório e prático sobre pipelines de dados na AWS, abordando armazenamento, transformação, catalogação, consulta e orquestração.

## Fontes utilizadas

1. Amazon S3  
https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html

2. AWS Glue  
https://docs.aws.amazon.com/pt_br/glue/latest/dg/what-is-glue.html

3. AWS Glue Data Catalog  
https://docs.aws.amazon.com/pt_br/glue/latest/dg/start-data-catalog.html

4. Amazon Athena  
https://docs.aws.amazon.com/pt_br/athena/latest/ug/what-is.html

5. AWS Step Functions  
https://docs.aws.amazon.com/pt_br/step-functions/latest/dg/welcome.html

## Prompts testados

### Prompt inicial

Como funciona um pipeline de dados na AWS?

### Problema encontrado

A resposta ficou genérica e citou muitos serviços sem explicar claramente a função de cada um.

### Prompt melhorado

Com base exclusivamente nas fontes adicionadas, explique como funciona um pipeline de dados utilizando Amazon S3, AWS Glue, Glue Data Catalog, Amazon Athena e AWS Step Functions.

Organize a resposta por etapas e informe a responsabilidade de cada serviço.

### Resultado

O segundo prompt produziu uma resposta mais organizada, objetiva e alinhada às fontes.

## Miniguia de estudo

Um pipeline de dados é um conjunto de processos responsáveis por coletar, armazenar, transformar e disponibilizar dados.

Uma possível arquitetura na AWS utiliza:

- Amazon S3 para armazenar os arquivos;
- AWS Glue para transformar os dados;
- Glue Data Catalog para armazenar metadados;
- Amazon Athena para realizar consultas SQL;
- AWS Step Functions para coordenar a execução das etapas;
- Amazon CloudWatch para monitorar logs e falhas.

Fluxo simplificado:

Fonte de dados → Amazon S3 → AWS Glue → Data Catalog → Athena

## Principais aprendizados

- O Amazon S3 armazena os dados, mas não realiza transformações;
- O AWS Glue pode executar processos de ETL;
- O Data Catalog armazena informações sobre tabelas, colunas e partições;
- O Athena permite consultar arquivos armazenados no S3 utilizando SQL;
- O Step Functions ajuda a controlar a sequência e o tratamento de falhas;
- Prompts específicos produzem respostas melhores que perguntas genéricas.

## Glossário

| Conceito | Definição |
|---|---|
| Pipeline de dados | Processo de movimentação e transformação de dados |
| ETL | Extração, transformação e carregamento |
| Data Lake | Repositório de dados estruturados e não estruturados |
| Metadados | Informações que descrevem os dados |
| Parquet | Formato colunar utilizado em análises |
| Particionamento | Organização dos dados em grupos ou diretórios |
| Orquestração | Coordenação das etapas de um processo |

## Prompts reutilizáveis

### Explicação de serviço

Explique o funcionamento do serviço AWS [NOME DO SERVIÇO], apresentando seu objetivo, principais recursos, exemplos de uso e limitações.

### Comparação

Compare [SERVIÇO A] e [SERVIÇO B], destacando suas responsabilidades e quando cada um deve ser utilizado.

### Revisão de arquitetura

Analise criticamente esta arquitetura de dados e identifique riscos, falhas, problemas de segurança e oportunidades de melhoria.

## Conclusão

O NotebookLM ajudou a transformar documentações técnicas da AWS em um material de estudo mais organizado. O principal aprendizado foi compreender que cada serviço possui uma responsabilidade específica dentro do pipeline e que a qualidade das respostas depende diretamente da clareza dos prompts utilizados.

## Autor

Moacyr Souza Barros
