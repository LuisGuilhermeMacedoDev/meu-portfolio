# Plano de Implantação e Arquitetura: PortfolioHUB

## 1. Visão Geral e Escopo
O **PortfolioHUB** é uma plataforma centralizada e escalável desenvolvida para a exibição, organização e gerenciamento de projetos de tecnologia. O escopo abrange desde projetos acadêmicos em Análise e Desenvolvimento de Sistemas até implementações web completas e infraestrutura em nuvem (como laboratórios AWS). O objetivo é garantir um ambiente de alta disponibilidade, versionamento seguro e processos automatizados.

## 2. Arquitetura e Stack Tecnológica
A infraestrutura e o desenvolvimento da aplicação baseiam-se nos seguintes pilares:
* **Frontend:** HTML5, CSS3, JavaScript.
* **Backend e Scripts:** Java e Python (para automações e lógica de negócios).
* **Infraestrutura e Nuvem:** Conceitos de Cloud Computing baseados na AWS Cloud Foundations, visando futura integração de CI/CD e hospedagem de aplicações multicamadas.
* **Versionamento:** Git e GitHub.

## 3. Configuração do Ambiente e Versionamento
* **Repositório Central:** Estruturação modular com separação clara de domínios (`/projetos-pessoais`, `/projetos-academicos`).
* **Estratégia de Branching:** Utilização de um fluxo baseado em *GitHub Flow*.
  * `main`: Ambiente de produção, refletindo sempre o código estável e funcional.
  * `feature/*`: Ramificações isoladas para desenvolvimento de novas funcionalidades ou adição de novos projetos.

## 4. Gestão de Usuários e Políticas de Segurança
O ambiente foi configurado utilizando o modelo de controle de acesso baseado em funções (RBAC) e as ferramentas nativas de segurança do GitHub, orientadas por IA (Gemini):
* **Proteção de Produção:** A branch `main` possui um *Ruleset* ativo que bloqueia commits diretos (Block force pushes).
* **Revisão Obrigatória:** Toda alteração de código exige a abertura de um Pull Request (PR) prévio.
* **Auditoria de Acesso:** Manutenção de logs de commit e histórico linear para garantir a rastreabilidade de todas as alterações feitas na base de código.

## 5. Testes e Validação
1. **Validação de Acesso:** Simulação de tentativas de envio direto para a `main` para certificar o bloqueio por política de segurança.
2. **Integração:** Testes de resolução de conflitos e validação de merge através de Pull Requests.
3. **Auditoria Documental:** Revisão dos guias de contribuição e arquivos README.md para garantir conformidade com as exigências do projeto.
