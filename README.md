# Miniguia de AWS e Pipelines de Dados com NotebookLM

## Sobre o projeto

Este projeto foi desenvolvido como parte de um desafio da Digital Innovation One — DIO, com o objetivo de explorar o uso da Inteligência Artificial como ferramenta de aprendizagem ativa.

Para a realização do projeto, foi utilizado o NotebookLM, ferramenta que permite organizar fontes, realizar perguntas e gerar respostas fundamentadas nos documentos fornecidos.

## Tema escolhido

O tema selecionado foi **AWS e Pipelines de Dados**.

A escolha está relacionada à importância da computação em nuvem e da engenharia de dados para a construção de soluções capazes de coletar, processar, armazenar e disponibilizar grandes volumes de informações.

## Objetivos de estudo

Os principais objetivos deste projeto foram:

- compreender o conceito de pipeline de dados;
- conhecer as principais etapas de um pipeline;
- identificar os serviços da AWS utilizados em cada etapa;
- entender as diferenças entre processamento em lote e em tempo real;
- conhecer boas práticas de arquitetura, segurança e monitoramento;
- produzir um miniguia para futuras revisões.

## Ferramenta utilizada

Foi utilizado o **NotebookLM** para:

- centralizar as fontes de estudo;
- consultar os documentos utilizando linguagem natural;
- gerar resumos estruturados;
- identificar conceitos importantes;
- criar perguntas de revisão;
- comparar diferentes variações de prompts.

## Curadoria de fontes

As seguintes fontes foram selecionadas para compor o caderno temático:

1. Documentação do AWS Glue;
2. Documentação do Amazon S3;
3. Documentação do Amazon Athena;
4. Documentação do AWS Step Functions;
5. Material sobre arquiteturas de dados na AWS.

## Engenharia de prompts

Durante o estudo, foram utilizados prompts com diferentes níveis de detalhamento.

### Prompt inicial

> Explique o que é um pipeline de dados na AWS.

### Resultado observado

A resposta apresentou uma definição geral, mas não detalhou suficientemente os serviços utilizados e o fluxo dos dados.

### Prompt aprimorado

> Explique como funciona um pipeline de dados em lote na AWS, desde a ingestão até a disponibilização dos dados para análise. Relacione cada etapa aos serviços Amazon S3, AWS Glue, Amazon Athena e AWS Step Functions.

### Melhoria observada

A resposta passou a apresentar uma sequência mais clara das etapas e relacionou os serviços da AWS com suas respectivas funções.

### Prompt para visão prática

> Crie um exemplo de arquitetura para processar diariamente arquivos CSV recebidos em um bucket do Amazon S3. O pipeline deve validar, transformar, catalogar e disponibilizar os dados para consultas no Amazon Athena.

### Prompt para revisão

> Crie dez perguntas sobre pipelines de dados na AWS, separadas entre nível básico, intermediário e avançado. Apresente as respostas somente ao final.

## Cicatrizes e dificuldades encontradas

Durante os testes, algumas dificuldades foram identificadas:

- prompts muito genéricos geraram respostas superficiais;
- algumas respostas misturaram serviços com funções semelhantes;
- foi necessário solicitar exemplos práticos para compreender melhor as arquiteturas;
- perguntas longas demais produziram respostas pouco organizadas;
- a indicação explícita dos serviços desejados melhorou a qualidade das respostas;
- a validação das referências foi importante para evitar interpretações incorretas.

A principal aprendizagem foi que prompts com contexto, objetivo, serviços envolvidos e formato esperado produzem respostas mais úteis.

## Miniguia de estudo

### O que é um pipeline de dados?

Um pipeline de dados é um conjunto de processos responsáveis por transportar dados entre diferentes sistemas.

Normalmente, um pipeline realiza etapas como:

1. ingestão;
2. armazenamento;
3. validação;
4. transformação;
5. catalogação;
6. disponibilização;
7. monitoramento.

### Exemplo de pipeline na AWS

Um pipeline em lote pode seguir o seguinte fluxo:

