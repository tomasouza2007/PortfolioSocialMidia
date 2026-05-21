# Barbara Luisa — Portfolio

Site pessoal de Social Media & Criadora de Conteúdo, hospedado via GitHub Pages com armazenamento de vídeos no Supabase.

## Estrutura

```
index.html   — página principal
1.png        — foto principal (hero + contato)
2.png        — foto seção sobre
3.png        — foto seção sobre
```

## Deploy no GitHub Pages

1. Suba todos os arquivos para um repositório público
2. Vá em **Settings → Pages**
3. Em **Branch**, selecione `main` e clique em **Save**
4. O site ficará disponível em `https://seuusuario.github.io/nomerepositorio`

## Upload de vídeos (área admin)

A área de upload é oculta por padrão. Para acessar, adicione `?admin=1` na URL:

```
https://seuusuario.github.io/nomerepositorio?admin=1
```

Os vídeos são enviados e armazenados no **Supabase** (bucket `videos`). Não ficam no GitHub.

## Tecnologias

- HTML + CSS + JavaScript puro
- [Supabase](https://supabase.com) — armazenamento de vídeos
- [Google Fonts](https://fonts.google.com) — Playfair Display + Syne
- GitHub Pages — hospedagem gratuita
