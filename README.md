# RepoMentor

Encontre sua primeira contribuição open source com contexto, evidências e um caminho para começar.

**Status: Em desenvolvimento**

## A ideia

O RepoMentor ajudará desenvolvedores a compreender issues e a começar a contribuir com projetos open source. O MVP será dedicado a analisar documentação, estrutura do código e issues abertas para recomendar oportunidades e produzir um guia de contribuição.

O Gemma 4 explicará a arquitetura, avaliará a dificuldade das issues e sugerirá áreas para investigar. Cada recomendação deverá apresentar evidências e distinguir fatos de hipóteses. Caminhos sugeridos serão conferidos contra os arquivos coletados.

## Fluxo planejado

1. Consultar dados reais e issues abertas.
2. Selecionar documentação e arquivos relevantes, com limites de tamanho.
3. Enviar o contexto ao Gemma 4 no Google Cloud.
4. Validar a resposta e os caminhos citados.
5. Exibir recomendações e gerar um guia para a issue escolhida.

## Stack escolhida

| Camada | Tecnologia planejada |
| --- | --- |
| Interface | React, Vite, JavaScript/JSX e CSS |
| Backend | Python 3.12+, FastAPI, Pydantic e HTTPX |
| IA | Gemma 4 em endpoint próprio do Vertex AI, Google Cloud |
| Dados | GitHub REST API, somente leitura |
| Testes | Pytest, Vitest e React Testing Library |

A variante inicial candidata é Gemma 4 26B A4B. A seleção final depende de uma chamada real, qualidade, latência, região, quotas e orçamento. Modelo e endpoint serão configuráveis.

O processamento será em nuvem: o contexto público selecionado será enviado ao Google Cloud. Credenciais ficarão exclusivamente no backend.

## Escopo

O MVP inclui análise arquitetural, classificação explicada de issues, verificação de referências e guias de contribuição. Repositórios genéricos, login, execução de código, edição de arquivos e abertura automática de PRs ficam fora da primeira versão.

## Documentação

- [Plano de implementação e specs](docs/IMPLEMENTATION_PLAN.md)
- [Decisão Google Cloud + Gemma 4](docs/GOOGLE_CLOUD.md)
- [Plano de testes e aceite](docs/TEST_PLAN.md)
- [Registro de experimentos](docs/GEMMA_EXPERIMENTS.md)

## Próximas entregas

- [x] Criar a base documental do repositório.
- [x] Inicializar frontend e backend com endpoint de saúde.
- [x] Validar acesso ao Gemma 4 no Google Cloud.
- [x] Consultar issues e contexto reais: Respositorio Utilizado para teste - [Meteor](https://github.com/meteor/meteor)
- [x] Implementar análise com evidências e guia de contribuição.
- [x] Executar testes e revisar pelo menos três issues reais.
- [ ] Gravar demonstração e preparar a primeira release.

## Participação no evento

Hacktoberfest Hack Day São José dos Campos
A categoria pretendida é:  Best Use of Gemma 4

## Licença

[MIT](LICENSE). O projeto não é afiliado ao Google. Modelos, dependências e materiais consultados mantêm suas próprias licenças.

## Autores

- [Flora Rosa Pupo](https://github.com/FloraRosaPupo)
- [Daniel Dias](https://github.com/Danieldpereira)
- [Lucas Roberto](https://github.com/LucasR022)
- [Ana Claudia](https://github.com/anacnogueira)
