# How to Choose a License for Your Own Work
[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/sinabek/licences/blob/main/README.md)
[![pt-br](https://img.shields.io/badge/lang-pt--br-green.svg)](https://github.com/sinabek/licences/blob/main/README.pt.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.es.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.fr.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.de.md)


As pessoas costumam nos perguntar qual licença recomendamos que usem para seus projetos. Já escrevemos sobre isso publicamente antes, mas as informações foram espalhadas entre diferentes ensaios, entradas de FAQ e comentários de licença. Este artigo reúne todas essas informações em uma única fonte, para tornar mais fácil para as pessoas seguirem e consultarem.


Estas recomendações são para trabalhos projetados para fazer trabalhos práticos. Isso inclui software, documentação e algumas outras coisas. Obras de arte e obras que expressam um ponto de vista são questões diferentes; o Projeto GNU não tem uma posição geral sobre como eles devem ser lançados, exceto que todos devem ser utilizáveis sem software não-livre (em particular, sem DRM). No entanto, você pode querer seguir estas recomendações para obras de arte que acompanham um determinado programa.


As recomendações se aplicam ao licenciamento de um trabalho que você cria, seja uma modificação de um trabalho existente ou um novo trabalho original. Eles não abordam a questão de combinar material existente sob diferentes licenças. Se você está procurando ajuda com isso, verifique nosso FAQ GPL.

Depois de ver o que recomendamos aqui, se quiser orientação, escreva para <licensing@gnu.org>. Observe que provavelmente levará algumas semanas para a equipe de licenciamento entrar em contato com você; se você não obtiver resposta em um mês, por favor, escreva novamente.


## Contribuindo para um projeto existente


Quando você contribui para um projeto existente, geralmente deve lançar suas versões modificadas sob a mesma licença do trabalho original. É bom cooperar com os mantenedores do projeto, e usar uma licença diferente para suas modificações geralmente torna essa cooperação muito difícil. Você só deve fazer isso quando houver uma forte razão para justificá-lo.


Um caso em que o uso de uma licença diferente pode ser justificado é quando você faz grandes alterações em um trabalho sob uma licença não copyleft. Se a versão que você criou for consideravelmente mais útil que a original, então vale a pena fazer copyleft, pelos mesmos motivos que normalmente recomendamos o copyleft. Se você estiver nessa situação, siga as recomendações abaixo para licenciar um novo projeto.


Se você optar por liberar suas contribuições sob uma licença diferente por qualquer motivo, certifique-se de que a licença original permita o uso do material sob a licença escolhida. Por uma questão de honestidade, mostre explicitamente quais partes do trabalho estão sob qual licença.


### Programas


Recomendamos diferentes licenças para diferentes projetos, dependendo principalmente da finalidade do software. Em geral, recomendamos o uso da licença copyleft mais forte que não interfira nessa finalidade. Nosso ensaio “O que é Copyleft?” explica o conceito de copyleft com mais detalhes e por que geralmente é a melhor estratégia de licenciamento.


Para a maioria dos programas, recomendamos que você use a versão mais recente da GNU General Public License (GPL) para seu projeto. Seu forte copyleft é apropriado para todos os tipos de software e inclui várias proteções para a liberdade dos usuários. Para permitir futuras atualizações de licença, especifique “versão 3 ou qualquer versão posterior” para que seu programa seja compatível com a licença do código que pode ser lançado, no futuro, em versões GPL subsequentes.


### Pequenos programas


Não vale a pena usar o copyleft para a maioria dos programas pequenos. Usamos 300 linhas como referência: quando o código-fonte de um pacote de software é menor que isso, os benefícios proporcionados pelo copyleft são geralmente muito pequenos para justificar a inconveniência de garantir que uma cópia da licença sempre acompanhe o software.


Para esses programas, recomendamos a Licença Apache 2.0. Esta é uma licença de software fraca, frouxa e “pushover” (sem copyleft) que tem termos para impedir que colaboradores e distribuidores processem por violação de patente. Isso não torna o software imune a ameaças de patentes (nenhuma licença de software pode conseguir isso), mas evita que os detentores de patentes estabeleçam uma “isca e troca” onde eles liberam o software sob termos gratuitos e exigem que os destinatários concordem com termos não-livres em uma licença de patente.


Entre as licenças fracas (pushover), a Apache 2.0 é a melhor; portanto, se você for usar uma licença fraca, seja qual for o motivo, recomendamos o uso dessa.


### Bibliotecas


Para bibliotecas, distinguimos três tipos de casos.


Algumas bibliotecas implementam formatos de dados gratuitos que competem com formatos de dados restritos, como Ogg Vorbis (que compete com o áudio MP3) e WebM (que compete com o vídeo MPEG-4). O sucesso do formato livre requer permitir que muitos programas de aplicativos proprietários sejam vinculados ao código para lidar com o formato. Por exemplo, queríamos que players de mídia não livres, especialmente aparelhos, incluíssem o código para Ogg Vorbis e também para MP3.


Nessas situações especiais, se você deseja convencer os desenvolvedores de aplicativos proprietários a usar a biblioteca para o formato livre, você precisa facilitar isso licenciando a biblioteca sob uma licença fraca, como a Apache License 2.0.


No entanto, devemos reconhecer que esta estratégia não teve sucesso para Ogg Vorbis. Mesmo depois de alterar a licença de direitos autorais para permitir a fácil inclusão desse código de biblioteca em aplicativos proprietários, os desenvolvedores proprietários geralmente não o incluíram. O sacrifício feito na escolha da licença acabou nos ganhando pouco.


Para todas as outras bibliotecas, recomendamos algum tipo de copyleft. Se os desenvolvedores já estiverem usando uma biblioteca alternativa estabelecida lançada sob uma licença não-livre ou uma licença flexível flexível, recomendamos o uso da GNU Lesser General Public License (LGPL).


Ao contrário do primeiro caso, em que a biblioteca implementa um padrão eticamente superior, aqui a adoção por si só não atingirá nenhuma meta objetiva especial, portanto não há razão para evitar totalmente o copyleft. No entanto, se você exigir que os desenvolvedores que usam sua biblioteca liberem seus programas inteiros sob copyleft, eles simplesmente usarão uma das alternativas disponíveis, e isso também não promoverá nossa causa. A Lesser GPL foi projetada para preencher o meio termo entre esses casos, permitindo que desenvolvedores de software proprietário usem a biblioteca coberta, mas fornecendo um copyleft fraco que dá aos usuários liberdade em relação ao próprio código da biblioteca.


Para bibliotecas que fornecem instalações especializadas e que não enfrentam concorrência entrincheirada de não-copyleft ou não-livre, recomendamos o uso da GNU GPL simples. Para saber os motivos, leia “Por que você não deve usar a Lesser GPL para sua próxima biblioteca”.


### Software de servidor


Se for provável que outros façam versões aprimoradas de seu programa para rodar em servidores e não distribuam suas versões para mais ninguém, e você está preocupado que isso colocará sua versão lançada em desvantagem, recomendamos a Licença Pública Geral GNU Affero (AGPL). Os termos da AGPL são quase idênticos aos da GPL; a única diferença substantiva é que ele tem uma condição extra para garantir que as pessoas que usam o software em uma rede possam obter o código-fonte para ele.


O requisito da AGPL não aborda os problemas que podem surgir para os usuários quando eles confiam sua computação ou seus dados ao servidor de outra pessoa. Por exemplo, isso não impedirá que o Serviço como Substituto de Software (SaaSS) negue a liberdade dos usuários — mas a maioria dos servidores não usa SaaSS. Para saber mais sobre essas questões, leia “Por que o Affero GPL.”


### Documentação


Recomendamos a GNU Free Documentation License (GFDL) para tutoriais, manuais de referência e outros grandes trabalhos de documentação. É uma forte licença copyleft para trabalhos educacionais, inicialmente escrita para manuais de software, e inclui termos que tratam especificamente de problemas comuns que surgem quando esses trabalhos são distribuídos ou modificados.


Para trabalhos curtos de documentação secundária, como um cartão de referência, é melhor usar a licença GNU totalmente permissiva, pois uma cópia do GFDL dificilmente caberia em um cartão de referência. Não use CC BY, pois é incompatível com o GFDL.


Para páginas de manual, recomendamos o GFDL se a página for longa e a licença GNU totalmente permissiva se for curta.


Algumas documentações incluem código fonte de software. Por exemplo, um manual para uma linguagem de programação pode incluir exemplos para os leitores seguirem. Você deve incluí-los no manual sob os termos da FDL e liberá-los sob outra licença apropriada para o software. Isso ajuda a facilitar o uso do código em outros projetos. Recomendamos que você dedique pequenos pedaços de código ao domínio público usando CC0 e distribua pedaços maiores sob a mesma licença que o projeto de software associado usa.


### Outros dados para programas


Esta seção discute todos os outros trabalhos para uso prático que você pode incluir com o software. Para dar alguns exemplos, isso inclui ícones e outros gráficos funcionais ou úteis, fontes e dados geográficos. Você também pode segui-los para arte, embora não critiquemos se você não o fizer.


Se você estiver criando esses trabalhos especificamente para uso com um projeto de software, geralmente recomendamos que você libere seu trabalho sob a mesma licença do software. Não há nenhum problema em fazer isso com as licenças que recomendamos: GPLv3, LGPLv3, AGPLv3 e GPLv2 podem ser aplicadas a qualquer tipo de trabalho—não apenas software—que seja protegido por direitos autorais e tenha uma forma preferida clara para modificação. Usar a mesma licença do software ajudará a tornar a conformidade mais fácil para os distribuidores e evitar qualquer dúvida sobre possíveis problemas de compatibilidade. O uso de uma licença gratuita diferente pode ser apropriado se fornecer algum benefício prático específico, como melhor cooperação com outros projetos gratuitos.


Se o seu trabalho não estiver sendo criado para uso com um projeto de software específico, ou se não for apropriado usar a mesma licença do projeto, recomendamos apenas que você escolha uma licença copyleft que seja apropriada para o seu trabalho. Temos alguns deles listados em nossa lista de licenças. Se nenhuma licença parecer especialmente apropriada, a licença Creative Commons Attribution-ShareAlike é um copyleft que pode ser usado para muitos tipos diferentes de trabalhos.