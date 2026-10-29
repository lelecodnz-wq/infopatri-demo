# InfoPatri — editor para GitHub Pages

Esta pasta é um site estático pronto para publicar. Não precisa de Node, instalação ou servidor próprio para os visitantes.

## Publicar

1. Crie ou escolha um repositório GitHub para este site.
2. Envie o conteúdo desta pasta para a raiz do repositório, incluindo index.html, assets e .nojekyll. Não envie a pasta de desenvolvimento nem infopatri-release.
3. No repositório, abra Settings → Pages.
4. Em Build and deployment → Source, escolha Deploy from a branch.
5. Escolha a branch que recebeu os arquivos (normalmente main), a pasta /(root) e clique Save.
6. Aguarde a publicação e abra o endereço exibido pelo GitHub Pages.

Os endereços relativos permitem usar tanto um domínio próprio quanto usuario.github.io/nome-do-repositorio/.

## Recursos disponíveis

- Espectro Partidário com canvas, importação CSV/TSV/XLSX, edição, biblioteca de partidos, comparação manual, zoom e arraste com Espaço.
- Gráficos e votação manual.
- Abrir/salvar projetos .ifp, salvamento local no navegador e exportações PNG/JPG/SVG/PDF e tabelas compatíveis com cada editor.

As consultas às APIs oficiais usam acesso direto pelo navegador. Quando a fonte bloqueia esse acesso, é necessário configurar VITE_API_PROXY_URL durante a geração para usar o intermediário hospedado (ver docs/apis-online.md nas fontes). O botão Compartilhar cria uma cópia interativa com dados compactados no próprio link, sem armazenamento em servidor. A cópia não acompanha alterações no original; quem tiver o link poderá acessar seus dados. Links de até 16.000 caracteres e cópias de até 1 MB são aceitos; aplicativos de mensagens podem impor limites menores. Os arquivos importados permanecem no navegador; não são enviados a um servidor do InfoPatri. Guarde cópias .ifp para transferir projetos ou protegê-los contra a limpeza dos dados do navegador. Não inclua planilhas pessoais ou projetos no repositório destinado à publicação.

## Manutenção

Esta é a cópia compilada. Para gerar outra, execute na pasta de desenvolvimento: node tools/packagePages.cjs --output infopatri-pages-nova. As fontes e a versão com servidor permanecem separadas.

Documentação de publicação: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
