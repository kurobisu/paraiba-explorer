# Implementação de Domínio Customizado

**Objetivo:** Transição do subdomínio GitHub para `paraibaexplorer.com.br`.

## Arquivos Afetados
- `CNAME`: Contém o nome do domínio para o GitHub Pages.

## Lógica e Configuração
A configuração foi dividida em duas partes:

### 1. Lado do Repositório (Concluído)
- Foi criado o arquivo `CNAME` na raiz do projeto.
- O GitHub lerá este arquivo e tentará associar o domínio ao repositório.

### 2. Lado do DNS (Registro.br) - Ação Necessária
Para que o domínio funcione, é necessário configurar os registros DNS no painel do Registro.br:

**Registros Tipo A (Apontam para os servidores do GitHub):**
- Host: `@` (ou deixe vazio) -> IP: `185.199.108.153`
- Host: `@` (ou deixe vazio) -> IP: `185.199.109.153`
- Host: `@` (ou deixe vazio) -> IP: `185.199.110.153`
- Host: `@` (ou deixe vazio) -> IP: `185.199.111.153`

**Registro Tipo CNAME (Aponta para o seu repositório):**
- Host: `www` -> Valor: `kurobisu.github.io`

## Verificação
Após as mudanças no DNS, pode levar de algumas horas até 48 horas para a propagação total. O status pode ser verificado em:
- Configurações do Repositório -> Pages -> Custom Domain.
- Recomendado marcar a opção "Enforce HTTPS" assim que o certificado SSL for gerado.

## Histórico de Modificações
- **2026-05-11:** Implementação inicial e documentação das etapas de DNS.
