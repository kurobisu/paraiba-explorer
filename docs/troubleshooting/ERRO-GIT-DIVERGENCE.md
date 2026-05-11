# Erro: Divergência de Branches (Diverged Branches)

**Data:** 2026-05-11
**Erro:** O branch local `main` e o remoto `origin/main` divergiram, impedindo o `push`.
**Causa:** Um arquivo `CNAME` foi criado diretamente na interface do GitHub, enquanto simultaneamente um arquivo `CNAME` foi criado e commitado localmente.

## Solução Aplicada
1. Executado `git pull --rebase origin main` para integrar as mudanças remotas.
2. Identificado conflito no arquivo `CNAME`.
3. Resolução manual do conflito (ambos os arquivos continham o mesmo domínio `paraibaexplorer.com.br`).
4. Executado `git add CNAME` e `git rebase --continue`.
5. Efetuado `git push origin main` com sucesso.

## Prevenção
Evitar criar arquivos diretamente na interface web do GitHub quando estiver trabalhando localmente, ou sempre realizar um `git pull` antes de iniciar novas implementações locais.

[[PLAN-configuracao-dominio.md]]
