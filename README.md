# Sorteio — Roleta de prêmios (white label)

Sorteador em roleta com **vários ponteiros de prêmios**, em uma única página
estática e sem dependências (`index.html`). Basta abrir o arquivo no navegador —
funciona offline (só as fontes vêm do Google Fonts) — ou publicar em qualquer
hospedagem estática (GitHub Pages, Vercel, Netlify…).

## Recursos

- **Prêmios** com quantidade, descrição, cor e rótulo do ponteiro (ou colados
  em texto: `4 X Cupom de R$ 100,00`).
- **Participantes** colados um por linha (ou importados de .txt/.csv), com
  embaralhar e remover repetidos.
- **Modos:** *vários ponteiros* (um ponteiro por prêmio, um único giro revela
  todos) ou *um por vez*; ordem do último para o primeiro; remover ganhadores.
- **Aparência:** título, subtítulo, logo (também no centro da roleta), 6 temas
  prontos e cores livres.
- **Som:** trilha embutida (Web Audio), efeitos de roleta/fanfarra/aplausos ou
  música própria (salva no IndexedDB).
- Ganhador ausente → re-sorteio do prêmio; exportação CSV e cópia do resultado.
- Tudo é salvo no `localStorage` do navegador; exporte/importe a configuração
  em JSON para reutilizar por cliente.
- Sorteio com `crypto.getRandomValues`: todos os nomes têm a mesma chance.

Atalhos: `Espaço` gira, `F` tela cheia, `M` música, `Esc` fecha.

## Publicar no GitHub Pages

Settings → Pages → *Deploy from a branch* → `main` / `root`. A roleta fica em
`https://<usuario>.github.io/<repositorio>/`.
