# Design de Software

![](/SoftwareDevelopment/Image.png)

> Binary Code/David Camargo

O design de software é o processo de conceber e planejar a estrutura, a arquitetura e os componentes de um sistema de software. Ele envolve tomar decisões sobre como os diferentes elementos do software serão organizados para atender aos requisitos funcionais e não funcionais do sistema. Esse processo inclui várias etapas:

- **Análise de requisitos:** Entender as necessidades do cliente e os requisitos do sistema é o primeiro passo. Isso envolve identificar funcionalidades, restrições, expectativas e escopo do projeto.
- **Arquitetura de software:** Definir a estrutura global do sistema, incluindo a identificação de componentes principais, suas interações, fluxos de dados e interfaces. Isso pode envolver a seleção de padrões de design, linguagens de programação, frameworks e tecnologias apropriadas.
- **Design detalhado:** Desenvolver o design detalhado de cada componente do sistema, considerando como eles se encaixam na arquitetura geral. Isso pode incluir a definição de classes, métodos, interfaces, banco de dados, APIs e outros elementos específicos do software.
- **Testabilidade e escalabilidade:** Considerar aspectos de testabilidade, como a capacidade de realizar testes unitários e de integração, bem como a escalabilidade do sistema para lidar com aumentos esperados de carga ou dados.
- **Padrões e boas práticas:** Aplicar padrões de design e boas práticas de engenharia de software para criar um sistema mais robusto, fácil de entender, manter e estender.

O design de software não se limita apenas à fase inicial do desenvolvimento; é um processo contínuo e iterativo à medida que o software é construído, testado e refinado. Ele visa criar sistemas que sejam funcionais, confiáveis, eficientes, de fácil manutenção e adaptação a mudanças futuras. Além disso, o design de software frequentemente aborda questões de arquitetura, segurança, usabilidade e desempenho para garantir que o produto final atenda às necessidades do cliente e aos padrões de qualidade estabelecidos.

## Design Patterns
Padrões de projeto são soluções reutilizáveis para problemas recorrentes de design de software. Eles descrevem estruturas e interações entre classes e objetos de forma genérica, permitindo adaptar boas práticas a diferentes contextos.

- **Padrões de Criação (Creational):** abstratificam e encapsulam o processo de instanciar objetos. Exemplos: Singleton, Factory Method, Abstract Factory, Builder, Prototype.
- **Padrões Estruturais (Structural):** organizam como classes e objetos se combinam para formar estruturas maiores. Exemplos: Adapter, Decorator, Facade, Composite, Bridge.
- **Padrões Comportamentais (Behavioral):** definem a forma de comunicação e responsabilidade entre objetos. Exemplos: Observer, Strategy, Command, State, Template Method.

## SOLID
Conjunto de cinco princípios de design orientado a objetos que garantem sistemas mais flexíveis, extensíveis e fáceis de manter.

- **SRP (Single Responsibility):** cada classe tem uma única razão para mudar.
- **OCP (Open/Closed):** entidades abertas para extensão, fechadas para modificação.
- **LSP (Liskov Substitution):** subclasses devem ser substituíveis pelas superclasses sem quebrar o sistema.
- **ISP (Interface Segregation):** interfaces específicas em vez de genéricas, evitando métodos não usados.
- **DIP (Dependency Inversion):** depende-se de abstrações, não de implementações concretas.

## Manifesto Ágil
O Manifesto Ágil, criado em 2001 por 17 desenvolvedores, estabelece quatro valores centrais e 12 princípios que guiam a prática de desenvolvimento de software de forma flexível e colaborativa.

- Valores
    - Indivíduos e interações mais que processos e ferramentas.
    - Software funcionando mais que documentação abrangente.
    - Colaboração com o cliente mais que negociação de contratos.
    - Responder a mudanças mais que seguir um plano.

