# Prompts testados no NotebookLM

Este documento apresenta os prompts utilizados durante o estudo sobre **AWS e Pipelines de Dados**.

Além das perguntas realizadas, foram registrados os resultados observados, as melhorias aplicadas e as dificuldades encontradas durante a interação com a Inteligência Artificial.

## Prompt 1 — Definição inicial

### Prompt utilizado

> Explique o que é um pipeline de dados na AWS.

### Resultado observado

A resposta apresentou uma definição geral de pipeline de dados e citou alguns serviços da AWS.

Entretanto, a explicação não detalhou:

* as etapas do processo;
* a função de cada serviço;
* o fluxo dos dados;
* exemplos de aplicação;
* formas de monitoramento.

### Dificuldade encontrada

O prompt era muito genérico e não determinava o nível de profundidade esperado.

### Aprendizado

Prompts muito amplos podem gerar respostas corretas, porém superficiais.

---

## Prompt 2 — Explicação estruturada

### Prompt utilizado

> Explique como funciona um pipeline de dados em lote na AWS, desde a ingestão até a disponibilização dos dados para análise. Relacione cada etapa aos serviços Amazon S3, AWS Glue, Amazon Athena e AWS Step Functions.

### Resultado observado

A resposta apresentou uma sequência mais organizada, incluindo:

1. recebimento dos arquivos;
2. armazenamento no Amazon S3;
3. transformação com AWS Glue;
4. catalogação dos dados;
5. consulta com Amazon Athena;
6. orquestração com AWS Step Functions.

### Melhoria identificada

Ao especificar os serviços e o formato da explicação, a resposta ficou mais direcionada.

---

## Prompt 3 — Exemplo prático

### Prompt utilizado

> Crie um exemplo de arquitetura para processar diariamente arquivos CSV recebidos em um bucket do Amazon S3. O pipeline deve validar, transformar, catalogar e disponibilizar os dados para consultas no Amazon Athena.

### Resultado observado

A resposta apresentou um exemplo próximo de um cenário real.

O fluxo sugerido incluiu:

1. recebimento dos arquivos no Amazon S3;
2. acionamento do pipeline;
3. validação dos dados;
4. execução de um job do AWS Glue;
5. conversão dos arquivos para Parquet;
6. atualização do Glue Data Catalog;
7. disponibilização para consultas no Athena.

### Aprendizado

Adicionar um cenário de negócio ajuda a gerar respostas mais práticas.

---

## Prompt 4 — Comparação entre serviços

### Prompt utilizado

> Compare AWS Glue, AWS Lambda e AWS Step Functions dentro de um pipeline de dados. Apresente a finalidade de cada serviço, exemplos de uso, vantagens, limitações e quando utilizar cada um.

### Resultado observado

A resposta diferenciou os serviços da seguinte forma:

* AWS Glue para transformação e integração de dados;
* AWS Lambda para execuções curtas orientadas a eventos;
* AWS Step Functions para orquestração e controle do fluxo.

### Dificuldade encontrada

Em algumas respostas, o NotebookLM misturou execução de tarefas com orquestração.

### Correção aplicada

Foi necessário solicitar uma comparação baseada na responsabilidade principal de cada serviço.

---

## Prompt 5 — Batch e streaming

### Prompt utilizado

> Explique as diferenças entre pipelines de dados em lote e pipelines em tempo real na AWS. Apresente características, vantagens, limitações, exemplos e serviços indicados para cada arquitetura.

### Resultado observado

A resposta apresentou uma comparação entre:

* processamento periódico;
* processamento contínuo;
* latência;
* custo;
* complexidade;
* exemplos de aplicação.

Também foram citados Amazon Kinesis e Amazon MSK para cenários de streaming.

---

## Prompt 6 — Boas práticas

### Prompt utilizado

> Liste boas práticas para construir um pipeline de dados seguro, escalável e monitorável na AWS. Organize a resposta nas categorias armazenamento, processamento, segurança, qualidade, custo e monitoramento.

### Resultado observado

A resposta ficou mais organizada por causa das categorias definidas no prompt.

Foram apresentadas práticas relacionadas a:

* particionamento;
* formato Parquet;
* criptografia;
* controle de acesso;
* logs;
* tratamento de erros;
* alertas;
* validação de dados;
* controle de custos.

---

## Prompt 7 — Perguntas de revisão

### Prompt utilizado

> Crie quinze perguntas sobre pipelines de dados na AWS, divididas entre os níveis básico, intermediário e avançado. Apresente as respostas somente depois de todas as perguntas.

### Resultado observado

O prompt gerou um conjunto de perguntas que pode ser reutilizado para revisão do conteúdo.

A separação por níveis ajudou a organizar a evolução do aprendizado.

---

## Prompt 8 — Glossário

### Prompt utilizado

> Crie um glossário sobre AWS e pipelines de dados. Para cada termo, apresente uma definição simples e um exemplo de aplicação.

### Resultado observado

A resposta gerou definições para conceitos como:

* pipeline de dados;
* ETL;
* ELT;
* Data Lake;
* Data Warehouse;
* batch;
* streaming;
* partição;
* catálogo;
* orquestração.

---

## Prompt 9 — Identificação de lacunas

### Prompt utilizado

> Com base nas fontes fornecidas, identifique quais conceitos sobre pipelines de dados na AWS ainda não foram suficientemente explicados. Em seguida, sugira perguntas para aprofundar o estudo.

### Resultado observado

A resposta ajudou a identificar temas que precisavam de aprofundamento, como:

* segurança;
* monitoramento;
* tratamento de falhas;
* custos;
* governança;
* qualidade dos dados.

---

## Prompt 10 — Resumo final

### Prompt utilizado

> Produza um miniguia sobre AWS e pipelines de dados utilizando somente as fontes fornecidas. Organize o conteúdo em introdução, etapas do pipeline, serviços da AWS, exemplo de arquitetura, boas práticas, glossário e conclusão.

### Resultado observado

Esse prompt foi utilizado como base para consolidar o conteúdo final do projeto.

## Cicatrizes e troubleshooting

Durante os testes, foram identificadas as seguintes dificuldades:

### Respostas superficiais

Prompts genéricos produziram respostas com pouco detalhamento.

**Solução:** incluir contexto, objetivo, serviços envolvidos e formato esperado.

### Confusão entre serviços

Algumas respostas apresentaram sobreposição entre AWS Glue, Lambda e Step Functions.

**Solução:** solicitar uma comparação baseada na responsabilidade principal de cada serviço.

### Falta de exemplos

Explicações conceituais nem sempre ajudavam a visualizar o funcionamento do pipeline.

**Solução:** adicionar cenários práticos ao prompt.

### Respostas pouco organizadas

Prompts com muitas perguntas em uma única frase geraram respostas desorganizadas.

**Solução:** definir seções e categorias de resposta.

### Necessidade de validação

Mesmo utilizando fontes confiáveis, as respostas precisaram ser verificadas.

**Solução:** analisar as referências indicadas pelo NotebookLM e comparar as informações com a documentação oficial.

## Modelo de prompt reutilizável

> Atue como um instrutor de engenharia de dados. Utilizando somente as fontes fornecidas, explique [ASSUNTO]. Organize a resposta em definição, funcionamento, serviços envolvidos, exemplo prático, vantagens, limitações e boas práticas. Ao final, crie cinco perguntas para revisão e indique as fontes utilizadas.
