# Aula 08 — Criando o cluster e a arquitetura

**Base:** material autoral da disciplina, aula 08; nota de estudo, não registro de vídeo assistido.

## Resumo

O laboratório usa kind com um control plane e três workers. `kubectl` opera no contexto selecionado. Deployments e Services conectam MongoDB, API e front-end; a API usa o DNS do Service MongoDB, não `localhost` de outro pod.

## Para praticar e revisar

Confira contexto e use `kubectl get nodes,pods,services`, `describe` e `logs`. Desenhe a rota `mongodb://mongo:27017/unipdi`.
