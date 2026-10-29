# NovaShop — versão corrigida para publicação

Este pacote foi reorganizado como site estático, porque o ZIP original estava inconsistente: `composer.json` continha rotas PHP, os arquivos de rotas e controladores estavam truncados, e arquivos HTML/CSS/JS tinham extensões erradas.

## Executar localmente

1. Extraia a pasta.
2. Abra a pasta no VS Code.
3. Instale a extensão **Live Server** (Ritwick Dey).
4. Clique com o botão direito em `index.html` e selecione **Open with Live Server**.

Alternativa: com Python instalado, execute `python -m http.server 8000` dentro desta pasta e abra `http://localhost:8000`.

## Publicar

- **Netlify**: envie esta pasta como deploy manual, ou conecte o repositório GitHub e use a raiz do projeto como diretório de publicação. Não é necessário comando de build.
- **GitHub Pages**: envie os arquivos para a raiz de um repositório e ative Pages para a branch principal, pasta `/ (root)`.

## Limitações importantes

Esta versão é frontend estático. Carrinho usa `localStorage` no navegador. Checkout, contato e painel administrativo são demonstrações: não processam pagamentos, não enviam e-mails, não possuem autenticação real nem banco de dados. Para uma loja real, será necessário backend e integração segura com pagamento.
