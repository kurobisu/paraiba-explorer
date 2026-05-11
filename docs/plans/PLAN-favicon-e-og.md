# Plano de Implementação: Favicon e Meta Tags (Open Graph)

**Objetivo:** Configurar a imagem `assets/tiktok.png` como favicon do site e garantir que ela apareça corretamente em pré-visualizações de chats (WhatsApp, Telegram, etc.) através de tags Open Graph.

## Arquivos Afetados
- `index.html` (Inserção das tags `<link>` e `<meta>`)
- `docs/Kanban - paraiba-explorer.md` (Atualização de status)

## Lógica de Implementação
Para atingir o objetivo de aparecer no WhatsApp, não basta apenas o favicon; é necessário implementar as tags de Open Graph (OG).

### 1. Favicon
Adicionar a tag `<link rel="icon" ...>` apontando para `assets/tiktok.png`.

### 2. Open Graph (WhatsApp/Social)
Adicionar as seguintes meta tags:
- `og:image`: URL absoluta da imagem.
- `og:title`: Título do site.
- `og:description`: Descrição breve.
- `og:url`: URL do site (`https://paraibaexplorer.com.br`).

## Dependências
- Existência do arquivo `assets/tiktok.png` (Confirmado).

## Histórico de Modificações
- **2026-05-11:** Criação do plano para melhoria visual e SEO social.
