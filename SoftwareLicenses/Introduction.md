# `/` Introdução

![](/SoftwareLicenses/Image.png)

`>` `The Law/David Camargo`

Licenças de software são documentos legais que estabelecem os termos e condições sob os quais um software pode ser utilizado, modificado e distribuído. Elas desempenham um papel crucial na definição dos direitos e deveres dos desenvolvedores e usuários, oferecendo um equilíbrio entre a proteção dos direitos autorais e a liberdade de uso.

As licenças de software são essenciais porque:
- **Protegem a propriedade intelectual:** Elas garantem que o autor mantenha certos direitos sobre o software, mesmo ao permitir que outros o utilizem.
- **Definem direitos e deveres:** Especificam o que os usuários podem ou não fazer com o software, como copiar, modificar ou redistribuir.
- **Facilitam a colaboração:** Em projetos open source, uma licença bem escolhida promove contribuições ao deixar claro como o código pode ser reutilizado e compartilhado.

## `-` Software Livre e Código Aberto
- Definição de Software Livre:

    O conceito de Software Livre foi inicialmente promovido pela [Free Software Foundation](https://www.fsf.org) (FSF). Para ser considerado "livre", o software deve garantir quatro liberdades essenciais aos seus usuários:

    - **Liberdade 0:** Executar o software para qualquer propósito.
    - **Liberdade 1:** Estudar como o software funciona e adaptá-lo às suas necessidades.
    - **Liberdade 2:** Redistribuir cópias do software.
    - **Liberdade 3:** Melhorar o software e distribuir essas melhorias para o público.

    A filosofia do Software Livre é centrada na ideia de que os usuários devem ter controle total sobre o software que utilizam, promovendo a colaboração e a transparência.

- Definição de Open Source:

    - O termo "Open Source" foi cunhado pela [Open Source Initiative](https://opensource.org) (OSI) como uma forma de tornar a ideia de software de código aberto mais aceitável para o mundo corporativo. Enquanto ambos os conceitos defendem o acesso ao código-fonte, o Open Source tende a focar mais nos benefícios práticos, como a inovação, a qualidade do código e a segurança.
    - A OSI mantém a Open Source Definition, que descreve critérios que uma licença deve cumprir para ser considerada "Open Source", como a livre redistribuição e a inclusão do código-fonte.

### `+`  Open Source e Código Aberto
Embora "Open Source" e "Código Aberto" sejam tecnicamente sinônimos, o termo "Open Source" é amplamente utilizado em todo o mundo, inclusive em países de língua portuguesa, devido ao impacto global do movimento. A tradução literal "Código Aberto" não é tão comum em materiais e discussões técnicas, especialmente no Brasil, onde "Open Source" é mais reconhecido e adotado por desenvolvedores e empresas. Além disso, "Open Source" carrega consigo todo o contexto histórico e cultural do movimento que o termo "Código Aberto" às vezes não reflete completamente.

## `-` Copyleft e copyright
O copyleft é um conceito fundamental no movimento de Software Livre, criado como uma forma de garantir que o software mantenha suas liberdades originais ao longo do tempo. Em sua essência, copyleft é uma prática jurídica que usa as leis de copyright (direitos autorais) para garantir que todas as modificações ou redistribuições de um software continuem sendo livres, no sentido das quatro liberdades definidas pela Free Software Foundation.

Enquanto o copyright tradicional concede ao autor o direito exclusivo de controlar como sua obra é usada, o copyleft inverte essa lógica: ele permite o uso livre do software, mas impõe uma condição importante — qualquer trabalho derivado também deve ser distribuído sob os mesmos termos da licença original. Ou seja, o copyleft impede que alguém pegue um software livre, faça modificações e o torne proprietário ou restrito.

### `+` Como funciona o copyleft?
- **Baseado no copyright:** Apesar de parecer o oposto, o copyleft depende do sistema de copyright. Ao invés de remover todos os direitos do autor, ele usa as regras do copyright para impor a obrigatoriedade de que as liberdades sejam preservadas.
- **Imposição de condições:** Um software com uma licença copyleft, como a GPL (General Public License), permite que qualquer pessoa copie, modifique e redistribua o software, mas exige que quaisquer trabalhos derivados sejam licenciados sob os mesmos termos. Isso significa que as liberdades originais (como estudar, modificar e redistribuir o código) devem ser mantidas em todos os futuros trabalhos baseados naquele software.
- **Resolvendo problemas com software proprietário:** O copyleft foi criado para resolver o problema de softwares que, mesmo originados de código livre, eram transformados em proprietários, ou seja, fechados para uso, modificação e redistribuição. Ao aplicar uma licença copyleft, como a GPL, os desenvolvedores garantem que o software nunca poderá ser "fechado", assegurando que qualquer pessoa possa continuar a contribuir e se beneficiar do código no futuro.

### `+` Exemplos de licenças copyleft
- **GPL (GNU General Public License):** A licença copyleft mais popular, criada pela Free Software Foundation. Ela exige que qualquer software derivado de um código licenciado sob a GPL também seja distribuído sob a GPL, garantindo que o código permaneça livre em todas as suas versões.
- **AGPL (Affero General Public License):** Uma variante da GPL, focada em software que é executado em servidores. Ela assegura que os usuários que acessam o software remotamente (por exemplo, via web) também tenham os direitos garantidos pela GPL.

### `+` Comparação com licenças permissivas
O copyleft é frequentemente comparado com as licenças permissivas, como a MIT ou Apache 2.0, que oferecem maior liberdade de uso e modificação, mas sem a exigência de que os trabalhos derivados mantenham as mesmas liberdades.

- Licenças permissivas permitem que os usuários façam praticamente qualquer coisa com o código, incluindo a incorporação dele em software proprietário.
- Licenças copyleft, por outro lado, garantem que o código e suas melhorias permaneçam sempre livres, impondo restrições sobre como ele pode ser redistribuído.

## `-` O impacto da filosofia
A diferença entre as filosofias de Software Livre e Open Source se reflete diretamente nas licenças que promovem:
- **GPL (GNU General Public License):** Associada ao movimento de Software Livre, é uma licença copyleft que exige que qualquer software derivado também seja distribuído sob os mesmos termos, garantindo que as liberdades originais sejam mantidas. É ideal para quem deseja assegurar que todas as futuras versões do software permaneçam livres.
- **MIT:** Uma licença permissiva popular no mundo Open Source, que permite praticamente qualquer uso, desde que a licença original seja mantida, oferecendo maior liberdade para uso em contextos comerciais. É uma boa escolha para quem deseja que o software seja amplamente adotado, inclusive em projetos proprietários.
