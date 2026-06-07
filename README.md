# Vila Dejulie — Landing (Lista de Espera)

Página de captação de lista de espera do **@viladejulie** — hotel boutique nascendo em
Jacumã, Costa do Conde, Paraíba. Site estático de um arquivo (`index.html`), hospedado
no **GitHub Pages**. O formulário envia os contatos para o **Brevo** (lista de e-mail própria).

---

## 🚀 Publicar no GitHub Pages

1. Crie um repositório novo no GitHub (ex.: `viladejulie-site`) — pode ser **público**.
2. Suba **o conteúdo desta pasta** (`index.html`, este README, `.nojekyll`) — veja os comandos abaixo.
3. No GitHub: **Settings → Pages → Build and deployment**.
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` · pasta `/ (root)` → **Save**.
4. Em ~1 min o site fica no ar em `https://SEU-USUARIO.github.io/viladejulie-site/`.
5. Cole essa URL no **link da bio** do Instagram. ✅

### Comandos (rodar DENTRO da pasta `site/`)
> ⚠️ **Importante:** inicialize o git **dentro de `site/`**, nunca na raiz do projeto —
> a pasta `Fotos e Videos/` tem ~59 GB e **não pode** ir para o GitHub.

```bash
git init
git add .
git commit -m "Landing lista de espera Vila Dejulie"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/viladejulie-site.git
git push -u origin main
```

---

## ✉️ Conectar o formulário ao Brevo

1. Crie a conta e a lista no **brevo.com** (plano grátis, contatos ilimitados).
2. **Contacts → Forms → Create a form** com os campos **NOME**, **EMAIL**, **SMS**
   (os mesmos nomes já usados no HTML).
3. Em *Confirmation*, redirecione de volta para a URL do site com `#ok` no final
   (mostra a mensagem de sucesso da Julie).
4. No `index.html`, troque o `action="TODO_COLE_AQUI..."` pela URL de action do Brevo.

> Alternativa: se preferir o código *embed* do Brevo em vez de editar o `action`,
> peça que adaptamos a página para encaixá-lo dentro do design.

---

## 🎨 Personalizações marcadas no código

- **Logo:** ✅ já embutido — o símbolo oficial (azulejo hidráulico) está inline no `<header>`
  e também salvo como `logo-vila-dejulie.svg` (usado no favicon). Vetor, nítido em qualquer tamanho.
- **Foto de fundo do hero:** linha comentada no CSS (`background ... url('hero.jpg')`).
  Coloque uma aérea do empreendimento como `hero.jpg` nesta pasta e descomente.
- **Imagem de compartilhamento (Open Graph):** troque `og-image.jpg` por uma imagem
  1200×630 do prédio para o link ficar bonito quando compartilhado.

---

## Domínio próprio (depois)

Quando tiver `viladejulie.com.br`: crie um arquivo `CNAME` nesta pasta com o domínio
dentro, aponte o DNS para o GitHub Pages e ative em *Settings → Pages → Custom domain*.

---

## Marca

Paleta Creme `#F1ECE0` · Azul Tijolo `#2D5A6B` · Terracota `#8B3F26` · Quase-preto `#2D2D2D`.
Tipografia Cormorant Garamond + DM Sans. Voz da Julie: 1ª pessoa, sem datas de abertura,
sem "sonho/promessa", sem CTA genérico.
