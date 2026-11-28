# Revisão geral — Infraestrutura e Cloud Computing

Use estas perguntas para revisar a disciplina sem depender de decorar comandos. A resposta deve explicar **quando usar**, **o que a ferramenta resolve** e **qual limite permanece**.

## Contêineres

1. Qual a diferença entre imagem e contêiner? Uma imagem é o pacote de aplicação e dependências; o contêiner é uma instância em execução desse pacote.
2. Por que um volume é importante para o MongoDB? O ciclo de vida dos dados não deve depender da recriação do contêiner.
3. O que um build multiestágio melhora? Separa compilação do runtime, reduzindo a imagem final e a quantidade de ferramentas presentes nela.
4. Docker e Podman são idênticos? Ambos trabalham com imagens OCI e comandos semelhantes, mas arquitetura, permissões, rede e integração com o host podem diferir. Podman é daemonless e favorece execução rootless.

## Kubernetes

5. O que fazem Pod, Deployment e Service? O Pod hospeda contêineres; o Deployment mantém o estado desejado de réplicas e atualizações; o Service oferece um endereço estável para alcançá-las.
6. Por que `localhost` não conecta dois Pods distintos? Cada Pod tem seu próprio contexto de rede. A aplicação normalmente usa o nome DNS de um Service para falar com outro componente.
7. Qual a diferença entre readiness e liveness? Readiness controla se o Pod recebe tráfego; liveness verifica se o contêiner precisa ser reiniciado. Startup probe protege inicializações lentas.
8. O que o HPA precisa para escalar com base em CPU? Métricas disponíveis, um alvo de utilização e `requests` de CPU coerentes. Escalar Pods não aumenta automaticamente a capacidade do banco ou da API externa.
9. Quando usar Secret ou ConfigMap? Secret para dados sensíveis; ConfigMap para configuração comum. Um Secret não dispensa controle de acesso, criptografia adequada e cuidado com logs.

## AWS e entrega

10. Qual a responsabilidade do time ao usar cloud? Ainda é necessário configurar IAM, rede, observabilidade, segurança, orçamento e ciclo de vida dos recursos. Preço e quotas devem ser conferidos na documentação atual.
11. Por que S3 e Lambda combinam em processamento de arquivos? S3 guarda objetos e pode emitir eventos de criação; Lambda executa a transformação sem servidor dedicado. O fluxo precisa considerar repetição de eventos, idempotência e custo.
12. Por que modelar DynamoDB pelos padrões de acesso? Chaves e índices determinam consultas eficientes; `Scan` percorre dados e pode custar caro em escala.
13. O que CI/CD automatiza? Build, testes e entrega, com gatilhos e condições definidos. Automação não garante qualidade por si só e não elimina revisão ou testes exploratórios.
14. O que diferencia GitHub Actions e Jenkins? Ambos executam pipelines; Actions usa workflows e runners integrados ao GitHub, enquanto Jenkins exige servidor, agents, plugins e manutenção próprios.
15. Como uma pipeline deve acessar a AWS? Com permissões mínimas, preferencialmente identidade federada e credenciais temporárias. Nunca versionar access keys ou segredos no YAML/Jenkinsfile.

## Exercício de integração

Desenhe UniPDI (front-end, API e banco) em três etapas: execução local com Compose, cluster Kubernetes local e uma alternativa AWS. Para cada etapa, indique rede, persistência, segredos, verificação de saúde, custo e forma de entrega. Não é necessário criar recursos pagos para responder.

Estas respostas são um roteiro de estudo baseado nos tópicos da disciplina, não comprovam visualização das videoaulas nem substituem o material oficial.
