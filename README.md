# Blockchain Experiments

# BitcoinCash

Bitcoin Cash é uma criptomoeda criada no dia 1 de agosto de 2017, em um processo de hard fork, separação, da Bitcoin. Trata-se da mais bem-sucedida bifurcação do bitcoin. Durante o processo de criação, todos os usuários de Bitcoin tiveram suas reservas privadas duplicadas, sendo as duplicatas nomeadas de "Bitcoin Cash", uma criptomoeda aparte do Bitcoin original, com propriedades técnicas distintas. É regida por um protocolo alternativo que aumenta a capacidade de transação em comparação ao Bitcoin "clássico", sendo este o ponto principal do fork. Isto será permitido graças ao tamanho de bloco diferenciado, de 8 MB. Este bloco, maior, em comparação ao original, visa auxiliar na correção do problema de escalabilidade, uma solução alternativa àquela adotada pelo Bitcoin, o SegWit (Segregated Witness), assim chamada a otimização de código polêmica que será ativada na blockchain do Bitcoin principal. Em 19 de dezembro de 2017, a Coinbase passou a permitir o depósito de Bitcoin Cash, o que permitiu que os usuários que possuiam Bitcoin na plataforma no momento do Hard Fork obtivessem uma quantia equivalente em Bitcoin Cash.<br/>

# Mecanismo de Consenso:

Uma questão fundamental na blockchain é: quem (qual nó) pode propor um novo bloco? Sabemos que a blockchain pública é uma rede aberta, formada por nós desconhecidos e sem uma autoridade central. Assim, é necessário a existência de um mecanismo que selecione quem tem o direito de propor um bloco em um dado momento.Isto é: um mecanismo capaz de manter o consenso na rede. Um mecanismo de consenso é um processo de acordo entre nós, mutuamente suspeitos, sobre uma mesma mensagem ou estado da blockchain. <br/>

A prova de trabalho (PoW) é uma forma de prova criptográfica na qual uma parte (o provador) prova a outras (os verificadores) que uma certa quantidade de um esforço computacional específico foi gasto. Os verificadores podem posteriormente confirmar esta despesa com um esforço mínimo da sua parte. O conceito foi inventado por Cynthia Dwork e Moni Naor em 1993 como uma maneira de impedir ataques de negação de serviço e outros abusos de serviço, como spam em uma rede, exigindo algum trabalho de um solicitante de serviço, geralmente significando tempo de processamento por um computador. O termo "prova de trabalho" foi cunhado e formalizado pela primeira vez em um artigo de 1999 por Markus Jakobsson e Ari Juels. A prova de trabalho foi mais tarde popularizada pelo Bitcoin como uma base para o consenso na rede descentralizada sem permissão, na qual os mineradores competem para anexar blocos e cunhar novas moedas, cada minerador experimentando uma probabilidade de sucesso proporcional ao esforço computacional gasto. <br/>

A prova de trabalho é um mecanismo de consenso para escolher quais desses participantes da rede – chamados de mineradores – têm permissão para lidar com a lucrativa tarefa de verificar novos dados. É lucrativo porque os mineradores são recompensados com novas criptomoedas quando validam com precisão os novos dados e não enganam o sistema. <br/>

“Proof of work é um algoritmo de software usado pelo Bitcoin e outros blockchains para garantir que os blocos sejam considerados válidos apenas se exigirem uma certa quantidade de poder computacional para serem produzidos”, diz Amaury Sechet, fundador da criptomoeda eCash. “É um mecanismo de consenso que permite que entidades anônimas em redes descentralizadas confiem umas nas outras.” Os mineradores vencedores só recebem sua recompensa de nova criptomoeda depois que outros participantes da rede verificarem se os dados adicionados à cadeia estão corretos e válidos. <br/>

Mecanismos de consenso na blockchain vêm da teoria dos jogos. Seu sistema deve ser projetado de tal forma que os nós obtenham o maior benefício se eles seguirem as regras. Um dos aspectos para garantir que os nós se comportem honestamente é recompensar o comportamento honesto e punir por atividades fraudulentas Atualmente. Há diferentes formas de chegar a um consenso entre os nós, dependendo do caso de uso. O mecanismo deve ser capaz de manter o consenso e a rede funcionando oferecendo algum incentivo aos nós para a blockchain ser autossustentável. <br/>

