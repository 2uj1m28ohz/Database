# `/` Escolher

![](/SoftwareLicenses/Image.png)

`>` `The Law/David Camargo`

Escolher a licença correta para um projeto de software é uma decisão estratégica, que depende dos objetivos do projeto e da comunidade que você deseja atrair. A licença não apenas define como o código pode ser utilizado, mas também impacta a colaboração, a distribuição e o potencial comercial do software.

## `-` Avaliação de critérios
- **Compatibilidade com outros projetos:** Licenças diferentes têm regras variadas sobre como o código pode ser combinado e redistribuído. Se você pretende integrar bibliotecas de terceiros, é essencial escolher uma licença que seja compatível com elas. Por exemplo, a GPLv3 pode não ser compatível com algumas licenças permissivas, o que pode limitar as opções de integração.
- **Filosofia do projeto:** A escolha da licença deve refletir a filosofia do projeto. Se o objetivo é garantir que todas as melhorias sejam sempre compartilhadas com a comunidade, uma licença copyleft, como a GPL, pode ser mais adequada. Por outro lado, se a flexibilidade e a adoção em ambientes comerciais são prioridades, uma licença permissiva, como a MIT ou a Apache, pode ser mais apropriada.
- **Ambição comercial:** Para projetos que visam integração em produtos comerciais, uma licença permissiva é geralmente mais atrativa para parceiros de negócios, pois permite que eles usem o código sem as obrigações que uma licença copyleft impõe. Isso pode facilitar parcerias e colaborações com empresas que preferem manter seu código fechado.

## `-` Ferramentas de escolha
- **[Choose A License][CAL]:** Este site fornece uma visão geral de várias licenças populares, ajudando os desenvolvedores a entender as implicações de cada escolha. Ele oferece comparações diretas e orientações para encontrar a licença que melhor se alinha aos objetivos do seu projeto.
- **[SPDX][SPDX] (Software Package Data Exchange):** O SPDX é um padrão que fornece identificadores unificados para licenças, facilitando a gestão de dependências e a conformidade em projetos complexos. Utilizar o SPDX pode ajudar a evitar problemas legais e garantir que todas as partes interessadas estejam cientes das licenças em uso.

## `-` O impacto da escolha
- A escolha da licença pode afetar a disposição de novos colaboradores em contribuir para o projeto. Licenças mais restritivas podem desestimular contribuições, enquanto licenças permissivas frequentemente atraem desenvolvedores e empresas que desejam experimentar e adaptar o código.
- Licenças permissivas tendem a atrair mais contribuições de empresas, que muitas vezes estão mais dispostas a colaborar em projetos que não exigem que suas modificações sejam abertas. Em contraste, licenças copyleft são mais apreciadas por desenvolvedores que valorizam a transparência e o compartilhamento de melhorias.

## `-` Consequências legais
Escolher uma licença inadequada pode levar a complicações legais sérias. Por exemplo, se um projeto é licenciado sob uma licença copyleft e um desenvolvedor usa o código em um projeto fechado, isso pode resultar em ações legais por violação de direitos autorais. Além disso, a falta de clareza na licença pode causar confusões sobre os direitos e responsabilidades, levando a litígios e danos à reputação do projeto.

## `-` Histórias de sucesso
A escolha da licença pode ser observada em diversos projetos notáveis:
- **Linux Kernel (GPLv2):** A escolha da GPLv2 permitiu que o kernel se tornasse uma das maiores e mais colaborativas iniciativas open source, promovendo um ambiente de desenvolvimento ativo.
- **Mozilla Firefox (MPL):** Utiliza a Mozilla Public License, que equilibra permissividade e copyleft, permitindo que as alterações sejam feitas e compartilhadas, ao mesmo tempo que possibilita a integração com software proprietário.
- **Chromium e derivados (BSD):** O Chromium, base do Google Chrome, é licenciado sob a licença BSD, o que facilita a colaboração e o desenvolvimento de diversas aplicações que utilizam essa base.
- **TensorFlow (Apache 2.0):** O framework de aprendizado de máquina do Google, facilitando a adoção por empresas e pesquisadores, resultando em uma ampla gama de contribuições da comunidade.
- **WordPress (GPL):** Uma das plataformas de gerenciamento de conteúdo mais populares do mundo, que promove uma cultura de contribuição e personalização, permitindo um ecossistema vibrante.
- **Blender (GPL):** Licenciado sob a GPL, permitindo que uma comunidade engajada contribuísse para seu desenvolvimento e se tornando uma ferramenta respeitada na indústria de animação.
- **GIMP (GPL):** O software de edição de imagens muito popular, que permitiu uma ampla comunidade de desenvolvedores contribuírem com melhorias ao longo dos anos.
- **LibreOffice (MPL/GPL):** Uma suíte de escritório livre e open source, que promove um forte compromisso com a comunidade e a colaboração, resultando em uma alternativa robusta ao Microsoft Office.
- **7-Zip (GNU LGPL):** Um software de compressão de arquivos eficiente, que permite a utilização em projetos abertos ou proprietários, se destacando por sua simplicidade e eficácia.
- **Visual Studio Code (MIT License):** Um editor de código-fonte da Microsoft que se tornou uma das ferramentas de desenvolvimento mais populares do mundo, permitindo contribuições ativas da comunidade.
- **PowerShell (MIT License):** Lançado como open source, expandindo seu suporte para várias plataformas e ajudando a comunidade a criar scripts e ferramentas mais poderosas e interoperáveis.

[CAL]: https://choosealicense.com
[SPDX]: https://spdx.org