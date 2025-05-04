# Arquitetura de Software

![](/SoftwareDevelopment/Image.png)

> Binary Code/David Camargo

A arquitetura de software lida com a estruturação e organização de sistemas de software. Ela envolve o design de grandes componentes estruturais, seus relacionamentos e como esses componentes interagem para formar um sistema completo.

Em termos simples, é como criar um plano ou uma planta baixa para a construção de um edifício, mas no contexto da criação de software. Isso inclui a definição de padrões, princípios, guidelines e convenções para garantir que o software seja eficiente, escalável, fácil de manter e atenda aos requisitos funcionais e não funcionais.

A arquitetura de software abrange decisões importantes, como escolha de tecnologias, organização de módulos, distribuição de tarefas, gerenciamento de dados, interfaces do usuário e como todas essas partes se integram para criar um sistema coeso e funcional.

A arquitetura de software é um conceito abrangente que engloba diferentes estilos, padrões e abordagens para criar e organizar sistemas de software. Ela não se limita a uma única forma de desenvolver um sistema, mas sim inclui diversas estratégias e metodologias, como:

## Arquitetura Monolítica
Aplicação construída e entregue como uma única unidade, com todos os componentes interligados e compartilhando código-base e recursos.

- Características
    - Estrutura única: todo o código, deploy e gestão ocorrem em um só pacote.
    - Integração direta: componentes compartilham bibliotecas, memória e recursos.
    - Implantação simples: basta empacotar e subir uma única artefato.
    - Compartilhamento de recursos: comunicação interna sem chamadas de rede.

- Vantagens
    - Simplicidade de desenvolvimento: uma única base de código facilita a implementação inicial.
    - Facilidade de implantação: zero orquestração de múltiplos serviços.
    - Escalabilidade inicial simples: basta replicar a mesma aplicação em mais instâncias.
    - Menor overhead de comunicação: chamadas internas são mais rápidas que chamadas via rede.

## Arquitetura Modular
Sistema dividido em módulos independentes, cada um responsável por uma funcionalidade bem definida e isolada.

- Características
    - Divisão em módulos: cada parte tem responsabilidade clara e fronteiras definidas.
    - Baixo acoplamento: dependências mínimas entre módulos.
    - Independência de desenvolvimento: times podem trabalhar, testar e versionar cada módulo à parte.
    - Facilidade de escalabilidade: adiciona-se ou dimensiona-se módulos conforme a demanda.

- Vantagens
    - Manutenção simplificada: mudanças impactam apenas o módulo afetado.
    - Reutilização de componentes: módulos podem ser usados em outros projetos ou contextos.
    - Escalabilidade melhorada: escalonar módulos individuais em vez de toda a aplicação.
    - Testabilidade aprimorada: testes isolados garantem maior confiabilidade do sistema.

## Arquitetura em Camadas
Divisão do sistema em camadas hierárquicas (ex.: apresentação, negócio, persistência), cada uma só interage com a camada imediatamente abaixo.

- Características
    - Separação clara de responsabilidades por camada.
    - Comunicação unidirecional (camada superior chama a inferior).
    - Cada camada pode ter tecnologias e times distintos.

- Vantagens
    - Facilita manutenção e evolução isolada.
    - Testes concentrados em uma camada sem afetar as outras.
    - Organização previsível do fluxo de dados e dependências.

## Arquitetura Cliente-Servidor
Cliente (UI/aplicação leve) consome serviços de um servidor central que gerencia dados e lógica.

- Características
    - Papéis bem definidos: clientes consumindo APIs do servidor.
    - Estado centralizado no servidor.
    - Comunicação via rede (HTTP, TCP).

- Vantagens
    - Centralização de dados e segurança.
    - Escalabilidade vertical/horizontal do servidor sem mexer no cliente.
    - Atualização do servidor reflexiva em todos os clientes.

## Arquitetura Orientada a Serviços (SOA)
Sistema composto por serviços autônomos que expõem contratos (WSDL/REST) e falam por mensagens.

- Características
    - Serviços independentes com contratos bem definidos.
    - Interoperabilidade entre plataformas heterogêneas.
    - Uso de barramento de serviço ou ESB opcional.