A Prova de Trabalho (Proof of Work) consiste em o usuário provar que gastou algum tempo para encontrar uma resposta que satisfaça um desafio computacional proposto pelo protocolo. <br/>

PoW é baseado em dois princípios:
- A prova dever ser difícil de ser produzida;
- Mas deve ser fácil de ser verificada. <br/>

A prova deve ser difícil e trabalhosa de se produzir, mas não impossível. Neste contexto o termo “difícil” deve ser entendido como uma solução algo que exige um grande poder computacional e alguns minutos de cálculo. Consequentemente, é financeiramente caro, devido a energia elétrica gasta durante o cálculo da solução. A verificação da solução deve ser rápida e fácil de ser executada pelos demais nós. <br/>

O processo de gerar um novo bloco é chamado de mineração e os nós que executam esse processo são chamados de mineradores. Cada nó minerador inicia esse processo ordenando, com base no timestamp, as transações que recebeu. Em seguida, o nó grava as transações em um bloco (um tipo de rascunho do bloco a ser proposto), sobre o qual será calculado a PoW. <br/>

A PoW é calculada aplicando-se uma função hash, SHA256, ao cabeçalho do bloco. O cabeçalho do bloco possui, entre outros campos, um nonce (número usado apenas uma vez). Os mineradores devem modificar o nonce frequentemente para obter um hash que satisfaça o critério de dificuldade (ou valor alvo). Assim, por definição, a saída desta função é um número entre 0 e 2^256. A mudança sistemática de nonce pelo minerador durante o cálculo da PoW visa encontrar uma colisão de hash parcial. Ou seja, o minerador deve encontrar um valor hash que seja igual ou menor que o valor alvo. <br/>

Portanto, encontrar um hash que satisfaça essa colisão parcial, depende essencialmente do poder computacional do nó minerador. Quando um nó encontra uma solução válida, ele propaga o bloco para os outros nós e todos devem confirmar mutuamente a validade do hash encontrado. Se o bloco for validado, diz-se que o bloco foi minerado e os demais nós anexam esse novo bloco a suas próprias blockchains armazenadas localmente. <br/>

O processo de mineração acontece de forma independente e simultaneamente por cada um dos full nodes. Note que, todos os mineradores da rede competem entre si para encontrar uma solução válida. O primeiro que encontrar tem o direito de propor o novo bloco. <br/>

Quando as transações são ordenadas e gravadas em um novo bloco, o hash do cabeçalho do bloco precisa ser calculado de modo a ser menor que o alvo da dificuldade. A dificuldade do trabalho deve ser ajustável para que haja um controle sobre a rapidez com que os blocos podem ser gerados.

A dificuldade é uma medida de quão difícil é encontrar um hash abaixo de um determinado alvo. A dificuldade responde à pergunta: “quantas vezes mais difícil é minerar um bloco agora, comparado com o quão difícil era minerar o bloco Gênesis?”. A dificuldade tem uma relação próxima com o alvo, mas não é a mesma coisa. Em vez disso, tem uma relação inversa, onde uma dificuldade maior implica um valor alvo menor.

No Bitcoin, a dificuldade é projetada para aumentar ou diminuir a cada 2.016 blocos. Isso leva em torno de duas semanas. Significa que um bloco deve ser gerado, em média, a cada 10 minutos. Se forem gerados em 2 semanas mais blocos que o esperado, a dificuldade é aumentada. Caso seja gerado menos que o esperado a dificuldade é então diminuída. 

Tanto o Bitcoin quanto o Bitcoin Cash usam um algoritmo de prova de trabalho para marcar cada novo bloco. O algoritmo de prova de trabalho usado é o mesmo em ambos os casos. Pode ser descrito como uma inversão parcial de uma função hash. Além disso, tanto o Bitcoin quanto o Bitcoin Cash visam um novo bloco a ser gerado a cada dez minutos em média. O tempo necessário para calcular um novo bloco é influenciado por um parâmetro chamado dificuldade de mineração. Se a quantidade total de poder de mineração aumentar, um aumento na dificuldade de mineração pode manter o tempo de bloqueio aproximadamente constante. Vice-versa, se o poder de mineração diminuir, uma diminuição da dificuldade de mineração pode manter o tempo de bloqueio aproximadamente constante.

