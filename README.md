# Portfolio — Social Media

Site de portfólio pessoal desenvolvido para uma profissional de Social Media & Criadora de Conteúdo, com design editorial, autenticação real e gerenciamento de vídeos via painel admin.

## Tecnologias utilizadas

- **HTML5** — estrutura semântica
- **CSS3** — Grid, Flexbox, animações, `clip-path`, `drop-shadow`
- **JavaScript (Vanilla)** — sem frameworks, upload, autenticação e renderização dinâmica
- **Supabase** — autenticação (Auth) e armazenamento de vídeos (Storage)
- **GitHub Pages** — hospedagem estática gratuita

## Funcionalidades

- Design responsivo com tipografia editorial
- Cursor customizado animado
- Animações de scroll com Intersection Observer
- Portfólio de vídeos carregados dinamicamente via Supabase Storage
- **Upload de vídeos com barra de progresso e legenda opcional** — gerencie seu portfólio direto pelo site, sem precisar mexer no código
- Autenticação real via Supabase Auth
- **Área admin protegida por login** — faça upload e delete vídeos com segurança pela própria interface do site
- Botão flutuante de WhatsApp
- Proteção via RLS (Row Level Security) no Supabase

## Como configurar

### 1. Supabase

1. Crie uma conta em [supabase.com](https://supabase.com)
2. Crie um novo projeto
3. Vá em **Storage** e crie um bucket chamado `videos`
4. Vá em **Authentication → Users** e crie o usuário admin
5. Copie a **URL** e a **anon key** em **Project Settings → API**

### 2. Conectar ao projeto

No `index.html`, localize e preencha:

```js
const SB_URL = 'SUA_SUPABASE_URL';
const SB_KEY = 'SUA_SUPABASE_ANON_KEY';
```

### 3. Área Admin

A área de upload é oculta para visitantes. Para acessar, adicione `?admin=1` na URL e faça login com as credenciais criadas no Supabase.

### 4. Deploy no GitHub Pages

1. Suba os arquivos para um repositório público
2. Vá em **Settings → Pages → Branch: main → Save**
3. O site ficará em `https://seuusuario.github.io/nomerepositorio`

## Arquivos necessários

```
index.html   — página principal
1.png        — foto principal
2.png        — foto seção sobre (opcional)
3.png        — foto seção sobre (opcional)
README.md
```
