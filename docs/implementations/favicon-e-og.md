# Implementação: Favicon e Identidade Social (OG)

**Objetivo:** Configurar o `favicon` e as meta tags de pré-visualização para o domínio `paraibaexplorer.com.br`.

## Alterações Realizadas
### index.html
- Adicionada a tag `<link rel="icon">` apontando para `assets/logo-fav.ico`.
- Atualizado o logotipo principal do cabeçalho para `assets/logo-full.png`.
- Implementadas as tags **Open Graph (OG)** reforçadas com `logo-full.png?v=3` para forçar a atualização no WhatsApp.
- Adicionado `apple-touch-icon` com `logo-fav.png`.

## Lógica e Dependências
- **Favicon:** `assets/logo-fav.ico`.
- **Preview Social:** `assets/logo-full.png`.
- **Domínio base:** `https://paraibaexplorer.com.br/`.

## Resultados Esperados
1. O ícone do TikTok deve aparecer na aba do navegador.
2. Ao compartilhar o link `https://paraibaexplorer.com.br/` em um chat, deve aparecer o título, a descrição e o logotipo do TikTok como miniatura.

## Histórico de Modificações
- **2026-05-11:** Implementação de favicon e OG tags para o lançamento do domínio próprio.
