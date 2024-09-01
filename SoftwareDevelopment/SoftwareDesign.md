## :desktop_computer: Design de Software

<img align="right" height="600px" src="https://github.com/2uj1m28ohz/Database/blob/main/SoftwareDevelopment/Image.png"/>

O design de software é o processo de conceber e planejar a estrutura, a arquitetura e os componentes de um sistema de software. Ele envolve tomar decisões sobre como os diferentes elementos do software serão organizados para atender aos requisitos funcionais e não funcionais do sistema. Esse processo inclui várias etapas:

- **Análise de requisitos:** Entender as necessidades do cliente e os requisitos do sistema é o primeiro passo. Isso envolve identificar funcionalidades, restrições, expectativas e escopo do projeto.

- **Arquitetura de software:** Definir a estrutura global do sistema, incluindo a identificação de componentes principais, suas interações, fluxos de dados e interfaces. Isso pode envolver a seleção de padrões de design, linguagens de programação, frameworks e tecnologias apropriadas.

- **Design detalhado:** Desenvolver o design detalhado de cada componente do sistema, considerando como eles se encaixam na arquitetura geral. Isso pode incluir a definição de classes, métodos, interfaces, banco de dados, APIs e outros elementos específicos do software.

- **Testabilidade e escalabilidade:** Considerar aspectos de testabilidade, como a capacidade de realizar testes unitários e de integração, bem como a escalabilidade do sistema para lidar com aumentos esperados de carga ou dados.

- **Padrões e boas práticas:** Aplicar padrões de design e boas práticas de engenharia de software para criar um sistema mais robusto, fácil de entender, manter e estender.

O design de software não se limita apenas à fase inicial do desenvolvimento; é um processo contínuo e iterativo à medida que o software é construído, testado e refinado. Ele visa criar sistemas que sejam funcionais, confiáveis, eficientes, de fácil manutenção e adaptação a mudanças futuras. Além disso, o design de software frequentemente aborda questões de arquitetura, segurança, usabilidade e desempenho para garantir que o produto final atenda às necessidades do cliente e aos padrões de qualidade estabelecidos.

<details>
<summary>Clean Code</summary>

Clean Code é um conceito que se refere à prática de escrever código de programação de forma clara, simples e legível. O código limpo é fácil de entender, manter e modificar, além de seguir boas práticas de design e ser de alta qualidade. Alguns princípios associados ao Clean Code incluem:

- Legibilidade: O código é escrito de maneira clara, com nomes significativos para variáveis, funções e classes, facilitando a compreensão do que o código faz.

- Simplicidade: Evita a complexidade desnecessária, mantendo as soluções simples e diretas.

- Organização: Divide o código em partes lógicas, como funções ou classes, para facilitar a compreensão e a manutenção.

- Comentários úteis: Os comentários são usados de forma parcimoniosa e apenas quando necessário para explicar o porquê de certas decisões ou soluções complexas.

- Testabilidade: É fácil escrever testes para o código, permitindo a verificação de seu funcionamento de maneira confiável.

- Manutenibilidade: O código é escrito de forma a facilitar alterações futuras sem introduzir problemas.

- Conformidade com padrões: Segue as convenções e padrões de codificação estabelecidos na linguagem ou na comunidade, o que torna o código mais consistente e compreensível para outros programadores.

- Baixo acoplamento e alta coesão: As partes do código são independentes umas das outras (baixo acoplamento) e têm uma funcionalidade clara e específica (alta coesão).

O Clean Code não se trata apenas de escrever código que funcione, mas sim de criar código que seja fácil de entender, manter e evoluir ao longo do tempo. Isso é essencial para equipes de desenvolvimento que precisam colaborar em projetos complexos, já que um código limpo reduz erros, melhora a produtividade e torna o processo de desenvolvimento mais eficiente.

</details>

<details>
<summary>Solid</summary>

