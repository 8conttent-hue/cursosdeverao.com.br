# CLAUDE.md — CURSOSDEVERAO

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** CURSOSDEVERAO
**Nicho:** Educação
**Keywords:** Cursos de verao e o lugar para quem procura informacoes sobre cursos
**Paleta de cores:** teal | **Fonte:** lora

Cursos de verão é o lugar para quem procura informações sobre cursos. Nós fornecemos informações detalhadas sobre uma ampla gama de cursos, facilitando para você encontrar o curso certo para você. Se você está interessado em estudar no exterior, tirar um ano livre, ou simplesmente quer aprender algo novo, nós temos o curso perfeito para você! Nossa missão é tornar o aprendizado fácil e divertido, para que todos possam descobrir sua paixão. Com os Cursos de Verão ao seu lado, não há limites para o que você pode alcançar!



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-C |
| Hero | Hero-B |
| Features | Features-F |
| About Section | About-J |
| Posts | Posts-G |
| Footer | Footer-I |
| Página Sobre | Sobre-H |
| Página Contato | Contato-H |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
