# Política de Segurança — PortfolioHUB

## Visão Geral
A segurança das informações e a proteção de dados são prioridades no desenvolvimento e manutenção do **PortfolioHUB**. Este documento estabelece as diretrizes de segurança, versões suportadas e o procedimento para reporte responsável de vulnerabilidades.

## Versões Suportadas
Apenas a versão mais recente em execução no ambiente de produção (`main`) recebe atualizações de segurança e correções ativas.

| Versão | Suportada |
| :--- | :--- |
| Branch `main` (Produção / GitHub Pages) | :white_check_mark: Sim |
| Branches secundárias / Forks não mesclados | :x: Não |

## Como Reportar Vulnerabilidades de Forma Privada
Se você identificar uma falha ou vulnerabilidade de segurança no repositório ou na aplicação **PortfolioHUB**, **NÃO** abra uma Issue pública. Em vez disso, siga os passos abaixo:

1. Envie um e-mail privado detalhando a vulnerabilidade para o responsável pela segurança do repositório.
2. Inclua as seguintes informações no e-mail:
   - Descrição detalhada da vulnerabilidade.
   - Passos necessários para reproduzir o problema.
   - O impacto potencial da exploração da falha.
   - Sugestão de correção (se houver).

## Prazo de Resposta e Tratamento
- **Confirmação do Recebimento:** Comprometemo-nos a responder e confirmar o recebimento do seu reporte no prazo máximo de **48 horas**.
- **Avaliação e Correção:** A equipe analisará a falha, definirá um plano de mitigação e aplicará a correção necessária em até **7 dias úteis**.
- **Divulgação Responsável:** Após a publicação da correção em produção, o relator receberá os devidos créditos no histórico do repositório (caso deseje).

## Boas Práticas Implementadas no Repositório
- **Autenticação em Duas Etapas (2FA):** Obrigatória para todos os colaboradores do projeto.
- **Proteção da Branch `main`:** Bloqueio de pushes diretos e exigência de Pull Requests com revisão.
- **Gestão de Segredos:** Proibição do commit de chaves de API, credenciais ou tokens. Uso de GitHub Secrets para dados sensíveis.
- **Monitoramento com Dependabot:** Varredura automática contínua de dependências vulneráveis.
- **Conformidade com a LGPD:** Bloqueio e sanitização de Dados Pessoais Identificáveis (PII).