SOLID é um acrônimo que representa cinco princípios de design de software que visam criar sistemas mais compreensíveis, flexíveis e fáceis de manter. Esses princípios foram introduzidos por Robert C. Martin, conhecido como Uncle Bob, e são considerados fundamentais para o desenvolvimento de software orientado a objetos. Os cinco princípios SOLID são:

- SRP - Single Responsibility Principle (Princípio da Responsabilidade Única): Este princípio afirma que uma classe deve ter apenas uma razão para mudar. Em outras palavras, uma classe deve ter uma única responsabilidade ou função bem definida no sistema. Isso ajuda a manter o código mais coeso, facilitando sua compreensão e manutenção.

- OCP - Open/Closed Principle (Princípio do Aberto/Fechado): Esse princípio preconiza que as entidades de software (classes, módulos, funções etc.) devem ser abertas para extensão, mas fechadas para modificação. Isso significa que o código deve ser projetado de forma que seja possível estender seu comportamento sem alterar o código-fonte original.

- LSP - Liskov Substitution Principle (Princípio da Substituição de Liskov): Esse princípio afirma que os objetos de uma classe derivada devem ser substituíveis por objetos de sua classe base sem afetar a integridade do programa. Em termos simples, isso significa que os objetos devem ser substituíveis por suas subclasses sem causar problemas no programa.

- ISP - Interface Segregation Principle (Princípio da Segregação de Interfaces): Esse princípio sugere que interfaces maiores e generalizadas devem ser divididas em interfaces menores e mais específicas, adaptadas às necessidades exatas do cliente. Isso evita a implementação de métodos não utilizados e reduz a dependência de classes a funcionalidades que não são relevantes para elas.

- DIP - Dependency Inversion Principle (Princípio da Inversão de Dependência): Esse princípio propõe que as classes de alto nível não devem depender de classes de baixo nível, mas sim de abstrações. Além disso, detalhes de implementação devem depender de abstrações, não o contrário. Isso promove a flexibilidade e a reutilização de código.

Os princípios SOLID são diretrizes poderosas para desenvolver software mais robusto, flexível e de fácil manutenção. Quando aplicados corretamente, ajudam a criar sistemas mais escaláveis, com código mais limpo e menos propenso a erros.

</details>

Clean Code e SOLID estão intimamente relacionados e se complementam no contexto do desenvolvimento de software de alta qualidade.

Clean Code se refere principalmente à legibilidade, manutenibilidade e facilidade de compreensão do código. Envolve práticas como usar nomes significativos para variáveis, funções e classes, escrever comentários úteis e organizar o código de maneira clara e lógica. Clean Code busca criar um código que seja fácil de ler, entender e manter.

SOLID, por outro lado, são cinco princípios de design que se concentram mais nas relações entre classes, na estruturação do código e na flexibilidade do sistema. SOLID busca criar um design de software que seja modular, flexível, fácil de estender e menos propenso a problemas quando novos recursos são adicionados ou alterações são feitas.

Diferença entre eles:

- Escopo: Clean Code se concentra principalmente na legibilidade e manutenção do código-fonte, enquanto SOLID trata mais especificamente do design de classes e da estruturação do código.

- Objetivos: Clean Code visa tornar o código mais legível, entendível e fácil de manter. SOLID, por sua vez, busca criar um design de software mais flexível, extensível e menos propenso a introduzir problemas ao fazer alterações.

- Abordagem: Clean Code inclui práticas gerais e diretrizes para escrever código mais limpo, enquanto SOLID são princípios específicos que orientam o design de software, especialmente em relação à orientação a objetos.

Clean Code e SOLID estão inter-relacionados no sentido de que ambos visam melhorar a qualidade do software, mas focam em aspectos diferentes: Clean Code nas práticas de codificação e legibilidade, e SOLID nos princípios de design que influenciam a estruturação e extensibilidade do sistema. Ambos são fundamentais para a criação de software de alta qualidade e são frequentemente aplicados em conjunto para obter sistemas robustos e fáceis de manter.

> Imagem: Martina Stiftinger/Google DeepMind