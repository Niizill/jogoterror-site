# POSTO 13 — site oficial

Site estático e responsivo do jogo de terror **POSTO 13**, criado por **NILTWON**, hospedado na Vercel e conectado ao repositório `Niizill/jogoterror-site`.

O conteúdo público descreve apenas recursos informados pelo criador: terror 3D em Godot, exploração do posto de gasolina, monstro, lanterna, inventário de quatro espaços e multiplayer online de até quatro jogadores. A galeria usa capturas da intro 3D e referências do monstro enviadas pelo criador (não fotos de banco de imagens).

## Como publicar uma nova versão do jogo

**Versão publicada e verificada durante a atualização deste site:** `v1.0.0`, com arquivos `Posto13.exe` (Windows) e `Posto13-Android.apk` (Android).

Para lançar uma versão nova, por exemplo **v1.0.1**:

1. Exporte a nova versão no Godot e teste no Windows e no Android.
2. Para Windows, compacte em `Posto13-Windows.zip` caso a exportação tenha arquivos auxiliares como `.pck`. Se o executável for realmente autossuficiente, você também pode publicar `Posto13.exe`.
3. Para Android, exporte `Posto13-Android.apk` com o **mesmo package ID e certificado de assinatura** da versão anterior para permitir atualização sem desinstalar.
4. Acesse **https://github.com/Niizill/jogoterror-site/releases/new**.
5. Escolha **Choose a tag → v1.0.1 → Create new tag**, dê um nome à atualização e descreva as mudanças reais.
6. Arraste o novo arquivo de Windows e o novo APK para o campo de anexos da Release, aguarde terminar e clique em **Publish release**. Não marque como `draft` ou `pre-release` se deseja disponibilizá-la no site.
7. Pronto: a página de downloads do site consulta as Releases públicas e escolhe **o arquivo mais recente de cada plataforma**. Não precisa editar o HTML a cada atualização.

**Se atualizar só o Windows ou só o Android**, o site mantém o arquivo mais recente disponível da outra plataforma. O site não substitui os arquivos do jogo nem atualiza instalações automaticamente: o jogador precisa baixar e instalar a nova versão.

Não envie arquivos do jogo enormes como commits comuns: use os **assets das GitHub Releases**, que aceitam arquivos grandes.

## Como atualizar a galeria

A imagem compactada `assets/galeria/posto13-cenas.svg` contém quatro capturas/referências reais organizadas em uma grade 2 × 2 (duas da intro e duas do modelo do monstro). O site reutiliza as quatro regiões para reduzir peso e armazenamento. Para trocar as imagens, atualize esse recurso preservando a grade 2 × 2.

A página identifica separadamente o que é captura da intro e o que é referência do modelo.

## Publicação na Vercel

O projeto usa HTML, CSS e JavaScript, sem build, com configuração em `vercel.json`. A branch principal é `main`. Alterações enviadas ao GitHub normalmente iniciam uma nova publicação no projeto Vercel conectado. Se uma alteração não aparecer, consulte **Vercel → jogoterror-site → Deployments** e confirme a integração.

## Arquivos do site

- `index.html`: layout, galeria, FAQ e busca de versões nas GitHub Releases
- `assets/galeria/posto13-cenas.svg`: galeria otimizada com imagens reais do projeto
- `favicon.svg`: ícone
- `vercel.json`: configurações e headers

Os links de download oficiais vêm de https://github.com/Niizill/jogoterror-site/releases.
