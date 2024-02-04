## :arrow_right: Versionamento de Software

<img align="right" height="600px" src="https://github.com/2uj1m28ohz/Database/blob/main/Development/SoftwareVersioning.png"/>

O versionamento de software é o processo de controlar e gerenciar diferentes versões de um programa ou sistema ao longo do tempo. Ele é essencial para acompanhar e registrar as mudanças feitas no código-fonte e nos arquivos de um software, permitindo que os desenvolvedores trabalhem colaborativamente, acompanhem as alterações feitas, revertam para versões anteriores, e garantam a integridade e a evolução do projeto.

Existem sistemas de controle de versão, como o Git, Subversion, Mercurial, entre outros, que facilitam o versionamento, permitindo que equipes de desenvolvimento trabalhem simultaneamente em um código, gerenciem conflitos e preservem um histórico detalhado de todas as alterações realizadas. Esses sistemas ajudam a rastrear quem fez quais alterações, quando foram feitas e fornecem mecanismos para mesclar diferentes versões de código de maneira eficiente.

Alguns dos principais sistemas de controle de versão são:

- **Git:** É um dos sistemas mais populares. Ele é distribuído e foi projetado para lidar com projetos grandes e pequenos com eficiência. O Git é conhecido pela sua velocidade, flexibilidade e pelo suporte a fluxos de trabalho variados, como ramificação e mesclagem.

- **Subversion (SVN):** Um sistema de controle de versão centralizado, no qual todos os arquivos e históricos são armazenados em um único local central. Ele é mais linear em comparação com o Git, o que pode simplificar a compreensão do histórico de alterações.

- **Mercurial:** Similar ao Git em muitos aspectos, é distribuído e focado na facilidade de uso. Ele oferece muitos recursos similares ao Git, mas com diferenças na forma como algumas operações são executadas.

- **Perforce:** Um sistema de controle de versão que se destaca por sua capacidade de lidar com grandes volumes de dados e arquivos binários, comumente usado em grandes empresas e na indústria de jogos.

- **Team Foundation Version Control (TFVC):** Desenvolvido pela Microsoft, é uma opção centralizada similar ao SVN que integra-se bem ao ecossistema de desenvolvimento do Visual Studio e outros produtos da Microsoft.

<details>
<summary>Semantic Versioning</summary>

O Semantic Versioning (SemVer) é um sistema padronizado para numerar as versões de um software, permitindo uma compreensão clara e consistente das mudanças feitas em uma aplicação.

- Formato do Semantic Versioning: MAJOR.MINOR.PATCH

    - MAJOR: Incrementa para mudanças incompatíveis na API.

    - MINOR: Incrementa para adições compatíveis à funcionalidade.

    - PATCH: Incrementa para correções de bugs compatíveis.


O SemVer também permite o uso de etiquetas de pré-lançamento e metadados de construção para versões em desenvolvimento que ainda não são definitivas.

- Características do Semantic Versioning:

    - Clareza e Precisão: Fornece um esquema claro para entender o impacto das mudanças em cada versão.

    - Semântica Direta: O número de versão reflete as alterações e seu impacto no software.

    - Compatibilidade: Ajuda a identificar rapidamente se uma atualização pode ou não quebrar a compatibilidade com versões anteriores.

    - Padronização: É amplamente adotado e compreendido pela comunidade de desenvolvedores, facilitando a integração e a colaboração em projetos.

- Vantagens do Semantic Versioning:

    - Compreensão Rápida: Os números de versão fornecem informações imediatas sobre as mudanças realizadas.

    - Gerenciamento de Risco: Permite aos usuários decidir se devem ou não atualizar, com base nas mudanças anunciadas.

    - Integração Simplificada: Facilita a integração de bibliotecas e dependências, evitando conflitos e incompatibilidades.

    - Transparência para os Usuários: Os desenvolvedores podem comunicar facilmente o que mudou em cada versão para os usuários finais.

O Semantic Versioning é um sistema robusto e amplamente adotado que ajuda os desenvolvedores a entenderem e comunicarem melhor as mudanças em seus softwares, facilitando a vida tanto dos criadores quanto dos usuários finais.

</details>

<details>
<summary>Calendar Versioning</summary>

O Calendar Versioning (CalVer) é um sistema de versionamento que utiliza datas como base para numerar as versões de um software, trazendo uma abordagem temporal para indicar quando uma versão foi lançada.

- Formato do Calendar Versioning: YYYY.MM.DD ou YYYY.MM (ou variantes semelhantes)

    - Ano (YYYY): Refere-se ao ano do lançamento.

    - Mês (MM): Refere-se ao mês do lançamento.

    - Dia (DD): Refere-se ao dia do lançamento, opcionalmente incluído.

O CalVer também pode incluir letras, rótulos ou outras informações para indicar estágios de desenvolvimento, como alfa, beta, etc., agregando informações além da data de lançamento.

- Características do Calendar Versioning:

    - Ênfase na Temporalidade: Utiliza datas para numerar versões, proporcionando uma representação direta da cronologia dos lançamentos.

    - Simplicidade Conceitual: É fácil compreender a ordem cronológica das versões com base nas datas.

- Vantagens do Calendar Versioning:

    - Visibilidade Temporal: Permite aos usuários entender facilmente a cronologia dos lançamentos e atualizações.

    - Clareza na Ordem das Versões: A data indica claramente quando uma versão foi lançada, tornando mais simples a compreensão de quais versões são mais recentes.

    - Fácil de Acompanhar: Usar datas como versões facilita a identificação de quão atualizado está um software.

O Calendar Versioning, ao contrário do Semantic Versioning, enfoca mais a temporalidade do que as mudanças específicas realizadas em uma versão. Isso pode ser útil em contextos nos quais a data de lançamento é fundamental para os usuários ou quando se deseja destacar claramente a ordem cronológica das versões.

</details>

> Imagem: Mohammad Amin/Unsplash
