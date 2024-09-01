## :shield: Estratégias

<img align="right" height="600px" src="https://github.com/2uj1m28ohz/Database/blob/main/DataBackup/Image.png"/>

A adoção de estratégias robustas na rotina de backup é crucial para a proteção e a continuidade dos negócios em um cenário onde a perda de dados pode ter consequências devastadoras. Com o aumento da complexidade dos sistemas de TI e o volume de dados gerados diariamente, a simples execução de backups não é mais suficiente. É necessário implementar uma estratégia abrangente que garanta a integridade, disponibilidade e segurança dos dados.

Uma estratégia de backup eficaz vai além de criar cópias dos dados. Ela envolve a criação de um plano estruturado que considere fatores como frequência, locais de armazenamento, métodos de recuperação e auditorias regulares. A adoção de uma abordagem estratégica ajuda a assegurar que os backups não apenas existam, mas que também sejam recuperáveis em cenários de desastre. Sem uma estratégia robusta, as organizações correm o risco de enfrentar interrupções significativas, perda de produtividade e danos irreparáveis à sua reputação.

As tecnologias emergentes desempenham um papel cada vez mais importante na definição de estratégias de backup modernas. Soluções baseadas em nuvem, backup como serviço (BaaS), inteligência artificial e automação são exemplos de tecnologias que estão transformando a maneira como as organizações abordam o backup de dados. A adoção dessas inovações permite maior flexibilidade, escalabilidade e eficiência, além de fornecer proteção aprimorada contra ameaças cibernéticas e falhas de hardware. A integração de novas tecnologias na estratégia de backup não só melhora a proteção dos dados, mas também reduz os custos operacionais e o tempo de recuperação.

<details>
<summary>Estratégia 3-2-1</summary>

A estratégia 3-2-1 é uma das abordagens mais recomendadas para garantir a segurança e a disponibilidade dos dados. Ela preconiza que se mantenham três cópias dos dados, em dois tipos diferentes de mídia, sendo uma cópia armazenada fora do local principal.

- 3: Mantenha três cópias dos dados (o original e duas cópias de backup).
- 2: Armazene as cópias de backup em dois tipos diferentes de mídia (por exemplo, discos rígidos e fitas, ou armazenamento local e na nuvem).
- 1: Garanta que pelo menos uma dessas cópias esteja fora do local principal, protegida contra desastres que possam afetar fisicamente o ambiente de produção.

Essa estratégia oferece uma combinação de resiliência e acessibilidade, assegurando que os dados possam ser recuperados mesmo em casos de falhas de hardware ou desastres locais. Ela é simples de implementar e se adapta bem a diferentes ambientes e tamanhos de organizações.

</details>

<details>
<summary>Estratégia 3-1-2</summary>

A estratégia 3-1-2 é uma variação da 3-2-1, que enfatiza a importância de ter uma segunda cópia de backup armazenada fora do local principal, mas com uma abordagem mais rígida sobre a localização dos backups.

- 3: Três cópias dos dados são mantidas.
- 1: Uma cópia está em um local físico diferente, sem a necessidade de um segundo tipo de mídia.
- 2: As outras duas cópias são armazenadas em um local separado, possivelmente em um ambiente de nuvem com backup em diferentes data centers.

Essa estratégia aumenta a resiliência ao garantir que uma cópia dos dados esteja sempre em um local seguro e distante do ambiente de produção, mitigando riscos relacionados a desastres naturais ou falhas físicas. É especialmente útil para organizações que precisam de maior segurança geográfica sem a complexidade de múltiplos tipos de mídia.

</details>

<details>
<summary>Estratégia 3-2-2</summary>

A estratégia 3-2-2 é semelhante à 3-2-1, mas acrescenta uma camada adicional de segurança ao ter duas cópias externas dos dados, garantindo maior proteção contra perdas catastróficas.

- 3: Três cópias dos dados são mantidas.
- 2: As cópias são armazenadas em dois tipos diferentes de mídia.
- 2: Duas dessas cópias estão fora do local principal.

Ao duplicar as cópias externas, a estratégia 3-2-2 oferece um nível superior de segurança, assegurando que mesmo que uma cópia remota seja comprometida, outra estará disponível. É uma escolha excelente para ambientes críticos onde a continuidade do negócio depende da recuperação rápida e segura dos dados.

</details>

<details>
<summary>Estratégia 3-2-3</summary>

A estratégia 3-2-3 leva o conceito da 3-2-2 um passo adiante, aumentando ainda mais a redundância externa para máxima segurança.

- 3: Mantenha três cópias dos dados.
- 2: Armazene essas cópias em dois tipos diferentes de mídia.
- 3: Três cópias são mantidas fora do local principal.

Essa estratégia é ideal para organizações que necessitam de um nível extremamente elevado de resiliência e segurança dos dados. Com três cópias externas, os dados estão protegidos contra praticamente qualquer tipo de perda catastrófica, incluindo desastres naturais e ataques cibernéticos coordenados em múltiplas localizações.

</details>

<details>
<summary>Estratégia 3-2-1-1</summary>

A estratégia 3-2-1-1 adiciona uma camada extra de segurança ao modelo 3-2-1, garantindo que uma das cópias externas dos dados esteja offline ou em uma mídia com proteção extra, como criptografia ou um "air gap".

- 3: Três cópias dos dados são mantidas.
- 2: Armazene essas cópias em dois tipos diferentes de mídia.
- 1: Uma cópia está fora do local principal.
- 1: Uma cópia adicional está offline ou protegida por um air gap.

Esse modelo fortalece a segurança contra ataques cibernéticos, incluindo ransomwares, que podem comprometer sistemas conectados. A cópia offline ou com proteção extra garante que, mesmo em um cenário de comprometimento grave, uma versão dos dados estará segura e recuperável.

</details>

<details>
<summary>Estratégia 3-2-1-1-0</summary>

A estratégia 3-2-1-1-0 é a evolução mais abrangente do modelo 3-2-1, adicionando a exigência de que todas as cópias dos dados sejam verificadas regularmente para assegurar a integridade.

- 3: Mantenha três cópias dos dados.
- 2: Armazene essas cópias em dois tipos diferentes de mídia.
- 1: Uma cópia está fora do local principal.
- 1: Uma cópia adicional está offline ou protegida por um air gap.
- 0: Zero erros devem estar presentes nas cópias de backup, assegurando que todas as cópias são verificadas e estão íntegras.

Essa estratégia não só protege os dados contra uma ampla gama de ameaças e falhas, mas também garante que as cópias de backup são confiáveis e prontas para serem usadas em um momento de necessidade. A verificação contínua das cópias de backup é um diferencial importante, garantindo que os dados são consistentes e livres de corrupção.

</details>

A ausência de uma estratégia de backup bem planejada expõe as organizações a uma série de riscos. A perda total ou parcial de dados pode ocorrer devido a falhas de hardware, ataques cibernéticos, erros humanos ou desastres naturais. Sem uma estratégia robusta, a recuperação pode ser impossível ou extremamente demorada, resultando em perda financeira, penalidades legais e danos à imagem da empresa. Além disso, a falta de uma abordagem estratégica pode levar a backups inconsistentes, corruptos ou inacessíveis no momento crítico de recuperação. Esses riscos destacam a importância de investir tempo e recursos na criação e manutenção de uma estratégia de backup sólida e eficiente.

> Imagem: Rose Pilkington/Google DeepMind