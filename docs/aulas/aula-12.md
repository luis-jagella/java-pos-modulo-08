# Aula 12 — Armazenando dados com DynamoDB

**Base:** material autoral da disciplina, aula 12; nota de estudo, não registro de vídeo assistido.

## Resumo

DynamoDB é NoSQL gerenciado e exige modelagem pelos padrões de acesso. Exemplo: `Pessoa` com matrícula como chave de partição e PDI/metas aninhados; Enhanced Client usa `@DynamoDbBean` e `@DynamoDbPartitionKey`. `Query` usa chave/índice, `Scan` percorre tabela.

## Para praticar e revisar

Liste consultas antes de escolher chaves. Compare capacidade on-demand/provisionada e estime custo; evite scan em fluxo crítico.
