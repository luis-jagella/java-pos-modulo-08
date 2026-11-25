# Aula 09 — Escalabilidade e saúde

**Base:** material autoral da disciplina, aula 09; nota de estudo, não registro de vídeo assistido.

## Resumo

Réplicas melhoram capacidade e disponibilidade. Readiness tira pod do tráfego; liveness pode reiniciá-lo; startup protege inicialização lenta. HPA ajusta réplicas com métricas e `requests`; exemplo: 2–10 réplicas e alvo de 50% CPU.

## Para praticar e revisar

Inspecione `kubectl get hpa`. Ajustes de requests/limits extremos e TLS inseguro do metrics-server são apenas de laboratório, não recomendações de produção.
