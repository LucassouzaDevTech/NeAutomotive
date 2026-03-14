# NE Automotive — Site Institucional

Site institucional da NE Automotive, oficina de peças e serviços automotivos localizada em São Jerônimo da Serra, PR.

## Estrutura do projeto

```
ne-automotive/
├── index.html       # Página principal
├── style.css        # Estilos
├── main.js          # Scripts (nav, animações, smooth scroll)
└── imgs/            # Pasta de imagens (criar e adicionar as fotos)
    ├── amarok.jpeg
    ├── motorvectra.jpeg
    ├── fuquemotor.jpeg
    ├── amaroklfachada.jpeg
    └── fachadadia.jpeg
```

## Como usar

1. Clone ou baixe os arquivos do projeto
2. Crie a pasta `imgs/` na raiz
3. Adicione as fotos da galeria dentro de `imgs/`
4. Abra o `index.html` no navegador — pronto

Não há dependências, build ou instalação necessária. O site é HTML/CSS/JS puro.

## Seções

- **Hero** — chamada principal com botões de WhatsApp e scroll para serviços
- **Serviços** — 6 cards com os serviços oferecidos
- **Galeria** — grid de fotos da oficina e dos serviços
- **Sobre** — texto institucional e diferenciais da empresa
- **Contato** — endereço, telefones, mapa do Google e links sociais
- **CTA Final** — chamada para WhatsApp

## Personalização

### Alterar telefone / WhatsApp
Busque por `5543991787981` no `index.html` e substitua pelo número desejado (formato: `55` + DDD + número, sem espaços ou traços).

### Alterar endereço
Busque por `Avenida Pedro Ferreira da Costa` no `index.html`.

### Alterar o mapa
No `index.html`, localize a tag `<iframe>` dentro de `.map-placeholder` e substitua o atributo `src` pelo link de incorporação do Google Maps do endereço correto.

### Adicionar fotos na galeria
No `index.html`, localize a seção `gallery-grid` e adicione novos blocos seguindo o padrão:

```html
<div class="gallery-item">
  <img src="imgs/nome-da-foto.jpeg" alt="Descrição" loading="lazy" />
</div>
```

### Alterar cores
As variáveis de cor ficam no início do `style.css`, dentro de `:root`. As principais são:

```css
--red: #c8382a;         /* vermelho principal */
--red-bright: #e8453a;  /* vermelho no hover */
--bg: #0c0c0e;          /* fundo da página */
--text: #d4d4d8;        /* texto padrão */
```

## Deploy

O site é estático e funciona em qualquer hospedagem. Basta fazer upload dos arquivos:

- **Netlify** — arraste a pasta para o painel ou conecte ao GitHub
- **Vercel** — conecte o repositório e deploy automático
- **GitHub Pages** — ative em Settings → Pages → selecione a branch

## Tecnologias

- HTML5 semântico
- CSS3 com variáveis nativas e Grid Layout
- JavaScript vanilla (sem frameworks ou dependências)
- Google Fonts (Bebas Neue, Barlow Condensed, Barlow)
- Google Maps Embed API (mapa na seção de contato)