1. arquivos são enviados para o Amazon S3;
2. uma função AWS Lambda identifica a chegada dos arquivos;
3. o AWS Step Functions inicia a orquestração;
4. o AWS Glue realiza a transformação dos dados;
5. o AWS Glue Data Catalog registra as tabelas;
6. o Amazon Athena consulta os dados processados;
7. o Amazon QuickSight pode apresentar os dados em painéis.

### Processamento em lote

O processamento em lote trabalha com conjuntos de dados acumulados durante determinado período.

Exemplos:

- processamento diário de vendas;
- consolidação mensal de resultados;
- atualização noturna de indicadores;
- processamento de arquivos recebidos durante o dia.

### Processamento em tempo real

O processamento em tempo real trabalha com dados conforme eles são produzidos.

Exemplos:

- monitoramento de transações;
- detecção de fraudes;
- análise de sensores;
- acompanhamento de eventos de sistemas.

Na AWS, serviços como Amazon Kinesis e Amazon MSK podem ser utilizados em arquiteturas de streaming.

## Glossário

### Amazon S3

Serviço de armazenamento de objetos utilizado para armazenar arquivos, dados brutos e dados processados.

### AWS Glue

Serviço de integração de dados utilizado para descoberta, preparação, transformação e catalogação.

### Amazon Athena

Serviço que permite consultar dados armazenados no Amazon S3 utilizando SQL.

### AWS Step Functions

Serviço utilizado para criar e coordenar fluxos de trabalho.

### AWS Lambda

Serviço de computação sem servidor utilizado para executar códigos a partir de eventos.

### ETL

Processo de extrair, transformar e carregar dados.

### ELT

Processo de extrair, carregar e posteriormente transformar os dados.

### Data Lake

Repositório centralizado capaz de armazenar dados estruturados e não estruturados.

### Data Warehouse

Ambiente estruturado e otimizado para consultas analíticas e geração de relatórios.

### Orquestração

Coordenação da ordem, das dependências e da execução das diferentes etapas de um pipeline.

### Batch

Modelo de processamento realizado em lotes.

### Streaming

Modelo de processamento contínuo de eventos e dados.

## Prompts reutilizáveis

### Resumo conceitual

> Produza um resumo estruturado sobre [assunto], utilizando somente as fontes adicionadas ao NotebookLM. Separe a resposta em definição, funcionamento, aplicações, vantagens, limitações e exemplo prático.

### Comparação

> Compare [serviço A] e [serviço B]. Apresente as diferenças de finalidade, funcionamento, custos, escalabilidade e casos de uso.

### Arquitetura

> Crie uma arquitetura de pipeline de dados na AWS para [cenário]. Explique a função de cada serviço, o fluxo dos dados, os pontos de segurança e as formas de monitoramento.

### Revisão

> Crie quinze perguntas sobre [assunto], divididas entre os níveis básico, intermediário e avançado. Apresente o gabarito somente depois de todas as perguntas.

### Identificação de lacunas

> Com base nas fontes fornecidas, identifique os conceitos sobre [assunto] que ainda não foram suficientemente explicados. Em seguida, sugira perguntas para aprofundar o estudo.

### Validação de conhecimento

> Analise a explicação abaixo sobre [assunto], identifique erros ou imprecisões e apresente uma versão corrigida com referências às fontes.

## Principais aprendizados

O desenvolvimento deste projeto demonstrou que a inteligência artificial pode apoiar o aprendizado, mas seus resultados dependem da qualidade das fontes e dos prompts utilizados.

Também foi possível compreender que um pipeline de dados na AWS não depende de apenas um serviço. Ele é formado pela integração entre armazenamento, processamento, catalogação, consulta, orquestração, segurança e monitoramento.

## Conclusão

O NotebookLM ajudou a organizar o conteúdo e transformar documentações técnicas em um material de revisão mais acessível.

A atividade também reforçou a importância da curadoria de fontes, da validação das respostas e da melhoria contínua dos prompts.

## Autor

**Moacyr Souza Barros**

Projeto desenvolvido para o desafio de criação de um Caderno Temático com NotebookLM da Digital Innovation One — DIO.
