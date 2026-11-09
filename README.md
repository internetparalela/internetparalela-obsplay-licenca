# OBSPlay — senhas

## Baixar o OBSPlay (paróquias)

**[Clique aqui para baixar o OBSPlay](https://github.com/internetparalela/internetparalela-obsplay-licenca/raw/main/download/OBSPlay-paroquia.zip)**

1. Instale o OBS Studio (https://obsproject.com) e deixe o OBS fechado.
2. Extraia o arquivo baixado (botão direito > Extrair tudo).
3. Dê dois cliques em `INSTALAR.bat` e clique em "Sim".
4. Abra o OBS e envie ao responsável o código do computador que aparece na janela do OBSPlay.
5. Cole a chave recebida na janela do OBSPlay.

---

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
