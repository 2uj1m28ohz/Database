# Performance

![](/DataBackup/Image.png)

> Data Corruption/David Camargo

No contexto de backup local de dados, garantir a performance e a segurança do armazenamento é essencial para proteger informações críticas contra perda ou corrupção. A escolha correta da tabela de partições, do sistema de arquivos e do tamanho da unidade de alocação desempenha um papel fundamental no desempenho e na integridade dos dados armazenados. Cada um desses elementos tem impacto direto na eficiência da utilização do espaço de armazenamento, na rapidez de acesso aos dados e na resiliência contra falhas. Compreender suas características e benefícios é crucial para selecionar as melhores opções de configuração para cada cenário de backup, maximizando tanto a proteção quanto o desempenho.

## Tabela de partição
Uma tabela de partição é uma estrutura de dados armazenada no início de um disco rígido ou outro meio de armazenamento que descreve a organização e a estrutura das partições no disco. A partição é uma divisão lógica de um disco físico que permite o gerenciamento separado de diferentes seções do disco. A tabela de partições informa ao sistema operacional como acessar e gerenciar os dados armazenados nessas divisões.

A escolha da tabela de partição adequada é essencial para garantir compatibilidade com diferentes sistemas operacionais e dispositivos, bem como para otimizar o uso do espaço de armazenamento, segurança, e desempenho do sistema.

### MBR
O Master Boot Record (MBR) é um dos formatos de tabela de partição mais antigos e amplamente utilizados, criado pela IBM em 1983 para sistemas DOS. A tabela MBR é armazenada no primeiro setor de um disco rígido, chamado de "setor de boot", e contém informações sobre a organização das partições no disco, além de um pequeno programa executável que ajuda a iniciar o sistema operacional.

O MBR oferece suporte para discos de até 2 TB e permite a criação de até 4 partições primárias. Se for necessário usar mais de 4 partições, uma delas pode ser configurada como uma partição estendida, que pode conter múltiplas partições lógicas. Isso proporciona flexibilidade em discos menores e é uma solução funcional para muitas configurações de hardware e software.

O MBR funciona em conjunto com o firmware BIOS (Basic Input/Output System), que é responsável por inicializar o hardware do computador e, em seguida, carregar o MBR para iniciar o sistema operacional. Essa combinação de MBR e BIOS é amplamente compatível com uma variedade de sistemas operacionais, especialmente os mais antigos, o que garante sua utilidade contínua em muitos ambientes de TI.

No entanto, o MBR tem algumas limitações inerentes ao seu design. O suporte para tamanhos de partição é limitado a 2 TB, e o número de partições primárias também é restrito a quatro. Além disso, todas as informações críticas de inicialização e partições são armazenadas em um único local, o que pode apresentar um risco em caso de falhas ou corrupção. Apesar dessas limitações, o MBR continua sendo uma escolha confiável e eficaz para muitos sistemas que não exigem grandes capacidades de armazenamento ou não utilizam recursos de firmware mais recentes.

### GPT
A GUID Partition Table (GPT) é um padrão mais moderno de tabela de partição, introduzido como parte da especificação do UEFI (Unified Extensible Firmware Interface) em 2000. O GPT foi criado para superar as limitações do MBR e oferece várias melhorias significativas. Diferente do MBR, o GPT utiliza um identificador único global (GUID) para cada partição, o que permite um número muito maior de partições primárias — até 128 no Windows, embora, teoricamente, o limite seja muito maior.

O GPT também é projetado para suportar discos muito maiores, com um tamanho máximo de partição de até 9.4 ZB (zettabytes), o que está muito além das necessidades de armazenamento atuais. Além disso, o GPT armazena várias cópias da tabela de partições em diferentes locais do disco, proporcionando maior resiliência contra corrupção de dados. Ele inclui verificações de integridade utilizando CRC (Cyclic Redundancy Check), permitindo a detecção e recuperação automática de erros na tabela de partições.

O GPT é projetado para trabalhar com o firmware UEFI, que substitui o BIOS tradicional. O UEFI lê a tabela de partições GPT diretamente, permitindo inicializações mais rápidas e suporte a discos de grande capacidade e com um grande número de partições. No entanto, o uso do GPT requer que o sistema tenha suporte ao UEFI, o que pode ser uma limitação para sistemas operacionais ou hardware mais antigos.

Para o contexto de backup de dados, a GPT é claramente a opção mais vantajosa. Ela permite o uso de discos maiores, suporta um número maior de partições, e oferece maior proteção contra falhas de dados e corrupção, fatores críticos em ambientes de backup. Além disso, a compatibilidade com o UEFI garante maior flexibilidade e longevidade em sistemas modernos. A menos que você precise garantir compatibilidade com sistemas muito antigos que não suportam UEFI, a escolha da GPT é recomendada para garantir a máxima eficiência e segurança dos dados de backup.