Para manter o tempo de geração do bloco igual a dez minutos em média, tanto o Bitcoin quanto o Bitcoin Cash usam um algoritmo que ajusta o parâmetro de dificuldade de mineração. Esse algoritmo é chamado de algoritmo de ajuste de dificuldade (DAA). Originalmente, tanto o Bitcoin quanto o Bitcoin Cash usavam o mesmo algoritmo de ajuste de dificuldade, ajustando o parâmetro de dificuldade de mineração a cada 2016 blocos. Desde 1 de agosto de 2017, o Bitcoin Cash também usou uma adição ao DAA, chamado algoritmo de Ajuste de Dificuldade de Emergência (EDA). O EDA foi usado junto com o DAA original e foi projetado para diminuir a dificuldade de mineração do Bitcoin Cash em 20%, se a diferença de tempo entre 6 blocos sucessivos for maior que 12 horas.[34]

Os ajustes da EDA causaram instabilidades na dificuldade de mineração do sistema Bitcoin Cash, resultando no Bitcoin Cash milhares de blocos à frente do Bitcoin. Para resolver o problema com a estabilidade, foi implementada uma alteração do Bitcoin Cash DAA e o EDA cancelado. A alteração entrou em vigor em 13 de novembro de 2017. Após a alteração, o Bitcoin Cash DAA ajusta a dificuldade de mineração após cada bloco. Para calcular a dificuldade de um novo bloco, o Bitcoin Cash DAA usa uma janela móvel dos últimos 144 blocos.[34]

# Outras Características Importantes:
<strong>Diferenças entre Bitcoin e BitcoinCash:</strong></br>
Com o tempo, o número de diferenças entre Bitcoin e Bitcoin Cash continuou crescendo à medida que os desenvolvedores que trabalhavam em cada rede tinham objetivos diferentes em mente. A diferença entre as duas criptomoedas tornou-se tão grande que agora são vistas como ativos completamente diferentes na comunidade.
Como observado, a principal diferença entre Bitcoin e Bitcoin Cash é o tamanho do bloco. Por causa desse ajuste, o Bitcoin Cash pode ter transações mais rápidas e menos caras. Uma transação Bitcoin custa em média $ 59, enquanto o Bitcoin Cash custa menos de um centavo. A desvantagem de processar tudo mais rapidamente é que é potencialmente menos seguro que o Bitcoin. Há menos mineradores necessários para processar e confirmar transações, o que pode facilitar o comprometimento da segurança do Bitcoin Cash.
A principal diferença está relacionada ao tamanho do bloco de cada rede. Enquanto o Bitcoin mantém seu tamanho de bloco de 1 MB, com o Bitcoin Cash, os tamanhos de bloco aumentaram para 32 MB. Isso significa que as transações no BCH agora custam menos de um centavo e podem processar até 200 transações por segundo.
O Bitcoin Cash é uma bifurcação do Bitcoin que oferece melhorias quanto ao tempo de processamento e taxas.
A principal diferença entre as redes é o tamanho máximo de bloco permitido por cada rede, que no BCH é bem maior.
O que permite a rede Bitcoin Cash lidar com muito mais transações por segundo e tempos de espera mais curtos, assim como taxas de processamento menores.
Enquanto a taxa de transações no Bitcoin é de cerca de US$ 2,07, no Bitcoin Cash é de US$ 0,5. </br>

<strong>Vantagens e Desvantagens:</strong></br>
Transações mais rápidas e menos caras. Com um custo de transação de menos de um centavo e o potencial de processar mais de 100 transações por segundo, o Bitcoin Cash pode ser uma plataforma de pagamento viável. Ainda assim, a rede Visa processa 2.000 transações por segundo, então o Bitcoin Cash ainda tem um caminho a percorrer.
Mais escalável que o Bitcoin. Os blocos maiores do Bitcoin Cash permitem um blockchain com maior escalabilidade, resultando em taxas mais baixas para os usuários e, portanto, tornando-o mais transacionável.
Dinheiro descentralizado. Para aqueles preocupados com muito controle centralizado no sistema financeiro de bancos e governos centrais, o Bitcoin Cash oferece um sistema semelhante a uma moeda que é descentralizado e não controlado por nenhuma entidade.
Acessibilidade. Das milhares de criptomoedas existentes, o Bitcoin Cash é um dos mais populares e pode ser comprado na maioria das principais exchanges, ao contrário de concorrentes menos conhecidos. O preço do BCH/USD é de apenas US$ 370 por moeda, por isso também é mais acessível do que tentar comprar um único Bitcoin.

