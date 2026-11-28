# Aula 13 — AWS Lambda

**Base:** material autoral da disciplina, aula 13; nota de estudo, não registro de vídeo assistido.

## Resumo

Lambda executa código em resposta a eventos. Exemplo Java 21 `RequestHandler<S3Event, String>` reage a objeto novo no S3, lê configuração do SSM e envia notificação. IAM restringe acesso; CloudWatch registra execução.

## Para praticar e revisar

Desenhe S3 → Lambda → parâmetros → notificação. Considere idempotência, repetição, timeout e segredos; não crie recursos sem aprovar custo.
