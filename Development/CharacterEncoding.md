## :arrow_right: Codificação de Caracteres

<img align="right" height="600px" src="https://github.com/2uj1m28ohz/Database/blob/main/Development/CharacterEncoding.png"/>

A codificação de caracteres é um sistema que atribui códigos numéricos a caracteres e símbolos para permitir sua representação em computadores e dispositivos eletrônicos. Ela é essencial para a transmissão, armazenamento e exibição de texto em diferentes idiomas e sistemas de computador.

Os computadores entendem apenas números, então, para representar letras, números, símbolos e caracteres especiais, é necessário um sistema de codificação. Um dos sistemas mais comuns é o Unicode, que atribui um número único para cada caractere, permitindo a representação de uma ampla gama de idiomas e símbolos.

Outras codificações de caracteres incluem o ASCII (American Standard Code for Information Interchange) e o UTF-8 (Unicode Transformation Format), entre outros. Cada um desses sistemas utiliza diferentes conjuntos de números para representar caracteres, e a escolha de uma codificação específica pode afetar a forma como o texto é exibido ou interpretado em diferentes sistemas e softwares.

O UTF-8 é uma codificação de caracteres que se tornou amplamente adotada por sua capacidade de representar todos os caracteres Unicode enquanto mantém compatibilidade com o ASCII, que é um conjunto mais antigo e menor de caracteres. O UTF-8 é usado extensivamente em sistemas operacionais atuais por algumas razões principais:

- **Compatibilidade com ASCII:** Os primeiros 128 caracteres do Unicode correspondem exatamente aos caracteres ASCII. Isso significa que qualquer texto ASCII é automaticamente interpretado como UTF-8, tornando-o retrocompatível.

- **Eficiência de espaço:** O UTF-8 é projetado para ser eficiente em termos de espaço. Para caracteres comuns (especialmente em idiomas ocidentais), ele usa 1 byte por caractere, mantendo a compatibilidade com ASCII. Caracteres adicionais usam de 2 a 4 bytes, o que é crucial para representar uma ampla gama de idiomas e símbolos.

- **Ampla adoção:** É amplamente suportado em sistemas operacionais modernos, navegadores da web, linguagens de programação e aplicativos. Isso torna o UTF-8 uma escolha comum para armazenamento e transmissão de texto em ambientes digitais.

Nos sistemas operacionais atuais, como Windows, macOS, Linux e outros, o UTF-8 é amplamente suportado e frequentemente utilizado como a codificação de caracteres padrão. Ele é escolhido devido à sua capacidade de representar uma vasta gama de caracteres e sua eficiência em termos de espaço de armazenamento e transmissão de texto multilíngue.

Muitos desenvolvedores e administradores de sistemas preferem usar UTF-8 como a codificação de caracteres padrão em seus projetos devido à sua versatilidade e compatibilidade com diferentes idiomas e sistemas, facilitando a internacionalização e garantindo uma representação precisa de caracteres em várias línguas.

<details>
<summary>ASCII</summary>

ASCII (American Standard Code for Information Interchange): É um conjunto de caracteres que atribui códigos numéricos a letras, números, símbolos e comandos especiais usados em computadores e dispositivos. O ASCII originalmente inclui 128 caracteres e foi amplamente utilizado em sistemas informáticos mais antigos. No entanto, ele só era capaz de representar caracteres da língua inglesa e carecia de suporte para muitos outros idiomas e símbolos.

</details>

<details>
<summary>Unicode</summary>

Unicode é um padrão de codificação que visa representar todos os caracteres de todas as línguas e sistemas de escrita conhecidos. Ele define uma tabela de caracteres que atribui um número único (chamado de code point) a cada caractere, símbolo ou ideograma. O Unicode inclui muito mais caracteres do que o ASCII e é capaz de representar uma ampla gama de idiomas, símbolos e emojis.

</details>

<details>
<summary>UTF</summary>

UTF (Unicode Transformation Format): É uma família de esquemas de codificação que implementam o padrão Unicode para representar esses code points como sequências de bytes. As diferentes variantes do UTF incluem UTF-8, UTF-16 e UTF-32. Cada uma dessas variantes do UTF (Unicode Transformation Format) é uma forma de codificar os code points do Unicode em sequências de bytes para representar caracteres. Aqui está uma descrição de cada uma:

- UTF-8:

    - É uma codificação de comprimento variável.

    - Usa de 1 a 4 bytes por caractere.

    - É o mais popular na web e em sistemas baseados em texto.

    - Caracteres comuns (ASCII) são representados por 1 byte.

    - Caracteres menos comuns usam mais bytes.

    - Oferece compatibilidade com ASCII nos primeiros 128 caracteres.

- UTF-16:

    - Usa 2 ou 4 bytes por caractere.

    - Projetado para suportar todos os code points Unicode, incluindo os fora do BMP (Plano Multilíngue Básico), que estão além dos primeiros 65.536 caracteres.

    - É amplamente usado em sistemas que lidam com caracteres não-BMP, como muitos ideogramas e símbolos mais raros.

- UTF-32:

    - Usa 4 bytes por caractere, o que o torna uma codificação de tamanho fixo.

    - Atribui exatamente um code point Unicode a cada unidade de 32 bits.

    - Permite acesso direto a qualquer caractere no conjunto Unicode sem a necessidade de cálculos adicionais.

A escolha entre UTF-8, UTF-16 e UTF-32 geralmente depende das necessidades do sistema em relação ao suporte de idiomas, eficiência de armazenamento e processamento, bem como a necessidade de representar caracteres fora do BMP. O UTF-8 é comumente usado na web devido à sua eficiência de espaço e compatibilidade com ASCII, enquanto o UTF-16 e UTF-32 são mais adequados para ambientes que lidam com um grande número de caracteres além dos 65.536 primeiros caracteres Unicode.

<details>
<summary>Byte Order Mark</summary>

O BOM (Byte Order Mark) é uma sequência especial de bytes usada para indicar a ordem dos bytes em um arquivo de texto. O BOM é relevante principalmente em sistemas que armazenam texto codificado em UTF-16 ou UTF-32 para indicar se os bytes mais significativos ou menos significativos vêm primeiro. No caso do UTF-8:

- UTF-8 BOM (UTF-8 with BOM):

    - É uma variante do UTF-8 que inclui o BOM.

    - Consiste em uma sequência de bytes (0xEF, 0xBB, 0xBF) colocada no início do arquivo.

    - Seu propósito principal é indicar que o arquivo está codificado em UTF-8.

- UTF-8 No BOM (UTF-8 without BOM):

    - É o UTF-8 sem a presença do BOM.

    - Não possui os bytes que indicam a ordem do byte.

    - É comum em sistemas que não exigem a marca de ordem de byte ou onde a presença do BOM pode causar problemas de compatibilidade com sistemas que não interpretam corretamente esses bytes no início do arquivo.

A presença ou ausência do BOM em arquivos UTF-8 geralmente depende das preferências do sistema ou das aplicações que os criam. Alguns editores de texto ou ambientes de desenvolvimento permitem escolher se um arquivo UTF-8 deve ter ou não o BOM, enquanto outros geram automaticamente o BOM ao salvar um arquivo em UTF-8.

Em muitos casos, especialmente na web, o UTF-8 sem BOM é preferido, pois a presença do BOM pode causar problemas de interpretação em alguns sistemas ou aplicativos que não esperam ou interpretam incorretamente esses bytes no início do arquivo.

</details>

</details>
