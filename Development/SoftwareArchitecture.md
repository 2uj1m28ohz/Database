## :arrow_right: Arquitetura de Software

<img align="right" height="600px" src="https://github.com/2uj1m28ohz/Database/blob/main/Development/SoftwareArchitecture.png"/>

A arquitetura de software lida com a estruturação e organização de sistemas de software. Ela envolve o design de grandes componentes estruturais, seus relacionamentos e como esses componentes interagem para formar um sistema completo.

Em termos simples, é como criar um plano ou uma planta baixa para a construção de um edifício, mas no contexto da criação de software. Isso inclui a definição de padrões, princípios, guidelines e convenções para garantir que o software seja eficiente, escalável, fácil de manter e atenda aos requisitos funcionais e não funcionais.

A arquitetura de software abrange decisões importantes, como escolha de tecnologias, organização de módulos, distribuição de tarefas, gerenciamento de dados, interfaces do usuário e como todas essas partes se integram para criar um sistema coeso e funcional.

Dentro da arquitetura de software, a classificação de uma aplicação como monolítica ou modular é uma maneira de descrever a estrutura ou o design geral do sistema. Ambas são abordagens arquiteturais que se enquadram dentro do campo mais amplo da arquitetura de software.

A arquitetura de software é um conceito abrangente que engloba diferentes estilos, padrões e abordagens para criar e organizar sistemas de software. Ela não se limita a uma única forma de desenvolver um sistema, mas sim inclui diversas estratégias e metodologias, como:

- **Arquitetura de Componentes:** Baseada na ideia de dividir o sistema em componentes independentes que podem ser desenvolvidos e mantidos separadamente.

- **Arquitetura em Camadas:** Separa o sistema em camadas distintas, como a camada de apresentação, lógica de negócios e acesso a dados, cada uma responsável por funções específicas.

- **Arquitetura Orientada a Serviços (SOA):** Utiliza serviços independentes que se comunicam por meio de uma rede para realizar funções de negócios.

- **Arquitetura de Microsserviços:** Similar à modularidade, onde o sistema é dividido em serviços pequenos e independentes que se comunicam entre si.

A arquitetura monolítica e a arquitetura modular são apenas duas maneiras específicas de estruturar um sistema de software dentro desse espectro mais amplo. Elas representam diferentes abordagens para lidar com a organização e interconexão dos componentes de um sistema, cada uma com suas próprias vantagens e desvantagens.

<details>
<summary>Arquitetura Monolítica</summary>

A arquitetura monolítica é um estilo de design de software onde todas as partes de uma aplicação estão interligadas e combinadas em um único programa. Aqui estão algumas características e vantagens dessa abordagem:

- Características da Arquitetura Monolítica:

    - Estrutura Única: Todo o código é desenvolvido, implantado e gerenciado como uma única unidade.

    - Integração Direta: Os componentes estão intimamente integrados, muitas vezes compartilhando o mesmo código-base, bibliotecas e recursos.

    - Implantação Simples: Por ser uma única unidade, a implantação da aplicação monolítica é mais simples e requer menos configuração.

    - Compartilhamento de Recursos: Componentes podem compartilhar recursos e memória diretamente, facilitando a comunicação entre eles.

- Vantagens da Arquitetura Monolítica:

    - Simplicidade de Desenvolvimento: Geralmente, é mais simples e rápido desenvolver uma aplicação monolítica, já que todos os componentes estão no mesmo código-base.

    - Facilidade de Implantação: A implantação é mais simples, já que toda a aplicação é empacotada e implantada de uma só vez.

    - Facilidade Inicial de Escalabilidade: Em estágios iniciais, quando a carga do sistema é baixa, é mais fácil escalar uma aplicação monolítica, pois normalmente requer menos configuração.

    - Menor Overhead de Comunicação: Como os componentes estão diretamente integrados, há menos overhead de comunicação entre eles em comparação com sistemas distribuídos.

No entanto, é importante notar que enquanto a arquitetura monolítica tem suas vantagens, também possui desafios significativos, especialmente quando a aplicação cresce e as demandas de escalabilidade e manutenção aumentam. Esses desafios levaram ao surgimento de outras abordagens, como arquiteturas baseadas em microsserviços e arquiteturas modulares, que visam resolver algumas das limitações das arquiteturas monolíticas em sistemas maiores e mais complexos.

</details>

<details>
<summary>Arquitetura Modular</summary>

A arquitetura modular é um estilo de design de software onde um sistema é dividido em módulos independentes, cada um responsável por funcionalidades específicas.

- Características da Arquitetura Modular:

    - Divisão em Módulos: O sistema é dividido em partes independentes, onde cada módulo possui uma função clara e bem definida.

    - Baixo Acoplamento: Os módulos são interconectados, mas têm dependências mínimas entre si, o que reduz o impacto das mudanças em um módulo sobre os outros.

    - Independência de Desenvolvimento: Cada módulo pode ser desenvolvido, testado e mantido separadamente, o que facilita a colaboração entre equipes e a reutilização de código.

    - Facilidade de Escalabilidade: A adição de novos recursos ou a expansão do sistema pode ser feita através da introdução de novos módulos, sem afetar diretamente o restante do sistema.

- Vantagens da Arquitetura Modular:
    
    - Manutenção Simplificada: É mais fácil manter e atualizar um sistema modular, já que as mudanças podem ser feitas em módulos específicos sem afetar o sistema inteiro.
    
    - Reutilização de Componentes: Os módulos podem ser reutilizados em diferentes partes do sistema ou em projetos diferentes, economizando tempo e esforço de desenvolvimento.
    
    - Escalabilidade Melhorada: A arquitetura modular facilita a escalabilidade, pois novos módulos podem ser adicionados para lidar com aumento de demanda ou novas funcionalidades.
    
    - Testabilidade Aprimorada: Como os módulos são independentes, é mais fácil testar cada parte separadamente, o que melhora a qualidade do software.

Embora a arquitetura modular ofereça várias vantagens, também requer um planejamento cuidadoso e uma abordagem rigorosa na definição de interfaces entre os módulos para garantir a comunicação adequada entre eles. Além disso, a gestão de dependências entre os módulos é essencial para garantir um sistema coeso e funcional.

</details>

Ambas as abordagens têm vantagens e desvantagens, e a escolha entre elas muitas vezes depende das necessidades específicas do projeto, dos requisitos de escalabilidade, manutenção e dos recursos disponíveis.

Dentro da arquitetura de software, entender e decidir qual dessas abordagens (ou outras) melhor se adequa ao projeto é parte fundamental do processo de design e desenvolvimento.

> Imagem: Milad Fakurian/Unsplash