- Vantagens
    - Reuso de serviços em múltiplos processos de negócio.
    - Governança e versionamento centralizados.
    - Integração facilitada com sistemas legados.

## Arquitetura de Microsserviços
Evolução de SOA com serviços menores, deploy independente e comunicação leve (REST/gRPC).

- Características
    - Cada microserviço faz uma única função.
    - Deploy, escalonamento e ciclo de vida independentes.
    - Conteinerização (Docker/Kubernetes) comum.

- Vantagens
    - Escalabilidade isolada por serviço.
    - Time-autonomia na escolha de linguagem e ferramenta.
    - Tolerância a falhas: isolamento de blast radius.

## Arquitetura Dirigida a Eventos
Componentes produzem e consomem eventos de forma assíncrona, desacoplando emissor e receptor.

- Características
    - Uso de filas ou brokers (Kafka, RabbitMQ).
    - Comunicação assíncrona e reativa.
    - Emissor não aguarda processamento do consumidor.

- Vantagens
    - Alta escalabilidade e throughput.
    - Facilita pipelines de dados e auditoria.
    - Flexibilidade na adição de novos consumidores.

## Microkernel (Plug-in)
Núcleo mínimo com funcionalidades básicas, estendido por plug-ins que implementam features extras.

- Características
    - Kernel leve e estável.
    - Extensões carregadas dinamicamente.
    - APIs de plug-in bem definidas.

- Vantagens
    - Sistema base enxuto e confiável.
    - Atualização de funcionalidades sem alterar o core.
    - Comunidade pode desenvolver plug-ins independentes.

## Space-Based Architecture
Distribui dados e processamento em um “data grid” em memória para lidar com picos de carga.

- Características
    - Grid distribuído de memória (In-Memory Data Grid).
    - Processadores e dados co-localizados.
    - Elimina ponto único de falha e gargalo de BD.

- Vantagens
    - Baixa latência de acesso a dados.
    - Escalabilidade horizontal elástica.
    - Resiliência a falhas de nós isolados.

## Peer-to-Peer (P2P)
Nós iguais na rede que atuam simultaneamente como cliente e servidor, compartilhando dados.

- Características
    - Arquitetura descentralizada.
    - Descoberta dinâmica de peers.
    - Replicação de dados entre nós.

- Vantagens
    - Sem ponto único de falha.
    - Escalabilidade natural conforme entram mais peers.
    - Resiliência e distribuição de carga.

## Serverless/FaaS
Funções independentes que rodam sob demanda em nuvem, sem preocupação de servidores.

- Características
    - Código executado apenas quando estimulado (por evento).
    - Estateless e de curta duração.
    - Gerenciamento de infra feito pelo provedor.

- Vantagens
    - Zero gestão de servidores/instras.
    - Custo baseado em execução real (“pay-per-use”).
    - Time-to-market rápido para pequenas funcionalidades.

## Arquitetura Hexagonal (Ports & Adapters)
Core de domínio isolado de interfaces externas por “portas” e “adaptadores”.

- Características
    - Núcleo agnóstico a detalhes de infra.
    - Portas definem interfaces de entrada/saída.
    - Adaptadores concretizam integração (DB, UI, APIs).

- Vantagens
    - Testes de domínio sem mocks complexos.
    - Troca de tecnologias de infra sem mexer no core.
    - Design mais robusto e modular.

## CQRS + Event Sourcing
Separa modelo de escrita (Commands) do de leitura (Queries) e persiste estado como eventos imutáveis.

- Características
    - Dois modelos de dados: um para escrita, outro para leitura.
    - Store de eventos registra toda mudança de estado.
    - Reconstrução de estado via replay de eventos.

- Vantagens
    - Histórico completo e auditável.
    - Escalonamento de consultas sem impactar escrita.
    - Flexibilidade para recriar visões de dados.

## Clean Architecture/Onion/DDD
Organização em camadas concêntricas, com o domínio no centro e dependências apontando para dentro.

- Características
    - Domínio puro no núcleo, sem dependência de frameworks.
    - Camadas externas lidam com UI, infra e frameworks.
    - Inversão de controle e dependência para o núcleo.

- Vantagens
    - Alto isolamento do domínio e regras de negócio.
    - Fácil teste de unidades de negócio.
    - Evolução tecnológica sem afetar o core.