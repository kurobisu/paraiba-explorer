# Plano de Configuração de Domínio Customizado

**Objetivo:** Substituir o link padrão do GitHub Pages (`https://kurobisu.github.io/paraiba-explorer/`) pelo domínio próprio `paraibaexplorer.com.br` adquirido no Registro.br.

## Arquivos Afetados
- `CNAME` (A ser criado na raiz do projeto)
- `docs/Kanban - paraiba-explorer.md` (Atualização de status)

## Lógica de Implementação
A transição para um domínio customizado no GitHub Pages envolve duas etapas principais: configuração no repositório GitHub e apontamento de DNS no provedor (Registro.br).

### Etapa 1: Configuração no GitHub
1. Criação de um arquivo chamado `CNAME` na raiz do repositório contendo apenas o domínio: `paraibaexplorer.com.br`.
2. Verificação das configurações de "Pages" no repositório para garantir que o domínio foi reconhecido.

### Etapa 2: Configuração no Registro.br (DNS)
1. Criar registros do tipo **A** apontando para os IPs do GitHub:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
2. Criar um registro do tipo **CNAME** para o subdomínio `www` apontando para `kurobisu.github.io`.

## Dependências
- Acesso administrativo ao repositório GitHub.
- Acesso à conta do Registro.br.

## Histórico de Modificações
- **2026-05-11:** Criação do plano inicial para migração de domínio.
