# Módulo 08 — Infraestrutura e Cloud Computing

Repositório de estudos da pós-graduação **Java Applied Engineering**. O material autoral confirma o título completo da disciplina: **Infraestrutura e Cloud Computing com Docker, Kubernetes e AWS**.

O portal organiza o conteúdo em um **Módulo 01** com 15 videoaulas, um podcast e uma avaliação. A numeração deste repositório segue os módulos da sequência de estudos já registrados nos repositórios `java-pos-modulo-01` a `java-pos-modulo-07`.

## Organização

| Branch | Conteúdo |
| --- | --- |
| `main` | Índice, resumos e acompanhamento da disciplina |
| `modulo-01-docker-kubernetes-aws` | Práticas e arquivos executáveis acompanhando as aulas |

Os checks abaixo indicam **notas registradas no Git**. Não representam aulas assistidas nem alteram o progresso no portal.

## Módulo 01 — Videoaulas

Esta trilha parte da aplicação UniPDI usada no material da disciplina: primeiro empacotamos os serviços, depois os orquestramos e, por fim, estudamos integrações e entrega na AWS. Os checks indicam anotações concluídas, não presença nas aulas.

| Etapa | Aulas | Resultado de estudo esperado |
| --- | --- | --- |
| Contêineres | 01–06 | Entender infraestrutura, criar e otimizar imagens, comparar Docker e Podman. |
| Orquestração | 07–09 | Subir um cluster local, publicar workloads e configurar escala e saúde. |
| AWS | 10–13 | Entender serviços e custos; integrar S3, DynamoDB e Lambda com cuidado com credenciais. |
| CI/CD | 14–15 | Automatizar validação e entrega com GitHub Actions e Jenkins. |

O material autoral confirmou os títulos completos que aparecem truncados no portal. As notas são sínteses desse material, ainda sujeitas a complementação pelos vídeos.

- [x] [Aula 01 — Introdução a Infra e Cloud Computing](docs/aulas/aula-01.md)
- [x] [Aula 02 — Fundamentos Docker](docs/aulas/aula-02.md)
- [x] [Aula 03 — Criando e Disponibilizando Imagens](docs/aulas/aula-03.md)
- [x] [Aula 04 — Otimização de imagens Docker](docs/aulas/aula-04.md)
- [x] [Aula 05 — Conhecendo o Podman](docs/aulas/aula-05.md)
- [x] [Aula 06 — Podman Desktop](docs/aulas/aula-06.md)
- [x] [Aula 07 — Fundamentos de Kubernetes](docs/aulas/aula-07.md)
- [x] [Aula 08 — Criando o Cluster e a Arquitetura](docs/aulas/aula-08.md)
- [x] [Aula 09 — Escalabilidade e saúde](docs/aulas/aula-09.md)
- [x] [Aula 10 — Fundamentos AWS](docs/aulas/aula-10.md)
- [x] [Aula 11 — Integração com AWS S3](docs/aulas/aula-11.md)
- [x] [Aula 12 — Armazenando Dados com DynamoDB](docs/aulas/aula-12.md)
- [x] [Aula 13 — AWS Lambda](docs/aulas/aula-13.md)
- [x] [Aula 14 — Integração e Entrega Contínua com GitHub Actions](docs/aulas/aula-14.md)
- [x] [Aula 15 — Pipelines Declarativas com Jenkins](docs/aulas/aula-15.md)
- [ ] [Podcast 01](docs/podcast-01.md)

## Materiais e andamento

- Os PDFs e as mídias ficarão em uma pasta local de materiais; conteúdo com acesso temporário não será publicado no Git.
- As 15 notas foram preenchidas com base no material autoral oficial. Elas não substituem a visualização dos vídeos; pontos de versão, preço e quota devem ser conferidos nas fontes atuais.
- A avaliação é uma etapa separada e só será entregue após confirmação do aluno.

## Como estudar

1. Registre o resumo de cada aula em `docs/aulas/`.
2. Acompanhe os exercícios na branch prática, mantendo segredos e credenciais fora do Git.
3. Para AWS, use contas e recursos de baixo custo, configure alertas de orçamento e remova recursos ao terminar.
4. Diferencie as notas do repositório do progresso no ambiente virtual.

Comece pela [revisão geral dos conceitos](docs/revisao-geral.md) para identificar os tópicos que merecem estudo mais profundo antes dos laboratórios.
