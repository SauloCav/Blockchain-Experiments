# Blockchain Experiments

# Fantom
Fantom é uma plataforma de contrato inteligente de alto desempenho, escalável, compatível com EVM e segura.

A implantação da rede principal do Fantom - Fantom Opera - é construída no mecanismo de consenso do Fantom, Lachesis. O Fantom é um protocolo blockchain de camada 1 sem líder, assíncrono e tolerante a falhas bizantino.

O Lachesis permite que o Fantom forneça velocidades de transação rápidas, baixos custos de transação e finalidade determinística. Isso é alcançado enquanto permanece sem permissão, descentralizado e de código aberto.

O nascimento do Bitcoin em 2009 representou um grande passo em frente na tecnologia e mais um passo em direção a uma sociedade mais eficiente. No entanto, o Bitcoin não foi construído para escalar, e seu mecanismo de consenso – o mecanismo que alimenta o blockchain – é limitado pelo design.

As soluções atuais fazem concessões entre três componentes: escalabilidade, segurança e descentralização. Isso é conhecido como o trilema blockchain.

O Bitcoin, por exemplo, se concentra na descentralização e na segurança, o que o torna menos adequado para qualquer tipo de transação que exija velocidade e confirmação rápida, como pagamentos diários, transferência de dados, negociação de ativos ou outras transações nas quais consumidores e empresas confiam na vida cotidiana .

Especialmente o sistema financeiro legado, desde os processos que acontecem no back-end até as soluções voltadas para o consumidor, exige alto rendimento e rapidez de finalização.
Descentralizar esses serviços em escala, ao mesmo tempo em que fornece segurança de nível bancário, representa um desafio para toda a indústria de blockchain.

A Fantom aborda o problema em sua essência: seu mecanismo de consenso de alta velocidade, Lachesis, permite que ativos digitais operem em velocidade sem precedentes e oferece melhorias dramáticas em relação aos sistemas atuais.

Ao contrário de outras soluções, o Fantom não sacrifica a segurança e a descentralização em favor da escalabilidade.

De fato, as vantagens trazidas pelo Fantom não são apenas desempenho puro; sua arquitetura modular permite total customização de blockchains para ativos digitais, com diferentes características adaptadas ao seu caso de uso.

O Fantom também oferece níveis excepcionalmente altos de segurança usando um protocolo Proof-of-Stake sem líder para proteger a rede.

O consenso aBFT da Fantom, chamado Lachesis, é capaz de escalar para muitos nós ao redor do mundo em um ambiente aberto e sem permissão, proporcionando um bom grau de descentralização. Não usa Prova de Participação Delegada e não tem conceito de “Masternodes”.


# Mecanismo de Consenso
O mecanismo de consenso é o núcleo das tecnologias distribuídas. Em um ambiente descentralizado, onde nenhuma entidade central valida as transações, o protocolo de consenso garante que todos os participantes da rede cheguem a um acordo: a rede como um todo valida as transações de forma totalmente confiável.

Lachesis é o algoritmo de consenso aBFT do Fantom. Simplificando, um mecanismo de consenso é o mecanismo que alimenta o blockchain.
Comparado ao consenso Classical e Nakamoto, Lachesis é uma escolha mais rápida, mais escalável e mais segura.
Os desenvolvedores podem usar o Lachesis para criar aplicativos ponto a ponto sem precisar criar sua própria camada de rede.

Lachesis é:
Assíncrono: Os participantes têm a liberdade de processar comandos em momentos diferentes.
Sem líder: Nenhum participante desempenha um papel “especial”.
Tolerante a falhas bizantinas: Suporta um terço dos nós defeituosos, incluindo comportamento malicioso.
Final: A saída de Lachesis pode ser usada imediatamente. Não há necessidade de esperar por confirmações de bloqueio; as transações são confirmadas em 1-2 segundos.

## Asynchronous Byzantine Fault Tolerance (aBFT)
A tolerância a falhas bizantinas assíncronas é o mais alto padrão de algoritmos de consenso. Ele resolve o Trilema de Escalabilidade do blockchain, segundo o qual apenas dois dos três componentes a seguir são possíveis ao mesmo tempo:
Descentralização
Segurança
Escalabilidade
Um protocolo de consenso aBFT permite máxima descentralização, alta escalabilidade e segurança de nível bancário.

Em uma rede aBFT, os nós podem chegar a um consenso independentemente de transmitir essas informações e não precisam trocar blocos finalizados.
Por esta razão, os mecanismos de consenso aBFT são completamente sem liderança, aumentando a segurança: não há round-robin e nenhuma prova de trabalho.