## Sistema de arquivos
Um sistema de arquivos é uma estrutura lógica utilizada por sistemas operacionais para controlar a forma como os dados são armazenados e recuperados em um dispositivo de armazenamento, como discos rígidos, SSDs, cartões SD, entre outros. Sua função é organizar dados em arquivos e diretórios, permitindo que o sistema operacional e os aplicativos leiam, gravem e modifiquem informações de maneira eficiente e segura.

Os sistemas de arquivos fornecem métodos para nomear arquivos, definir permissões de acesso e organizar dados de maneira que possam ser facilmente gerenciados e protegidos contra corrupção ou perda. Eles também são responsáveis por gerenciar o espaço de armazenamento, mantendo o controle sobre onde cada arquivo está fisicamente localizado no dispositivo, facilitando a alocação e a recuperação rápida dos dados.

### Windows
- FAT32 (File Allocation Table 32)
    - Ano de criação: 1996
    - Tamanho máximo da partição: 2 TB
    - Tamanho máximo do arquivo: 4 GB
    - Tecnologias suportadas: Alocação de espaço simplificada, compatibilidade com sistemas mais antigos e diversos dispositivos.
    - Problema resolvido: Compatibilidade ampla com sistemas operacionais e dispositivos mais antigos, tornando-o ideal para dispositivos removíveis.

- exFAT (Extended File Allocation Table)
    - Ano de criação: 2006
    - Tamanho máximo da partição: 128 PB (petabytes)
    - Tamanho máximo do arquivo: 16 EB (exabytes)
    - Tecnologias suportadas: Maior capacidade de arquivos e partições, otimizado para armazenamento removível, compatibilidade com dispositivos modernos como cartões SDXC.
    - Problema resolvido: Necessidade de suporte a grandes arquivos e partições em dispositivos removíveis, sem as limitações do FAT32.

- NTFS (New Technology File System)
    - Ano de criação: 1993
    - Tamanho máximo da partição: 256 TB
    - Tamanho máximo do arquivo: 16 TB (em sistemas de 64 bits)
    - Tecnologias suportadas: Journaling, ACL (Listas de Controle de Acesso), criptografia, compressão de arquivos, suporte a longos nomes de arquivos, cota de disco, e recuperação após falhas.
    - Problema resolvido: Segurança e integridade dos dados, suporte a grandes volumes e arquivos, além de melhor desempenho em sistemas modernos.

- ReFS (Resilient File System)
    - Ano de criação: 2012
    - Tamanho máximo da partição: 35 PB (petabytes)
    - Tamanho máximo do arquivo: Ilimitado, dentro do limite de volume.
    - Tecnologias suportadas: Detecção e correção automática de erros, integridade de dados, suporte a volumes grandes, criação de snapshots, otimização para cargas de trabalho de dados grandes.
    - Problema resolvido: Necessidade de maior resiliência e integridade de dados em ambientes de servidor e de armazenamento de alta capacidade, especialmente em sistemas com grandes volumes e cargas de trabalho intensivas.

### Linux
- EXT (Extended File System)
    - Ano de criação: 1992
    - Tamanho máximo da partição: 2 GB
    - Tamanho máximo do arquivo: 2 GB
    - Tecnologias suportadas: Estrutura básica para suporte ao sistema Unix-like.
    - Problema resolvido: Limitação de armazenamento e falta de um sistema de arquivos adequado para o Linux inicial.

- EXT2 (Second Extended File System)
    - Ano de criação: 1993
    - Tamanho máximo da partição: 32 TB
    - Tamanho máximo do arquivo: 2 TB
    - Tecnologias suportadas: Melhoria na alocação de espaço, maior capacidade de partição e arquivos.
    - Problema resolvido: Necessidade de maior capacidade de armazenamento e melhor gerenciamento de espaço em comparação com o EXT.

- EXT3 (Third Extended File System)
    - Ano de criação: 2001
    - Tamanho máximo da partição: 32 TB
    - Tamanho máximo do arquivo: 2 TB
    - Tecnologias suportadas: Journaling para recuperação de falhas.
    - Problema resolvido: Necessidade de recuperação rápida e segura de dados após falhas, com compatibilidade retroativa ao EXT2.

- EXT4 (Fourth Extended File System)
    - Ano de criação: 2008
    - Tamanho máximo da partição: 1 EB (exabyte)
    - Tamanho máximo do arquivo: 16 TB
    - Tecnologias suportadas: Journaling aprimorado, alocação retardada, suporte a volumes maiores, verificação de integridade.
    - Problema resolvido: Necessidade de maior performance, capacidade de armazenamento, e integridade de dados em sistemas Linux modernos.

