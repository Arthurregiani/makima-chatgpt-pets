# Makima — pets animados para ChatGPT

Este repositório oferece duas versões v2 de um pet de fã inspirado na Makima, de
*Chainsaw Man*, com spritesheets transparentes e prévias animadas:

- **Makima** — enquadramento de corpo inteiro;
- **Makima — Retrato** — enquadramento próximo, com o rosto maior.

As duas versões preservam a trança ruiva, os olhos dourados anelados e o traje
social escuro. Escolher um pet altera apenas a aparência do ChatGPT; não altera
as respostas nem as capacidades do produto.

## Prévia

| Makima | Makima — Retrato |
| --- | --- |
| ![Makima](assets/makima/preview.gif) | ![Makima — Retrato](assets/makima-retrato/preview.gif) |

## Usar no ChatGPT

### Instalar pelo app desktop

Os links abaixo usam o esquema `codex://` e abrem o fluxo de instalação no app
desktop do ChatGPT:

As duas folhas v2 têm 1536 × 2288 pixels, transparência e menos de 20 MiB:

- [Instalar Makima](codex://pets/install?name=Makima&imageUrl=https%3A%2F%2Fraw.githubusercontent.com%2FArthurregiani%2Fmakima-chatgpt-pets%2Fmain%2Fassets%2Fmakima%2Fspritesheet.png&description=Makima%20de%20Chainsaw%20Man%3A%20tranca%20ruiva%2C%20olhos%20dourados%20anelados%20e%20traje%20social.&spriteVersionNumber=2)
- [Instalar Makima — Retrato](codex://pets/install?name=Makima%20%E2%80%94%20Retrato&imageUrl=https%3A%2F%2Fraw.githubusercontent.com%2FArthurregiani%2Fmakima-chatgpt-pets%2Fmain%2Fassets%2Fmakima-retrato%2Fspritesheet.png&description=Makima%20em%20enquadramento%20pr%C3%B3ximo%2C%20com%20rosto%20e%20olhos%20dourados%20anelados%20em%20destaque.&spriteVersionNumber=2)

1. Instale ou atualize o app desktop do ChatGPT para macOS ou Windows.
2. Abra este README no computador com o app instalado e clique no link da
   versão desejada.
3. Permita que o sistema abra o link `codex://` no ChatGPT, se solicitado.
4. Revise o nome e a prévia no fluxo exibido e confirme a instalação.

### Selecionar, mostrar e ajustar

Depois da instalação:

1. Abra **Settings > Pets** no ChatGPT e selecione **Makima** ou
   **Makima — Retrato**.
2. No app desktop para macOS ou Windows, use `/pet` ou **Show pet** no menu de
   comandos para mostrar ou ocultar o pet flutuante.
3. Para ajustar o tamanho, abra **Settings > Pets > Customize > Pet size**.

### Criar manualmente com uma spritesheet

Se um link `codex://` não abrir, baixe o `spritesheet.png` da versão desejada
pelos caminhos abaixo e use **Create pet** no app desktop, se essa opção estiver
disponível:

- [`assets/makima/spritesheet.png`](assets/makima/spritesheet.png)
- [`assets/makima-retrato/spritesheet.png`](assets/makima-retrato/spritesheet.png)

No fluxo de criação, carregue a folha, informe um nome e salve o pet. O seletor
de upload pela web documentado pelo ChatGPT especifica a folha v1 (1536 ×
1872); estas artes são v2 (1536 × 2288), portanto os links de instalação no
desktop são a opção indicada para estes arquivos.

## Solução de problemas

- **O link não abre:** abra o README no app ou navegador do computador, confirme
  que o ChatGPT desktop está instalado e escolha o ChatGPT quando o sistema
  perguntar qual aplicativo deve abrir `codex://`.
- **A instalação não aparece:** atualize o app, entre na conta correta e
  verifique se **Settings > Pets** está disponível para o seu workspace.
- **O pet foi instalado, mas não aparece:** selecione-o em **Settings > Pets** e
  use `/pet` ou **Show pet** no app desktop para exibi-lo.
- **O tamanho não muda:** ajuste **Settings > Pets > Customize > Pet size** e
  confirme que o pet está selecionado; esse controle pode não existir em versões
  antigas do app.
- **O upload manual falha:** confirme que o arquivo é o `spritesheet.png`
  completo e tente o fluxo de instalação `codex://`; a documentação pública de
  upload pode aceitar apenas spritesheets v1.

## Requisitos e limitações

- É necessário usar uma versão do app ChatGPT que ofereça **Pets**; a
  disponibilidade pode variar por conta, workspace, sistema operacional e
  versão do aplicativo.
- A instalação por `codex://` requer o app desktop para macOS ou Windows com
  esse esquema de links habilitado. O link pode não funcionar em um navegador,
  no celular ou quando o app não está instalado.
- A seleção e a personalização ficam em **Settings > Pets**. Os comandos
  `/pet` e **Show pet** para o pet flutuante são recursos do app desktop.
- A opção de upload manual e os formatos aceitos podem variar conforme o
  produto. A documentação pública do upload pela web especifica spritesheets
  v1; estas imagens são spritesheets v2.
- O pet é uma camada visual: não muda o modelo, as respostas, as ferramentas
  nem as permissões da conta.

## Arquivos

Cada pasta em `assets/` contém:

- `spritesheet.png` — folha transparente v2 para instalação;
- `preview.gif` e `preview.mp4` — demonstração animada;
- `contact-sheet.png` — todas as animações;
- `idle-jump-idle.gif` — demonstração de movimento vertical;
- `look-loop.gif` — ciclo com os 16 olhares.

## Referência oficial

- [Pets no ChatGPT](https://learn.chatgpt.com/docs/pets) — escolher, mostrar e redimensionar pets; diferenças entre desktop e web.
- [Comandos e links profundos](https://learn.chatgpt.com/docs/reference/commands#pets) — fluxo `codex://pets/install` e parâmetro de versão v2.

## Créditos

Pet de fã, sem afiliação oficial. Makima e *Chainsaw Man* pertencem aos respectivos criadores e titulares de direitos. Este repositório compartilha as folhas e prévias para uso pessoal no ChatGPT; não concede direitos sobre a personagem ou a obra.
