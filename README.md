# OBSPlay — senhas

O OBSPlay lê o arquivo `senhas.json` deste repositório toda vez que o OBS abre.
Aqui ficam só os códigos embaralhados (SHA-256) das senhas, nunca as senhas.

- `master`: libera tudo.
- `filial`: libera tudo menos a Saída HLS e a Saída SCTE-35.

Para trocar as senhas, abra `tools/gerar-senha.html` (repositório obsplay) no navegador,
gere o conteúdo novo e cole aqui no `senhas.json`. As senhas antigas deixam de valer na
próxima abertura do OBS com internet.

## Chaves das paróquias

Dentro de `"chaves"` fica uma linha por paróquia. Para renovar, mude a data `"vence"`.
Para cancelar, apague a linha. Use `tools/gerar-chave.html` (repositório obsplay) para gerar chaves novas.