Ao contrário do pBFT, que se baseia no fato de que todas as mensagens compartilhadas entre os nós serão eventualmente entregues, o aBFT permite que as mensagens sejam atrasadas ou perdidas por completo. Além de tornar as redes particularmente resistentes a ataques DDoS, o aBFT também reduz a latência da transação, resultando em uma rede mais rápida.

Por fim, as redes aBFT permitem maior escalabilidade e descentralização, pois não há comunicação excessiva para limitar o número de nós participantes.

## Lachesis consensus
Lachesis é um algoritmo de consenso aBFT baseado em DAG que oferece melhorias tangíveis nos modelos Classical e Nakamoto.
Lachesis é assíncrona, sem liderança e final, além de ser tolerante a falhas bizantinas.

Lachesis é projetado para se conectar facilmente a aplicativos escritos em qualquer linguagem de programação. Os desenvolvedores podem se concentrar na construção da lógica do aplicativo e integrar o Lachesis para lidar com o aspecto de replicação da máquina de estado.

Lachesis se conecta a outros nós Lachesis e garante que todos processem os mesmos comandos na mesma ordem. Para fazer isso, ele usa rede ponto a ponto e um algoritmo de consenso DAG aBFT.

## Por que Lachesis
Criamos Lachesis para superar as limitações dos algoritmos de consenso anteriores. Na verdade, é a opção ideal para aplicativos que precisam de alto rendimento, rapidez e segurança de nível bancário.
No mundo acelerado de hoje, qualquer coisa que exija uma espera ou atraso de qualquer tipo simplesmente não seria usada.

Lachesis remove a barreira para a criação de aplicativos rápidos e descentralizados que qualquer um pode usar.
Se você está criando uma versão aprimorada de produtos existentes
para setores como pagamentos, rastreamento da cadeia de suprimentos, armazenamento de dados de saúde e muito mais, ou revolucionando uma indústria emergente como DeFi, a Lachesis pode fazer tudo.

## Como o Lachesis funciona
Cada nó Lachesis armazena um grafo direcionado acíclico local (DAG) composto de blocos de eventos, cada um dos quais contém transações. O DAG, capturando o relacionamento acontecer antes entre os eventos, é usado para calcular uma ordem final exata dos eventos - e, portanto, das transações - independentemente em cada nó.

Os blocos de eventos são divididos em blocos de eventos confirmados e não confirmados. Novos blocos de eventos não são confirmados, enquanto os blocos de eventos dos últimos 2-3 quadros são todos confirmados e posteriormente ordenados por nós honestos.

O consenso resulta em lotes de blocos de eventos confirmados, onde cada lote de eventos é chamado de bloco. Blocos finalizados que formam a cadeia final são calculados a partir de blocos de eventos independentemente em cada nó.

Ao contrário do Proof-of-Work, Proof-of-Stake round-robin, Proof-of-Stake de cunhagem e BFT de sincronização, os nós Lachesis não; enviar blocos uns aos outros. Apenas os eventos estão sendo sincronizados entre os nós. Os validadores não votam em um estado concreto da rede; em vez disso, eles trocam periodicamente transações e eventos observados com seus pares.

Ao contrário do consenso clássico, como o pBFT, Lachesis não usa novos eventos na eleição atual; em vez disso, novos eventos são usados ​​para votar nos eventos em 2-3+ eleições virtuais anteriores simultaneamente. Isso leva a um número menor de mensagens de consenso criadas, pois o mesmo evento é reutilizado em diferentes eleições.
Assim, Lachesis atinge um menor tempo de finalização e uma menor sobrecarga de comunicação em comparação com o BFT síncrono.

## Épocas em Lachesis
A estrutura de eventos de Lachesis é um DAG de eventos. Para otimizar o armazenamento e a recuperação, o DAG é separado em sub-DAGs, cada um deles é chamado de época. Cada época compreende muitos blocos finalizados.

Cada época é selada quando uma destas condições é satisfeita:

A época atinge um número definido de blocos
A época dura por um tempo especificado
Pelo menos um trapaceiro está confirmado neste bloco
A vedação de época é solicitada pelo contrato NodeDriver
Quando uma época é selada, seus índices de época internos são removidos e novos eventos das épocas seladas são ignorados. Cada época forma um DAG separado e, portanto, pais de outras épocas não são permitidos.

Para uma verificação de sanidade, cada evento inclui o hash da época anterior.

Para uma visão mais técnica e aprofundada do Lachesis, você pode conferir nosso Wiki no GitHub.


