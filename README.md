# Sorteio — Roleta e Caça-níquel (white label)

Sorteador white label em uma única página estática e sem dependências
(`index.html`). Basta abrir o arquivo no navegador — funciona offline (só as
fontes vêm do Google Fonts) — ou publicar em qualquer hospedagem estática
(GitHub Pages, Vercel, Netlify…).

## Tipos de sorteio

- **Roleta** — vários ponteiros (um por prêmio) ou um prêmio por giro. Ideal
  para até ~80 nomes.
- **Caça-níquel** — uma coluna por prêmio, com os nomes rolando em letra
  grande e parando na linha premiada. Pensado para 200+ participantes: em
  repouso as colunas rolam devagar, mostrando a quantidade de participantes.

Nos dois: "todos de uma vez" ou "um por vez", do último para o primeiro
prêmio, remoção de ganhadores, re-sorteio de ausentes, CSV e cópia do resultado.

## Formatos de vídeo

- **Livre** — ocupa a tela (computador, TV, telão).
- **Stories 9:16** (1080×1920) — conteúdo dentro das margens seguras do
  Instagram/TikTok (260 px no topo, 300 px embaixo, 70 px nas laterais).
- **Vídeo 16:9** (1920×1080) — margens de 5% (title-safe).

Nos formatos de vídeo, logo, título, sorteio, prêmios, ganhadores e rodapé
(nº de participantes, data e texto livre) ficam todos no quadro. A barra de
ferramentas fica fora dele e some sozinha. Guias de margem: tecla `G`.

### Gravar

Botão **Gravar** (ou tecla `R`) no Chrome/Edge do computador: escolha "esta
aba" e o vídeo grava **somente o quadro**, com música e efeitos. Pare com `R`
ou "Parar de compartilhar". Sai em MP4 (H.264) quando o navegador suporta,
senão em WebM. A resolução é a do quadro na tela — use tela cheia (`F`).

## Personalização

Prêmios (quantidade, descrição, cor, texto curto ou colados como
`4 X Cupom de R$ 100,00`), participantes (colados ou .txt/.csv), título,
subtítulo, logo, 6 temas e cores livres, trilha embutida ou música própria.
Tudo é salvo no navegador; exporte/importe a configuração em JSON para
reutilizar por cliente. O sorteio usa `crypto.getRandomValues`.

Atalhos: `Espaço` sorteia · `F` tela cheia · `M` música · `G` guias · `R` gravar · `Esc` fecha.

## Publicar no GitHub Pages

Settings → Pages → *Deploy from a branch* → `main` / `root`.