- Princípios
    - Satisfazer o cliente através da entrega contínua e antecipada de software de valor.
    - Aceitar mudanças de requisitos, mesmo tardiamente no desenvolvimento, para vantagem competitiva do cliente.
    - Entregar software funcionando com frequência, preferencialmente em ciclos curtos (semanas a meses).
    - Pessoas de negócio e desenvolvedores devem trabalhar juntas diariamente ao longo do projeto.
    - Construir projetos em torno de indivíduos motivados; dar ambiente, apoio e confiar neles para fazer o trabalho.
    - A forma mais eficiente e eficaz de transmitir informações é a comunicação face a face.
    - Software funcionando é a medida primária de progresso.
    - Processos ágeis promovem desenvolvimento sustentável; patrocinadores, desenvolvedores e usuários devem manter ritmo constante indefinidamente.
    - Atenção contínua à excelência técnica e bom design aumenta a agilidade.
    - Simplicidade é essencial.
    - As melhores arquiteturas, requisitos e designs emergem de equipes auto-organizadas.
    - Em intervalos regulares, a equipe reflete sobre como se tornar mais eficaz e ajusta seu comportamento de acordo.

## Domain-Driven Design (DDD)
Abordagem de desenvolvimento que coloca o domínio de negócio no centro, criando um modelo rico e alinhado às regras e linguagens dos especialistas.

- **Ubiquitous Language:** vocabulário comum usado em código e comunicação.
- **Bounded Contexts:** contextos bem definidos com seus próprios modelos e limites.
- **Entidades e Value Objects:** distinção entre objetos com identidade e objetos imutáveis.
- **Aggregates:** agrupamentos de entidades/value objects que garantem consistência transacional.
- **Repositories:** abstrações para persistência, isolando detalhes de infra.
- **Domain Services & Domain Events:** lógica de domínio fora de entidades e eventos que registram ocorrências relevantes.

## Clean Code
Prática de escrever código claro, simples e legível, seguindo boas práticas para facilitar entendimento e manutenção.

- **Legibilidade:** nomes significativos para variáveis, funções e classes.
- **Simplicidade:** evita complexidade desnecessária, soluções diretas.
- **Organização:** divide o código em funções ou classes com responsabilidade única.
- **Comentários úteis:** usados apenas para explicar decisões não óbvias.
- **Testabilidade:** facilita a criação de testes unitários e de integração.
- **Baixo acoplamento e alta coesão:** partes independentes com foco em responsabilidades claras.
- **Conformidade com padrões:** segue convenções da linguagem/comunidade.

## Object Calisthenics
Conjunto de nove regras de Jeff Bay para exercitar a disciplina de escrever código mais limpo e focado em objetos.

- **Regra 1 – Um nível de indentação por método:** evita aninhamentos profundos.
- **Regra 2 – Encapsular todo primitivo ou string:** promove Value Objects.
- **Regra 3 – Coleções de primeira classe:** use classes para representar grupos de objetos.
- **Regra 4 – Uma chamada (.) por linha:** obedece ao princípio de Demeter.
- **Regra 5 – Não abreviar nomes:** privilégia clareza e semântica.
- **Regra 6 – Manter classes pequenas:** menos de 50 linhas é uma boa métrica.
- **Regra 7 – Sem getters/setters expostos:** favorece comportamento sobre dados.
- **Regra 8 – Evitar métodos estáticos:** reduz acoplamento global.
- **Regra 9 – Transições de estado em vez de setters:** modela mudanças de forma explícita.

## Desenvolvimento Orientado por Testes (TDD)
TDD é uma abordagem que inverte o fluxo tradicional de desenvolvimento: você escreve primeiro um teste que falha e, só então, implementa o código mínimo para fazê-lo passar, seguindo o ciclo `Red` `>` `Green` `>` `Refactor`. Isso garante que todo código seja validado desde o início e que o design emerja organicamente a partir dos próprios testes.

- Ciclo Red/Green/Refactor
    - **Red:** escreva um teste para uma nova funcionalidade; ele deve falhar inicialmente.
    - **Green:** implemente o menor trecho de código que faça o teste passar.
    - **Refactor:** limpe e melhore o código, mantendo todos os testes verdes.

- Por que adotar o TDD
    - **Design guiado por testes:** o próprio conjunto de testes define APIs claras e responsabilidades bem delimitadas.
    - **Feedback imediato:** regressões e erros são detectados assim que aparecem.
    - **Documentação viva:** a suíte de testes serve como especificação do comportamento esperado.
    - **Confiança para refatorar:** com todos os testes passando, você pode reestruturar sem medo de quebrar algo.
    - **Código mais modular e testável:** como você só escreve o mínimo necessário para cada teste, o sistema tende a ficar mais desacoplado.