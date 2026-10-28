# RadHub — site institucional em Quarto

Este é um ponto de partida para o site `radhubcursos.com.br`, com página inicial, catálogo de cursos, blog e página Sobre.

## O que você precisa instalar

1.  **Quarto:** https://quarto.org/docs/get-started/
2.  **Git:** https://git-scm.com/downloads
3.  Um editor, como VS Code: https://code.visualstudio.com/

Você pode usar o Quarto pelo terminal sem instalar R. Se preferir, também pode trabalhar com RStudio/Positron.

## Visualizar localmente

Abra o terminal na pasta do projeto e execute:

``` bash
quarto preview
```

O Quarto abrirá o site no navegador e atualizará a prévia quando você salvar os arquivos.

## Gerar os arquivos do site

``` bash
quarto render
```

O site gerado ficará na pasta `_site`.

## Personalizar os cursos

Edite `cursos/index.qmd`. Procure por `https://pay.hotmart.com/SEU_LINK_AQUI` e substitua cada ocorrência pelo link real de vendas do curso correspondente na Hotmart.

**Não publique com os links de exemplo.**

## Publicar com domínio próprio

Uma opção é publicar a pasta gerada `_site` no GitHub Pages ou Netlify. Depois, configure `radhubcursos.com.br` como domínio personalizado no serviço escolhido e ajuste os registros DNS no Registro.br conforme as instruções oficiais do provedor.

O arquivo `_quarto.yml` já define o endereço principal como `https://radhubcursos.com.br`. Só configure o DNS quando estiver pronta para publicar.

## Estrutura

- `_quarto.yml`: configuração geral e menu
- `index.qmd`: página inicial
- `cursos/index.qmd`: catálogo de cursos
- `blog/index.qmd`: índice do blog
- `blog/como-estudar-fisica-medica.qmd`: artigo de exemplo
- `sobre.qmd`: apresentação do RadHub
- `styles.scss`: paleta, tipografia e componentes visuais
- `assets/radhub-icon.svg`: símbolo vetorial do RadHub, usado como logo e favicon

## Próximos ajustes recomendados

- Inserir links reais da Hotmart.
- Revisar o texto institucional e os detalhes de cada produto.
- Criar artigos e resoluções com referências.
- Configurar domínio, HTTPS, sitemap e ferramentas de análise de tráfego, se desejar.
- Revisar os links de redes sociais e as informações legais antes de publicar.
