# POSTO 13 — site oficial

Landing page de terror/sobrevivência para o jogo POSTO 13. Layout estático responsivo (HTML, CSS, JS) pronto para Vercel.

## Publicar downloads

O executável do jogo tem cerca de 310 MiB, acima do limite de 100 MiB por arquivo comum no GitHub. Não inclua o .exe diretamente nos commits.

1. Altere a visibilidade deste repositório para Public em Settings > General > Danger Zone > Change repository visibility, depois de conferir que não há código ou materiais confidenciais.
2. Entre em Releases > Draft a new release.
3. Crie uma tag, por exemplo, v1.0.0, e anexe o arquivo Posto13.exe em Attach binaries (GitHub Releases aceita arquivos individuais de até 2 GiB).
4. Publique a release. Quando o GitHub disponibilizá-la publicamente, o site pesquisa as 10 releases públicas mais recentes e ativa automaticamente o botão do Windows ao localizar exatamente Posto13.exe.
5. Quando houver Android, anexe Posto13.apk à mesma release ou a uma release posterior. O site mantém ambos os botões disponíveis se os arquivos estiverem em qualquer uma das 10 releases públicas mais recentes.

Repositórios privados não fornecem downloads anônimos. Para manter o repositório privado, publique os arquivos em um host público separado e altere o HTML para esse URL.

## Vercel

Conecte este repositório à Vercel com Framework Preset: Other e Root Directory: .
Não há npm nem build. A configuração vercel.json adiciona alguns cabeçalhos de segurança.

## Imagem de ambientação

Fotografia por Markus Spiske / Pexels, https://www.pexels.com/photo/lights-night-dark-gas-92077/ . É uma foto ilustrativa, não uma screenshot do jogo.

Arquivos: index.html, favicon.svg, vercel.json.