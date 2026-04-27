# 🛒 Adzin Imports — Site Institucional

Site institucional da **Adzin Imports**, loja de eletrônicos premium localizada em Brasília-DF, especializada em iPhones, celulares, computadores e acessórios importados.

---

## 📁 Estrutura do Projeto

```
adzin-imports/
├── index.html          # Página principal
├── style.css           # Estilos personalizados
└── img/
    ├── logo-adzin.png  # Favicon e logo
    ├── categoria.jpg   # Imagem de fundo do Hero
    ├── iPhone.jpg      # Slide 1 do carrossel
    ├── PC-Gamer.png    # Slide 2 do carrossel
    └── Fones-de-Ouvido.jpg  # Slide 3 do carrossel
```

---

## 🚀 Tecnologias Utilizadas

| Tecnologia | Versão | Finalidade |
|---|---|---|
| HTML5 | — | Estrutura da página |
| CSS3 | — | Estilos personalizados |
| Bootstrap | 5.3.3 | Layout responsivo e componentes |
| Bootstrap Icons | 1.11.3 | Ícones (Instagram, WhatsApp, etc.) |
| Google Fonts (Montserrat) | — | Tipografia |
| Google Maps Embed | — | Mapa de localização |

---

## 🗂️ Seções da Página

1. **Navbar** — Fixa no topo com o nome da marca e efeito glassmorphism (backdrop blur).
2. **Hero Section** — Tela cheia com imagem de fundo, título, descrição e botões de ação.
3. **Carrossel** — 3 slides com fade automático a cada 4 segundos mostrando as categorias de produtos.
4. **Localização** — Endereço e mapa embutido do Google Maps (Shopping Popular de Ceilândia — BOX 466).
5. **Redes Sociais** — Links para Instagram e Grupo do WhatsApp.
6. **Footer** — Copyright.

---

## 🔧 Correções Realizadas (v1.1)

### HTML
- **Âncora quebrada:** `href="#Redes Sociais"` (com espaço) não funciona como âncora HTML. Corrigido para `href="#redes-sociais"` e o `id` da seção atualizado para `id="redes-sociais"`.
- **Âncora do carrossel:** `id="carrosselPremium"` com acento não é padrão seguro. Renomeado para `id="catalogo"` e todos os `data-bs-target` atualizados.
- **Markup inválido:** `<a>` dentro de `<h1>` dentro de outro `<a>` na navbar. Simplificado para um único `<a>` com a classe correta.
- **Botão "Voltar ao Início":** Tinha `href="#"` que não faz scroll. Corrigido para `href="#top"` com `id="top"` no `<body>`.
- **Links externos:** Adicionado `rel="noopener noreferrer"` em todos os links `target="_blank"` (segurança).
- **iframe acessibilidade:** Adicionado atributo `title` no iframe do Google Maps.
- **Hover inline removido:** `onmouseover`/`onmouseout` inline removidos dos botões de redes sociais e migrados para CSS.

### CSS
- **`scroll-behavior: smooth`** adicionado ao `html` — necessário para as âncoras funcionarem com animação suave.
- **`-webkit-backdrop-filter`** adicionado na navbar — corrige o efeito de blur no Safari/iOS.
- **`background-attachment: scroll`** no Hero — `fixed` não funciona no iOS causando fundo branco/bugado.
- **`min-height: 100svh`** no Hero mobile — `svh` (small viewport height) corrige o bug clássico onde a barra de endereço do Chrome/Safari no celular corta a seção.
- **Padding top no `.hero-content`** — evita que o texto fique escondido atrás da navbar fixa.
- **`height` explícita no iframe** — sem isso, alguns browsers mobile não renderizam o mapa.
- **Botões sociais em CSS** — classes `.btn-social`, `.btn-instagram`, `.btn-whatsapp`, `.btn-inicio` criadas, deixando o HTML limpo e facilitando manutenção.
- **`font-family` no body** — aplicado globalmente para consistência em toda a página.
- **Media query `@media (max-width: 400px)`** — ajustes extras para telas muito pequenas (ex: iPhone SE).

---

## 📱 Compatibilidade

- ✅ Chrome (Android / Desktop)
- ✅ Safari (iOS / macOS)
- ✅ Firefox
- ✅ Samsung Internet
- ✅ Edge

---

## 📍 Localização

**Shopping Popular de Ceilândia — BOX 466**
Brasília — DF, Brasil

---

## 🔗 Redes Sociais

- **Instagram:** [@adzin_imports](https://www.instagram.com/adzin_imports/)
- **WhatsApp:** [Grupo de Novidades](https://chat.whatsapp.com/EaLRkC482NACoDQsj18sL2)

---

## 👤 Autor

**Tiago de Aquino Nunes**

---

## 📄 Licença

© 2026 Adzin Imports. Todos os direitos reservados.