Taxa de adoção relativamente baixa. “Embora a maior parte do debate tenha se concentrado em debates tecnológicos sobre tempos de processamento e segurança, acho que há um grande fator negligenciado, mas talvez o mais importante com tecnologias emergentes: adoção”, disse Russell Star, chefe de mercados de capitais da DeFi Technologies. “O sucesso de qualquer tipo de rede, moeda ou tecnologia depende dos usuários que a utilizam.” Com menos pessoas usando Bitcoin Cash do que Bitcoin, ele pode ter dificuldades para crescer como um investimento aceito ou meio de troca.
Segurança mais fraca. O Bitcoin Cash processa as transações mais rapidamente e a um custo menor do que o Bitcoin porque requer menos poder de mineração para verificar novos blocos. Isso torna o sistema menos seguro que o Bitcoin.
Problemas de marca. Após o fork, houve uma batalha para ver qual moeda se tornaria mais popular. O Bitcoin foi o vencedor claro, o que torna difícil para o Bitcoin Cash se distinguir, especialmente porque eles compartilham um nome tão semelhante.
Impacto ambiental. O Bitcoin Cash ainda usa um sistema de prova de trabalho blockchain, onde os mineradores devem executar computadores para resolver equações criptográficas para processar transações, algo que consome uma energia considerável. Embora o Bitcoin Cash use menos eletricidade que o Bitcoin, esse sistema ainda tem um alto custo ambiental. De acordo com o New York Times, em 2009 você poderia minerar um Bitcoin usando um computador desktop comum e uma quantidade insignificante de eletricidade. Mas em 2021, você precisaria consumir uma quantidade de eletricidade igual à que uma casa americana padrão usaria em nove anos para minerar um Bitcoin.
O objetivo dos algoritmos de prova de trabalho não é provar que determinado trabalho foi realizado ou que um quebra-cabeça computacional foi "resolvido", mas impedir a manipulação de dados estabelecendo grandes requisitos de energia e controle de hardware para poder fazê-lo. Os sistemas de prova de trabalho têm sido criticados por ambientalistas por seu consumo de energia. <br/>

<strong>Avaliações e Uso:</strong></br>
“O dinheiro Bitcoin seria melhor para algo como uma xícara de café, enquanto uma compra maior, como um carro ou uma casa, pode garantir uma criptomoeda mais lenta e segura como o Bitcoin”, disse Daniel R. Hill, presidente da Hill Wealth Strategies em Virgínia.

<strong>BitcoinCash e o Mercado:</strong></br>
Até o momento, o Bitcoin Cash tem uma capitalização de mercado total de cerca de US$ 7,1 bilhões. Esta é uma fração do valor de mercado de US$ 881 bilhões do Bitcoin. "Forbes 17 maio".
Se você deve comprar Bitcoin Cash ou Bitcoin depende se você está procurando um investimento de longo prazo ou algo para usar em transações. “Quando medido em BTC, o preço do BCH caiu constantemente desde o seu início. É lógico que o Bitcoin original deve servir como um investimento mais seguro”, disse Gebbing. “Se escolher uma blockchain para fazer transações, o BCH é aceito em muitos dos mesmos lugares que aceitam BTC e pode ser usado por taxas quase zero devido ao tamanho do bloco maior e à menor utilização dessa cadeia”, acrescentou Gebbing. Como em qualquer investimento em criptomoedas, Star avisa que você deve ter cuidado. “Qualquer pessoa que considere investir em Bitcoin ou Bitcoin Cash deve considerar se pode suportar uma classe de ativos voláteis, que é o que é a criptomoeda.” Embora o conceito por trás do Bitcoin Cash tenha algum potencial, ele ainda não atingiu seu grande objetivo de substituir o Bitcoin original. Se começar a decolar como um meio de troca mais aceito, pode dar ao seu irmão mais velho e maior uma corrida mais difícil.
https://coinmarketcap.com/pt-br/currencies/bitcoin-cash/
