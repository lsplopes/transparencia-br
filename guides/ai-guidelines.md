# AI Guidelines

## 1. Contexto
Este projeto cria uma plataforma de transparência política, incluindo:
- Ingestão de dados de APIs públicas brasileiras.
- Enriquecimento de dados com IA.
- Front-end para visualização e interação com eleitores.

## 2. Padrões de Código
- **Linguagem principal**: TypeScript 5 (Node 20, ESM).
- **Paradigma**: Programação funcional leve, priorizando imutabilidade quando aplicável.
- **Linter**: ESLint com Airbnb-base e import/order.
- **Testes**: Jest com cobertura de 100% para linhas e ramos críticos.

## 3. Contribuições geradas por IA
- Todas as respostas devem incluir _comentários de contexto_ explicando as decisões tomadas.
- Evitar o uso de `any`; sempre utilizar tipagem explícita.
- Funções devem ter no máximo 50 linhas; helpers devem ser extraídos quando necessário.
- Cada export público deve ser acompanhado de testes adequados.

## 4. Estrutura dos Commits
- Seguir o padrão convencional:
  - `feat`: Adicionar novas funcionalidades.
  - `fix`: Corrigir bugs.
  - `chore`: Tarefas de manutenção.
  - `test`: Adicionar ou corrigir testes.
  - `docs`: Atualizar documentação.
- Exemplos:
  - `feat(etl): add job to fetch senate votes`
  - `fix(api): correct ISO date serialization`

## 5. Segurança e Ética
- Não armazenar dados pessoais sensíveis.
- Respeitar os limites de uso (rate limit) e os Termos de Serviço (ToS) de APIs externas.

## 6. Ferramentas de IA
- Sempre gerar comentários explicativos para o código gerado.
- Garantir cobertura de testes para todo export público.

## 7. Padrões de Formatação
- **Formatador**: Prettier obrigatório.
- **Estilo de código**: Funções com no máximo 50 linhas.
- **Configuração**: ESLint e Prettier devem ser integrados para evitar conflitos.
