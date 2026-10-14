# Formato de carregamento no ChatGPT

Os PNGs da release v1.0.0 são exportações das folhas v2 originais, específicas para o seletor **Carregar um mascote / Upload pet** do ChatGPT na web.

A [documentação oficial](https://learn.chatgpt.com/docs/pets) exige PNG ou WebP transparente de 1536 × 1872 pixels, até 20 MiB. Referência consultada em 14 de outubro de 2026.

## O que foi convertido

Cada célula tem 192 × 208 pixels. As folhas originais têm 8 colunas e 11 linhas. A exportação preserva a região `(0, 0, 1536, 1872)`: as primeiras nove linhas, contendo os nove estados e 57 quadros de animação. As 15 células sem uso continuam transparentes.

Não houve redimensionamento, recompressão com perda, mudança de cor nem redesenho. A comparação dos pixels RGBA decodificados confirmou igualdade exata entre os PNGs exportados e essa região dos originais. As duas linhas extras de olhar da v2 não fazem parte do layout v1.

## Validação executada

Os dois arquivos passaram pelo `validate_atlas.py` do contrato Pets: `ok: true`, sem erros ou avisos. Foram verificados formato PNG, canal RGBA, dimensões, quadros presentes, transparência das células sem uso, bordas e ausência de fundo cromático residual.

| Arquivo | Bytes | Resultado |
| :--- | ---: | :--- |
| `makima-chatgpt.png` | 875433 | v1 · aprovado estruturalmente |
| `makima-retrato-chatgpt.png` | 2125565 | v1 · aprovado estruturalmente |

Os relatórios estão em [`validation/`](validation/), e as somas SHA-256 em [`upload/SHA256SUMS`](../upload/SHA256SUMS).

Essa verificação confirma o formato dos arquivos. A disponibilidade e o aceite na interface dependem da conta, do workspace e da versão do ChatGPT; não foi realizado um carregamento de teste em uma conta de outro usuário.

## Cores do README

A identidade editorial usa rubro `#8C2635`, preto vinho `#1A0B11`, marfim `#F9F0E3` e dourado `#D7AF70`. As imagens de capa e os cartões reutilizam os sprites existentes; o fundo das prévias é apenas parte da apresentação do repositório. Os PNGs de carregamento mantêm transparência.
