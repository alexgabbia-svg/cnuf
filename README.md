# Site da CNUF

Site estático (um único `index.html`) para o GitHub Pages.

## 1. Receber as inscrições numa planilha
1. Crie uma planilha no Google Sheets (nome sugerido: "Inscrições CNUF").
2. Vá em Extensões > Apps Script, apague o código e cole o conteúdo de `Code.gs`.
3. Clique em Implantar > Nova implantação > tipo "App da Web".
   Executar como: você. Quem tem acesso: qualquer pessoa. Autorize quando o Google pedir.
4. Copie a URL gerada e cole na constante `ENDPOINT` no final do `index.html`.

Cada inscrição vira uma linha na planilha e o jogador recebe um e-mail de confirmação.
Contas gratuitas do Google enviam até cerca de 100 e-mails por dia.

## 2. Publicar no GitHub
1. Crie um repositório (por exemplo `cnuf`) e envie `index.html`, `Regulamento_Oficial_CNUF.pdf` e esta pasta.
2. Em Settings > Pages, escolha "Deploy from a branch", branch `main`, pasta `/ (root)`.
3. O site fica em `https://SEU-USUARIO.github.io/cnuf/`.

## 3. Manter o conteúdo
Troféus, ranking e Hall da Fama ficam no JavaScript do `index.html` (listas `O`, `E`, `R2` e `F`).
Para uma nova edição, basta acrescentar uma linha na lista `O`.
