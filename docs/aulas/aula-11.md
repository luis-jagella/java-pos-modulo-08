# Aula 11 — Integração com AWS S3

**Base:** material autoral da disciplina, aula 11; nota de estudo, não registro de vídeo assistido.

## Resumo

S3 armazena objetos em buckets. A API do UniPDI envia currículo para chave como `curriculo/{matricula}.pdf`; `S3Client` faz upload e `S3Presigner` cria URL temporária sem tornar bucket público.

## Para praticar e revisar

Desenhe upload → objeto privado → URL pré-assinada → expiração. Valide tipo/tamanho/autorização do arquivo. Nunca versionar chaves AWS.