# Outras Características Importantes

## Avaliações e Uso
O sucesso de Fantom pode ser melhor compreendido no contexto das chamadas “guerras de primeira camada”.

O Ethereum é lento e caro de usar e continuará assim (considerando que a quantidade de atividade da rede continue a mesma) até que atualizações ao protocolo forem implementadas. Isso pode levar alguns anos.

É tempo demais para pessoas que querem utilizar protocolos DeFi ao máximo atualmente, mas consideram apps DeFi nativos do Ethereum caros demais.

Alguns desenvolvedores, como os responsáveis por Loopring, Arbitrum e Optimism, decidiram criar soluções de primeira e segunda camada para acelerar a experiência do Ethereum sem abrir mão da segurança da rede.

Outras blockchains decidiram substituir Ethereum completamente (o Ethereum é conhecido como a camada base, primeira camada ou “L1”).

Solana, Avalanche, Polkadot, Terra (tecnicamente, uma blockchain de aplicações do Cosmos) e Fantom são as líderes dessa corrida, apesar de todas as suas moedas nativas terem despencado bastante desde suas altas recordes.

Dentre esses protocolos de primeira camada, LUNA, a moeda do Terra, é a maior, com uma capitalização de mercado de US$ 29 bilhões, seguida de Solana, com uma capitalização de US$ 26 bilhões. FTM está mais distante, com US$ 3,4 bilhões.

Cada uma dessas blockchains é lar de sua própria indústria DeFi. Segundo dados do DeFi Llama, o mercado DeFi do Terra é o maior após o Ethereum.

Atualmente, o Ethereum tem quase US$ 117 bilhões de valor total bloqueado (ou TVL) e Terra tem US$ 25,3 bilhões. Fantom, em sexto lugar, possui US$ 6,7 bilhões, perdendo para Solana, em quinto lugar, com US$ 7 bilhões.

## Serviços Fantom
### Fantom Finance
Permite a emissão de ativos sintéticos, staking de liquidez, tomada e concessão descentralizadas de empréstimos.

### SpookySwap
Um formador automatizado de mercado (ou AMM) descentralizado. É como um Uniswap, mas no Fantom. Seu token, para combinar com o nome “spooky” (“assustador”, em português), possui o código negociação “BOO”.

### Multichain
Um protocolo de roteamento entre blockchains.

### Solidly
Uma corretora descentralizada (ou DEX) com pouco “slippage” (diferença entre o preço esperado e o preço verdadeiro). Solidly foi criada por Andre Cronje, o criador do protocolo Yearn Finance (YFI).

É operada com um modelo “(3,3)”, assim como a OlympusDAO. “(3,3)” é uma situação da teoria de jogos em que participantes sabem do cenário mais benéfico para todos e ou ganham juntos ou perdem juntos.

Assim, na OlympusDAO, “(3,3)” representa a escolha de colocar tokens OHM em staking, obtendo recompensas de ajuste de base e removendo a oferta de tokens do mercado, beneficiando a próprio staker e a holders de OHM.

### Geist Finance
Um protocolo descentralizado de empréstimos.

## Prós e Contras

### Prós

### Contras

## Fantom e o Mercado
### Quantas Moedas Fantom (FTM) Há em Circulação
FTM é um token proof-of-stake (PoS) que existe em várias frentes.

A compatibilidade da plataforma com o Ethereum significa que usuários podem comprar FTM no padrão ERC-20, que é automaticamente convertido ao nativo FTM, uma vez que for recebido na carteira. Outra versão do FTM está disponível na Binance Chain usando o padrão BEP2. Apenas o FTM nativo pode ser utilizado na própria mainnet OPERA do Fantom.

O fornecimento total de FTM é de 3,175 bilhões de tokens, dos quais, 2.134.638.448 FTM estão em circulação no momento. O resto será liberado de acordo com um cronograma até 2023.

Os Staking são uma parte importante do tokenomics, sendo uma parte do suprimento reservado especialmente para recompensas de staking para os usuários que possuem FTM.

### Onde Comprar Fantom (FTM)
O token do Fantom, o FTM, é livremente negociado e pode ser encontrado nas maiores corretoras como a Binance, Gate.io e OKEx Korea.

O FTM existe em diversos protocolos, como ERC-20, BEP2 e, o do próprio Fantom, OPERA, todos com tokens em circulação.

Se você é novo em criptomoedas e quer saber mais sobre como comprar Bitcoin (BTC) ou outros tokens, confira primeiro esta informação.
