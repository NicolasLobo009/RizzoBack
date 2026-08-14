# RIZZOBACK — Site Oficial
## Guia de Personalização

---

## ✅ O que está pronto

- Estrutura completa do site (HTML + CSS + JS) em um único arquivo `index.html`
- Design elegante com paleta vinho, bege e verde cipó nos detalhes
- Header fixo com menu hambúrguer para celular
- Hero com destaque para fotografia real
- Seção de destaques (Moda Feminina, Fardamentos, Atendimento)
- Galeria de produtos com filtros por categoria
- Seção Sobre
- Seção Fardamentos
- CTA de conversão
- Localização com botão Google Maps
- Redes sociais
- Footer completo
- SEO básico configurado (title, meta description, Open Graph, Schema.org)
- `robots.txt` e `sitemap.xml`
- WhatsApp flutuante fixo na tela

---

## 🔧 O que você precisa personalizar

### 1. NÚMERO DO WHATSAPP
Busque e substitua todas as ocorrências de:
```
SEUNUMERODEWHATSAPP
```
Pelo número completo com código do país (sem espaços, traços ou parênteses):
```
5582912345678
```
Exemplo de link final: `https://wa.me/5582912345678?text=...`

---

### 2. LOGO
No header (linha com `nav-logo`), substitua o bloco de texto pela imagem real:
```html
<img src="imagens/logo-rizzoback.png"
     alt="Logo RIZZOBACK"
     class="nav-logo-img"
     width="48"
     height="48" />
```
Coloque sua logo na pasta `imagens/`.

No footer, faça o mesmo (versão branca/clara da logo se disponível).

---

### 3. FOTOGRAFIA HERO (imagem principal)
Procure o comentário `SUBSTITUA PELO CAMINHO DA SUA IMAGEM HERO` e substitua pelo `<img>` real:
```html
<img src="imagens/hero-rizzoback.jpg"
     alt="Vitrine e produtos da RIZZOBACK, loja de moda feminina em Maceió"
     class="hero-img"
     width="800"
     height="1000"
     loading="eager"
     fetchpriority="high" />
```

---

### 4. FOTOGRAFIA DA LOJA (Seção Sobre)
Procure `SUBSTITUA PELA FOTOGRAFIA REAL DA LOJA` e substitua pelo `<img>` correspondente.

---

### 5. FOTOGRAFIA DOS FARDAMENTOS
Procure `SUBSTITUA PELA FOTOGRAFIA REAL DOS FARDAMENTOS` e substitua pelo `<img>` correspondente.

---

### 6. ADICIONAR PRODUTOS / PEÇAS

Para cada produto, copie o modelo de card abaixo e cole dentro de `<div class="products-grid" id="products-grid">`:

```html
<article class="product-card" data-category="moda-feminina">
  <div class="product-img-wrap">
    <img src="imagens/pecas/nome-da-peca.jpg"
         alt="Nome da Peça — RIZZOBACK Maceió"
         width="400"
         height="533"
         loading="lazy" />
    <span class="product-tag">Novidade</span>   <!-- opcional -->
  </div>
  <div class="product-body">
    <p class="product-category">Moda Feminina</p>
    <h3 class="product-name">Nome da Peça</h3>
    <div class="product-footer">
      <a href="https://wa.me/5582912345678?text=Olá!+Tenho+interesse+na+peça+Nome+da+Peça+que+vi+no+site+da+RIZZOBACK."
         class="btn btn-primary btn-sm"
         target="_blank"
         rel="noopener noreferrer">
        Tenho interesse
      </a>
    </div>
  </div>
</article>
```

**Categorias disponíveis para `data-category`:**
- `moda-feminina`
- `fardamentos`
- `novidades`

Quando tiver produtos suficientes, remova o bloco `<div class="placeholder-notice">`.

---

### 7. INSTAGRAM
Procure `https://instagram.com/SEUPERFIL` e substitua pelo link real do perfil da RIZZOBACK.

Atualize também o `@rizzoback` para o @ correto.

---

### 8. MAPA (Google Maps incorporado)
1. Acesse https://maps.google.com
2. Pesquise o endereço: "Rua Miguel Palmeira, 908, Pinheiro, Maceió"
3. Clique em **Compartilhar → Incorporar um mapa**
4. Copie o código `<iframe>` e substitua o `<div class="loc-map-placeholder">` pelo iframe.

---

### 9. HORÁRIO DE FUNCIONAMENTO
Na seção de localização, substitua o texto de horários pelo horário real da loja.

---

### 10. SOBRE A RIZZOBACK (texto)
O texto da seção "Sobre" pode ser personalizado. Substitua pelos dados reais da RIZZOBACK (história, fundação, diferenciais).

---

### 11. SITEMAP
No arquivo `sitemap.xml`, atualize a data (`<lastmod>`) e a URL (`<loc>`) quando o site for publicado.

---

### 12. OPEN GRAPH (imagem para compartilhamento)
Adicione no `<head>` do `index.html`, dentro das tags Open Graph:
```html
<meta property="og:image" content="https://www.rizzoback.com.br/imagens/og-rizzoback.jpg" />
```
A imagem ideal para Open Graph é 1200×630px.

---

## 📁 Estrutura de pastas sugerida

```
rizzoback/
├── index.html
├── robots.txt
├── sitemap.xml
├── LEIA-ME.md
└── imagens/
    ├── logo-rizzoback.png
    ├── logo-rizzoback-branca.png
    ├── hero-rizzoback.jpg
    ├── loja-rizzoback.jpg
    ├── fardamentos-rizzoback.jpg
    ├── og-rizzoback.jpg
    └── pecas/
        ├── peca-01.jpg
        ├── peca-02.jpg
        └── ...
```

---

## 🌐 Publicação

Este site é um arquivo HTML estático. Pode ser hospedado em:
- **Hostinger** (recomendado para iniciantes)
- **Netlify** (gratuito, drag & drop)
- **GitHub Pages** (gratuito)
- **Qualquer hospedagem compartilhada** com suporte a HTML

Basta fazer upload dos arquivos para a pasta `public_html` do seu servidor.

---

## 📞 Dúvidas

Entre em contato com quem desenvolveu o site para qualquer ajuste.
