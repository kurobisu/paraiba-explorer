# Implementação: Favicon e Identidade Social (OG)

**Objetivo:** Configurar o `favicon` e as meta tags de pré-visualização para o domínio `paraibaexplorer.com.br`.

## Alterações Realizadas
### index.html
- Adicionada a tag `<link rel="icon">` apontando para `assets/tiktok.png`.
- Implementadas as tags **Open Graph (OG)** para compatibilidade com WhatsApp, Facebook e Instagram.
- Implementadas as tags **Twitter Card** para compatibilidade com o X (antigo Twitter).
- Utilizada URL absoluta (`https://paraibaexplorer.com.br/assets/tiktok.png`) para a imagem de pré-visualização, conforme requisito técnico de APIs de chat.

## Lógica e Dependências
- **Imagem base:** `assets/tiktok.png`.
- **Domínio base:** `https://paraibaexplorer.com.br/`.

## Resultados Esperados
1. O ícone do TikTok deve aparecer na aba do navegador.
2. Ao compartilhar o link `https://paraibaexplorer.com.br/` em um chat, deve aparecer o título, a descrição e o logotipo do TikTok como miniatura.

## Histórico de Modificações
- **2026-05-11:** Implementação de favicon e OG tags para o lançamento do domínio próprio.
