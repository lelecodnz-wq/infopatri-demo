# Bibliotecas locais

- Jspreadsheet CE 5.0.4: grade do modo Gráficos, em `jspreadsheet-ce/dist/index.js` e CSS local. Licença MIT, pacote npm e hashes em `jspreadsheet-ce/README.md` e `package-source.json`. Integração por `chartsGrid.js`; fórmulas e HTML de células desativados.
- jSuites 5.13.5: dependência compatível do Jspreadsheet CE, JS/CSS em `jsuites/dist/`; licença MIT, origem e hashes em `jsuites/README.md`. Sem recursos externos em tempo de execução.

- D3 7.9.0: distribuição UMD em `d3/d3.v7.9.0.min.js`, licença ISC em `d3/LICENSE`, origem e SHA-256 em `d3/README.md`. Usada na renderização SVG do espectro, comparação e leitor compartilhado.

- JSZip 3.10.1: `jszip.min.js`, distribuição browser do pacote npm, licença MIT/GPLv3 em `jszip-LICENSE.md`. https://github.com/Stuk/jszip
- pdf-lib 1.17.1: `pdf-lib.min.js`, distribuição browser do pacote npm, licença MIT em `pdf-lib-LICENSE.md`. https://github.com/Hopding/pdf-lib

Copiadas do runtime local instalado. Manter os avisos de licença. Não carregar por CDN; exportação e projetos devem funcionar por `file://` e sem rede.
