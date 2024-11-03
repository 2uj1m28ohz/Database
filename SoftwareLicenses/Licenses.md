# `/` Licenças

![](/SoftwareLicenses/Image.png)

`>` `The Law/David Camargo`

No desenvolvimento de software, a escolha de uma licença é fundamental para definir como seu código pode ser utilizado, modificado e redistribuído por outros. Existem licenças específicas para software que melhor se adequam a esse tipo de produto, equilibrando a proteção da propriedade intelectual e a liberdade de uso e modificação. Algumas são mais permissivas, permitindo amplo uso, enquanto outras possuem restrições mais rigorosas, como o copyleft, que exige que o código derivado seja licenciado sob os mesmos termos.

## `-` Licenças de software

|Licença                   |Identificador|Tipo      |Aprovada pela OSI|Aprovada pela FSF|
|:-------------------------|:------------|:---------|:---------------:|:---------------:|
|MIT License               |MIT          |Permissiva|Sim              |Sim              |
|Apache 2.0                |Apache-2.0   |Permissiva|Sim              |Sim              |
|GNU GPLv3                 |GPL-3.0-Only |Copyleft  |Sim              |Sim              |
|BSD-3 Clause              |BSD-3-Clause |Permissiva|Sim              |Sim              |
|BSD-4 Clause              |BSD-4-Clause |Permissiva|Não              |Sim              |
|Mozilla Public License 2.0|MPL-2.0      |Copyleft  |Sim              |Sim              |

## `-` Versões desatualizadas
Algumas versões antigas de licenças, embora ainda em uso, não são amplamente recomendadas devido a questões de compatibilidade, funcionalidades limitadas ou mudanças nas necessidades legais e de mercado. Um dos exemplos mais notáveis é a GPLv2, que, apesar de sua popularidade, apresenta problemas de compatibilidade que foram abordados na GPLv3, como questões relacionadas a patentes e distribuição em rede (ou "Tivoização"). A GPLv3 foi introduzida para resolver essas lacunas, tornando-a a escolha preferida por muitos desenvolvedores modernos.

### `+` Atualização flexível
A adoção de versões mais recentes de uma licença não é obrigatória. Os desenvolvedores podem optar por permanecer com a versão anterior, dependendo de como a licença foi originalmente atribuída ao projeto. Entretanto, muitas licenças oferecem a possibilidade de escolher entre:

- **"Only":** Especifica que o código está vinculado a uma versão específica da licença. Por exemplo, "GPLv2 only" significa que o software pode ser usado e redistribuído apenas sob os termos da GPLv2.
- **"Or Later":** Especifica que o código pode ser redistribuído sob a versão mencionada ou qualquer versão posterior da licença. Por exemplo, "GPLv2 or later" permite que o código seja redistribuído sob os termos da GPLv2 ou de qualquer versão futura da GPL, como a GPLv3.

Na prática, a escolha entre "only" e "or later" influencia a flexibilidade de migração para versões mais novas. Quando o código é licenciado como "GPLv2 only", ele fica restrito às regras da GPLv2, o que pode gerar problemas de compatibilidade com projetos que utilizam a GPLv3. No entanto, ao utilizar a cláusula "GPLv2 or later", os desenvolvedores têm a liberdade de optar pela versão mais recente quando apropriado.

### `+` Antes de atualizar
Ao migrar de versões antigas de uma licença para versões mais recentes, os desenvolvedores precisam considerar algumas questões importantes:
- **Compatibilidade do código:** O primeiro passo para migrar de uma licença antiga (como a GPLv2) para uma nova (como a GPLv3) é garantir que o código seja compatível com a nova licença. Algumas licenças mais permissivas podem ser mais fáceis de migrar, mas licenças copyleft exigem uma revisão cuidadosa das dependências e da integração com outras bibliotecas.
- **Aprovação dos colaboradores:** Se o projeto utiliza a licença "Only", qualquer mudança exigirá a aprovação de todos os colaboradores que contribuíram com o código. Isso pode ser um obstáculo em projetos maiores com muitos contribuidores.
- **Impacto nos usuários:** A migração para uma licença mais recente pode impactar os usuários e como eles utilizam o software. Licenças como a GPLv3 incluem novos termos de patentes e proteções contra dispositivos que limitam as modificações de software (Tivoização), o que pode não ser desejável em todos os casos.
- **Transição transparente:** Ferramentas como a [SPDX License Identifiers](https://spdx.org/licenses) e sites como o [ChooseALicense.com](https://choosealicense.com) podem ajudar os desenvolvedores a identificar as melhores práticas e as licenças mais compatíveis ao realizar a migração.

## `-` Compatibilidade entre licenças open source
Nem todas as licenças são compatíveis entre si, e a escolha da licença impacta como o software pode ser combinado com outros projetos:
- **MIT e Apache 2.0:** São altamente compatíveis entre si e podem ser integradas facilmente. Ambas permitem uso e redistribuição ampla, incluindo integração com código fechado.
- **GPLv3:** É menos compatível com licenças permissivas como a Apache 2.0 ou MIT, já que exige que o código derivado seja distribuído sob os mesmos termos de copyleft.
 - **MPL 2.0:** Pode ser combinada com software proprietário, mas exige que as alterações feitas no código MPL sejam divulgadas. Ela é compatível com licenças permissivas, mas apresenta desafios quando combinada com a GPL.

## `-` Compatibilidade com licenças proprietárias
Quando se trata de integrar código open source com software proprietário, algumas licenças são mais flexíveis que outras:
- **MIT, BSD (3-Clause e 4-Clause), e Apache 2.0:** Todas permitem que o código seja integrado em projetos proprietários sem exigir que o restante do projeto seja aberto. Isso faz delas escolhas populares para empresas que desejam manter parte de seu código fechado.
- **GPLv3:** Não permite que código seja fechado; qualquer projeto derivado deve ser distribuído sob a mesma licença, impedindo o uso em projetos proprietários.
- **MPL 2.0:** Permite que partes do software sejam combinadas com código proprietário, desde que as modificações no código MPL sejam abertas e licenciadas sob MPL.