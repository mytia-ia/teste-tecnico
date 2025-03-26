# Teste para candidatos à vaga de Desenvolvedor Backend Laravel
### Desafio

O objetivo deste teste é avaliar sua capacidade de desenvolver uma API robusta, escalável e bem estruturada utilizando Laravel. Você deverá criar um serviço de análise de sentimento baseado em IA para avaliações de produtos. O sistema deverá permitir que usuários registrem avaliações de produtos e, em segundo plano, um job deverá analisar o sentimento do texto utilizando uma API externa de NLP (Processamento de Linguagem Natural).

1. Funcionalidade do Projeto
Você deve desenvolver uma API que:
- Permita o cadastro de usuários com diferentes níveis de permissão (admin, moderador e usuário comum).
  - Autentique usuários e controle permissões usando Laravel Sanctum.
- Disponibilize endpoints RESTful para:
  - Gerenciamento de usuários:
    - Cadastro de usuários por convite (apenas administradores podem convidar novos usuários).
    - Autenticação e renovação de token.
    - Recuperação de senha via e-mail.
    - Alteração de perfil e permissões (restrito a administradores).
  - Gerenciamento de produtos:
    - Cadastro, listagem, edição e remoção de produtos (apenas administradores e moderadores podem cadastrar/editar/remover).
  - Gerenciamento de avaliações:
  - Cadastro de avaliações associadas a produtos, feitas apenas por usuários autenticados.
  - Listagem de avaliações por produto, incluindo análise de sentimento.
  - Exclusão de avaliações (apenas pelo próprio usuário ou administradores).
- Utilize jobs para processar as análises de sentimento em background.
- Consuma a API externa de NLP da MeaningCloud para identificar sentimentos nas avaliações. Documentação disponível em: https://www.meaningcloud.com/developer/sentiment-analysis.
- Implemente cache para otimizar consultas recorrentes.
- Utilize Docker para garantir fácil configuração e execução.

2. Diferenciais
Para se destacar no teste, considere os seguintes diferenciais:
- Implementação de GraphQL para consulta dos dados.
- Utilização de Observers para gerenciar eventos no sistema.
- Cobertura de testes consistente, incluindo testes unitários e de integração.
- Uso de Design Patterns (ex: Repository Pattern, Strategy, Factory, etc.).
- Documentação clara da API utilizando Swagger ou Postman.
- Proposta de melhoria na arquitetura do código.
- Tratamento adequado de erros e exceções.
- Código modular e de fácil manutenção.

3. Avaliação
Seu projeto será avaliado nos seguintes critérios:
- Arquitetura do Código: Organização e clareza do código.
- Uso correto de Laravel: Aplicação dos recursos do framework.
- Eficiência da solução: Performance e escalabilidade.
- Testes: Cobertura e qualidade dos testes automatizados.
- Manutenibilidade: Facilidade de expansão do código.
- Tratamento de Erros: Robustez e segurança.
- Uso de Docker: Configuração correta para ambiente de desenvolvimento.

4. Boas Práticas
Para garantir um código de qualidade, siga estas recomendações:
- Utilize PSR-4 para organização do código.
- Escreva commits semânticos e bem documentados.
- Utilize env variables para credenciais e configurações sensíveis.
- Prefira Service Providers e Repositories para desacoplar regras de negócio.
- Priorize a segurança, evitando exposição de dados sensíveis e injeção de SQL.

5. Entrega
- Suba o código em um repositório público (GitHub/GitLab).
- Inclua um README com:
  - Instruções para rodar o projeto com Docker.
  - Explicação sobre a arquitetura escolhida.
  - Como executar os testes.
  - Envie o link do repositório para o email que entrou em contato com você.

Boa sorte e obrigado por participar do nosso processo seletivo.
