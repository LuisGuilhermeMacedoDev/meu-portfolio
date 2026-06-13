# Guia de Contribuição e Padrões de Qualidade

Bem-vindo ao guia de contribuição do **PortfolioHUB**. Este documento define os processos de colaboração, políticas de segurança e padrões de qualidade de código exigidos para manter a integridade deste repositório.

## 1. Políticas de Acesso e Segurança
Para garantir a estabilidade do ambiente de produção:
* **Nenhum desenvolvedor tem permissão para realizar *commits* diretos na branch `main`.**
* Todas as alterações devem ser feitas em ramificações (*branches*) isoladas e submetidas a revisão.
* Violações de segurança, como a exposição de credenciais de banco de dados ou chaves de API (ex: AWS, chaves privadas), resultarão na rejeição imediata do código.

## 2. Fluxo de Trabalho de Desenvolvimento
Recomendamos o seguinte fluxo para adicionar novos projetos ou corrigir bugs:

1. **Sincronização:** Certifique-se de que seu ambiente local está atualizado.
   ```bash
   git pull origin main
