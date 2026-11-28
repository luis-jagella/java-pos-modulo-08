# Práticas — Docker, Kubernetes e AWS

Esta branch concentrará os exercícios executáveis da disciplina. O roteiro abaixo é uma estrutura inicial baseada nos tópicos visíveis no portal; os laboratórios concretos serão definidos conforme o material das aulas for estudado.

1. Construir e executar uma aplicação em contêiner com Docker.
2. Reduzir e publicar uma imagem, comparando Docker e Podman.
3. Declarar workloads, serviços, escalabilidade e verificações de saúde em Kubernetes.
4. Exercitar integrações AWS com S3, DynamoDB e Lambda.
5. Automatizar build e entrega com pipeline declarativa no Jenkins.

## Segurança e custos

- Nunca versionar chaves, tokens, arquivos `.env` ou credenciais AWS.
- Preferir variáveis de ambiente locais, perfis temporários e permissões mínimas.
- Antes de criar recursos AWS, confirmar região, configurar alertas de orçamento e verificar os custos do serviço.
- Remover recursos de laboratório ao finalizar e conferir que não ficaram serviços cobrando.

## Estado

Nenhum recurso de nuvem foi criado. Os exemplos serão locais por padrão e não publicarão imagens nem farão deploy sem solicitação explícita.
