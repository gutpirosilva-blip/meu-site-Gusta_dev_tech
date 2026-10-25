# Gusta Dev Tech

Site de apresentação de **Gustavo Rodrigues | Dev & Design** (@gusta_dev_tech), Pesqueira, PE.
Sites, landing pages, agentes de IA, logos, design 3D e animações.

É uma página única, em HTML, CSS e JavaScript puros. Não tem build, dependências nem servidor.

## Estrutura

```
gusta-dev-tech/
├── index.html        # o site inteiro (estilos, scripts e imagens já embutidos)
├── README.md
└── assets/
    ├── logo-gr.jpg               # logo da capa
    ├── avatar.jpg                # foto redonda (topo e seção Sobre)
    ├── policlinica-franca.jpg    # print do site no portfólio
    └── originais/                # imagens originais enviadas
```

O `index.html` funciona sozinho: as três imagens estão embutidas nele.
A pasta `assets/` guarda as mesmas imagens para você reutilizar ou trocar.

## Seções do site

Topo com menu, capa com texto digitado e logo animado, faixa de serviços,
Serviços, Portfólio, Como funciona, Sobre, Perguntas frequentes,
Pedir orçamento e rodapé. Há também um botão flutuante de WhatsApp.
O site tem somente o tema escuro (preto com dourado).

## Como publicar na Vercel

1. Crie um repositório no GitHub (ex.: `gusta-dev-tech`).
2. Envie o `index.html` para a raiz do repositório (Add file > Upload files).
3. Em vercel.com, entre com o GitHub e clique em Add New > Project.
4. Importe o repositório, deixe Framework Preset como **Other**, sem comando de build, e clique em **Deploy**.

Pelo terminal: instale com `npm i -g vercel`, entre na pasta e rode `vercel`, depois `vercel --prod`.
Qualquer hospedagem estática (Netlify, GitHub Pages, Cloudflare Pages) também serve.

## O que editar

Abra o `index.html` em um editor de texto e procure por:

| O que mudar | Procure por |
|---|---|
| Número do WhatsApp | `5587992051783` (aparece em vários links) e `(87) 99205-1783` |
| Instagram | `instagram.com/gusta_dev_tech` |
| Textos de Serviços, Como funciona e Perguntas frequentes | `id="servicos"`, `id="como"`, `id="faq"` |
| Texto da seção Sobre | `id="sobre"` |
| Projetos do portfólio | `id="portfolio"` |
| Cores | variáveis no início do `<style>`: `--bg`, `--gold`, `--ink` |

Para trocar uma imagem pelo arquivo novo, o jeito mais fácil é pedir ao Claude que atualize o `index.html`,
pois as imagens estão embutidas em formato base64.

## Observações

- O número usa o código do Brasil (+55). Teste os botões de WhatsApp depois de publicar.
- Os textos de **Como funciona** e **Perguntas frequentes** são sugestões. Revise para refletir o seu jeito de trabalhar.
- As fontes (Bricolage Grotesque e Figtree) vêm do Google Fonts, então é preciso internet para o visual completo.
- As animações são desligadas para quem usa "reduzir movimento" no aparelho.
- O botão de WhatsApp só pulsa quando o mouse passa por cima.

## O que falta fazer

### Antes de publicar
- [ ] Testar o botão flutuante de WhatsApp e o "Enviar no WhatsApp" do orçamento (abrem a conversa com (87) 99205-1783?)
- [ ] Revisar os textos de **Como funciona** e **Perguntas frequentes** (prazo, pagamento, o que o cliente envia)
- [ ] Revisar a descrição de cada serviço em **Serviços**
- [ ] Abrir o site no celular e no computador e conferir se tudo aparece bem
- [ ] Confirmar que as imagens (logo, avatar, print da Policlínica França) estão corretas

### Publicação
- [ ] Criar o repositório no GitHub e enviar o `index.html`
- [ ] Fazer o deploy na Vercel
- [ ] Testar o endereço `.vercel.app` depois de publicado
- [ ] Colocar o link do site na bio do Instagram @gusta_dev_tech

### Melhorias futuras
- [ ] Adicionar mais projetos ao portfólio, com imagens
- [ ] Incluir depoimentos de clientes (a Policlínica França pode ser a primeira)
- [ ] Botão "Ver site" nos projetos que estão no ar
- [ ] Galeria de logos e design 3D
- [ ] Seção de antes e depois
- [ ] Domínio próprio (Settings > Domains na Vercel)
- [ ] Ajustar o título e a descrição para busca (ex.: "criação de sites em Pesqueira")
