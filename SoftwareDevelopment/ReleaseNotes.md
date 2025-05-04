# Notas de Lançamento
Um changelog é um documento que lista, em ordem cronológica, todas as mudanças feitas em um projeto de software: correções de bugs, novas funcionalidades, melhorias e quebras de compatibilidade. Ele é essencial para:

- **Comunicação:** mantém time e usuários informados sobre o que mudou.
- **Rastreabilidade:** ajuda a entender quando e por que uma alteração foi feita.
- **Governança:** facilita auditoria, rollback e planejamento de releases.

## SemVer-tiered
Agrupa as entradas segundo os níveis do Semantic Versioning: Major, Minor e Patch.

- **Como funciona:** toda mudança é classificada conforme quebra de compatibilidade (major), novos recursos compatíveis (minor) ou correções/ajustes (patch).
- **Contexto ideal:** bibliotecas e APIs públicas que seguem rigorosamente o SemVer; equipes que desejam evidenciar o impacto de cada release.

## Conventional-style
Baseado em Conventional Commits (`feat`, `fix`, `chore`, `refactor` etc.), gera changelogs automaticamente por meio de ferramentas como semantic-release.

- **Como funciona:** cada commit segue um padrão (type(scope): subject); um script agrupa commits por tipo e monta o changelog.
- **Contexto ideal:** times que valorizam automação total de releases e têm disciplina para seguir o padrão de commits.

## Component-based
Separa entradas por módulos ou subsistemas do projeto (ex.: `UI`, `Backend`, `Banco`, `Integrações`).

- **Como funciona:** o changelog lista seções como `UI`, `API`, `DB`, e cada mudança é alocada na seção correspondente.
- **Contexto ideal:** monólitos modulares ou sistemas grandes em que cada equipe cuida de um componente diferente.

## Feature-based
Organiza o changelog em torno de funcionalidades entregues, em vez de níveis de versão.

- **Como funciona:** seções como `Novas Funcionalidades`, `Melhorias`, `Correções` ou focadas em features específicas.
- **Contexto ideal:** produtos orientados ao cliente final, onde importa destacar o que o usuário recebe em cada release.

## Category-based (Keep a Changelog)
Changelog organizado em categorias padronizadas como `Added`, `Changed`, `Deprecated`, `Removed`, `Fixed` e `Security`.

- **Como funciona:** cada seção do changelog recebe um cabeçalho de categoria; todas as mudanças são listadas sob o título correspondente.
- **Contexto ideal:** projetos que buscam clareza e consistência na comunicação das alterações, facilitando a leitura tanto para desenvolvedores quanto para usuários finais.

## Time-based
Changelog dividido por períodos de tempo em vez de versões ou tipos.

- **Como funciona:** agrupa todas as mudanças realizadas num intervalo definido (ex.: `Sprint 10 – Maio/2025` ou `Abril 2025`), listando-as em ordem cronológica dentro de cada seção temporal.
- **Contexto ideal:** equipes que trabalham em ciclos ágeis com entregas regulares (sprints, releases mensais, trimestres), onde o foco é o ritmo de entrega mais do que a classificação detalhada das alterações.

## Release Notes + Changelog híbrido
Combina notas de release detalhadas com um changelog enxuto para diferentes públicos.

- **Como funciona:** apresenta primeiro notas de release ricas (descrição de novas funcionalidades, instruções de migração, links para PRs, autores e até screenshots), seguidas de um changelog simplificado ou categorizado para referência rápida.
- **Contexto ideal:** produtos maduros que precisam oferecer documentação completa para usuários finais e, ao mesmo tempo, manter um histórico de mudanças objetivo para desenvolvedores e integradores.

## Flat
Lista simples, em ordem cronológica, sem subgrupos nem tags especiais.

- **Como funciona:** Contém apenas a data e a descrição da mudança, uma linha por item.
- **Contexto ideal:** projetos pequenos ou protótipos onde categorizar gera sobrecarga e é irrelevante.