### macOS
- HFS (Hierarchical File System)
    - Ano de criação: 1985
    - Tamanho máximo da partição: 2 GB
    - Tamanho máximo do arquivo: 2 GB
    - Tecnologias suportadas: Sistema de organização hierárquica, suporte básico a metadados.
    - Problema resolvido: Limitações do Macintosh File System (MFS) ao permitir maior capacidade de armazenamento e melhor organização de dados.

- HFS+ (Hierarchical File System Plus)
     - Ano de criação: 1998
     - Tamanho máximo da partição: 8 EB (exabytes)
     - Tamanho máximo do arquivo: 8 EB
     - Tecnologias suportadas: Unicode para nomes de arquivos, compatibilidade com volumes maiores, suporte a journaling, gerenciamento melhorado de espaço.
     - Problema resolvido: Limitação de capacidade de armazenamento e performance do HFS, adicionando maior robustez e suporte a nomes de arquivos complexos.

- APFS (Apple File System)
    - Ano de criação: 2017
    - Tamanho máximo da partição: 8 EB
    - Tamanho máximo do arquivo: 8 EB
    - Tecnologias suportadas: Suporte a SSDs e armazenamento flash, criptografia nativa, snapshots, clones, espaço dinâmico entre volumes.
    - Problema resolvido: Necessidade de um sistema de arquivos moderno e otimizado para SSDs, com melhor desempenho, segurança, e eficiência no uso de espaço.

Ao escolher um sistema de arquivos para o drive em que o backup será armazenado, é essencial considerar o sistema operacional em que os dados serão lidos, o volume de dados a ser armazenado e as tecnologias que o sistema de arquivos oferece para garantir a segurança e a integridade dos dados. A compatibilidade entre sistemas operacionais, o suporte a arquivos grandes, a criptografia, e a tolerância a falhas são fatores críticos que influenciam na escolha do sistema de arquivos ideal para cada cenário de backup.

## Unidade de alocação
A unidade de alocação, também chamada de cluster, é o menor bloco de espaço de armazenamento que um sistema de arquivos pode usar para gerenciar arquivos em um disco ou partição. Cada arquivo armazenado em um dispositivo é alocado em um ou mais clusters, e mesmo o menor arquivo ocupará pelo menos um cluster inteiro. A escolha do tamanho da unidade de alocação influencia diretamente o desempenho e a eficiência do armazenamento.

- **Influência no armazenamento:** O tamanho da unidade de alocação define como o espaço de armazenamento em um drive é organizado e usado. Um tamanho de cluster menor permite que o sistema de arquivos armazene dados de forma mais eficiente, pois minimiza o "espaço desperdiçado" dentro dos clusters. No entanto, com clusters menores, o sistema precisa gerenciar um número muito maior de unidades, o que pode aumentar a sobrecarga administrativa em discos grandes.

    Por outro lado, tamanhos de cluster maiores reduzem a quantidade de clusters que o sistema precisa gerenciar, o que é benéfico para drives de grande capacidade. Porém, isso pode resultar em desperdício de espaço, especialmente se o drive armazenar muitos arquivos pequenos, já que cada arquivo ocupa pelo menos um cluster inteiro, independentemente de seu tamanho.

- **Influência no desempenho:** O tamanho da unidade de alocação também impacta diretamente o desempenho das operações de entrada e saída (I/O). Clusters maiores tendem a melhorar o desempenho de I/O para arquivos grandes, pois menos operações são necessárias para ler ou escrever grandes blocos de dados em uma única operação. Isso é especialmente vantajoso em situações de leitura/gravação sequencial, como grandes transferências de arquivos.

    Por outro lado, clusters menores podem melhorar a eficiência do uso de espaço e o desempenho em operações de I/O envolvendo muitos arquivos pequenos, pois cada arquivo ocupa apenas o espaço estritamente necessário. No entanto, isso pode aumentar a fragmentação e a quantidade de operações de I/O necessárias para acessar dados espalhados por muitos clusters, afetando o desempenho em leituras/gravações aleatórias.

O tamanho da unidade de alocação afeta tanto o uso de espaço quanto o desempenho do armazenamento. A escolha ideal depende do perfil de uso do drive: clusters maiores beneficiam cargas de trabalho que envolvem arquivos grandes e operações sequenciais, enquanto clusters menores são preferíveis para cenários com muitos arquivos pequenos e operações de I/O aleatórias.

A performance e a segurança de backups dependem de diversas escolhas técnicas, como o tipo de tabela de partições, o sistema de arquivos e o tamanho da unidade de alocação. Decisões bem informadas nestes aspectos podem otimizar o uso de espaço, melhorar a velocidade de acesso aos dados e aumentar a resiliência contra falhas. Seja para backups corporativos em larga escala ou para soluções de armazenamento doméstico, essas considerações ajudam a garantir que os dados estejam sempre seguros, acessíveis e armazenados de maneira eficiente. Avaliar as necessidades específicas de cada cenário é a chave para selecionar a configuração ideal e assegurar uma estratégia de backup robusta e confiável.