# Debugou

Landing page para vender sites a pequenos negócios: landing page, domínio, hospedagem e Perfil da Empresa no Google, com a promessa de achar o "bug" da presença online do cliente e corrigir.

Projeto estático, feito apenas com HTML, CSS e JavaScript, sem build e sem dependências.

## O que tem na página

- **Diagnóstico interativo** no topo, que mostra os problemas de um negócio sem site e os corrige em sequência.
- **Quem está por trás**, com foto, apresentação e links para GitHub e LinkedIn.
- **Quatro jeitos de criar o site**: Lovable, Base44, Claude e Wix, em abas.
- **Planos com preço fechado** (Start, Pro e Premium), com o Pro destacado como mais popular.
- **Serviço extra**: criação do Perfil da Empresa no Google.
- **Envio de briefing em PDF**, com validação de tipo e tamanho (até 10 MB).
- **Integração com WhatsApp**: ao escolher um plano, abre uma conversa com a mensagem pronta informando o plano, o extra e o nome do negócio.

## Estrutura

    debugou/
    ├── index.html   # página completa (HTML, CSS e JS)
    ├── foto.jpg     # foto exibida na seção "Quem está por trás"
    ├── README.md
    └── .gitignore

## Como rodar localmente

Abra o `index.html` no navegador. Não precisa instalar nada.

## Como publicar na Vercel

1. Suba os arquivos na **raiz** de um repositório no GitHub (o `index.html` e o `foto.jpg` lado a lado).
2. Na Vercel, clique em **Add New → Project** e importe o repositório.
3. Clique em **Deploy**. Não precisa de nenhuma configuração extra.

A cada novo commit, a Vercel publica a atualização automaticamente.

## Como personalizar

Tudo fica no `index.html`:

- **Número do WhatsApp:** constante `WA` no início do script, no formato `55` + DDD + número.
- **Planos e preços:** array `plans`.
- **Valor do extra do Google:** procure por `R$ 190` no HTML e no script.
- **Foto:** substitua o `foto.jpg` mantendo o mesmo nome, ou altere o `src` da tag `<img class="avatar">`.
- **Cores:** variáveis no bloco `:root` do CSS.

## Observação sobre o upload de PDF

Como o site é estático, o PDF não é armazenado. No celular, o botão abre o compartilhamento direto para o WhatsApp. No computador, abre a conversa e o cliente anexa o arquivo manualmente. Para receber os arquivos automaticamente, é possível integrar um serviço de formulários, como o Formspree.

## Autora

**Layse Rondon**, Petrolina-PE
[GitHub](https://github.com/layserondon) · [LinkedIn](https://linkedin.com/in/layse-rondon)
