<div name="readme-top">
    <h1 align=center>BLOCKCHAIN</h1>
</div>

<details>
    <summary><span>📌 Índice</span></summary>

- [Conceitos da Tecnologia ***BLOCKCHAIN***](#conceitos-da-tecnologia-blockchain)
  - [Blocos](#blocos)
  - [Mineração](#mineração)
  - [Node](#node)
- [Início da Blockchain: ***CRIPTOMOEDAS***](#início-da-blockchain-criptomoedas)
- [Whitepaper do ***BITCOIN***](#whitepaper-do-bitcoin)
- [Fundamentação Tecnológica ***BLOCKCHAIN***](#fundamentação-tecnológica-blockchain)
  - [***Hash***](#hash)
- [Criptografia de ***Chave Pública***](#criptografia-de-chave-pública)
- [Formação de Blocos](#formação-de-blocos)
- [Encadeamento](#encadeamento)
- [Plataforma ***BLOCKCHAIN***](#plataforma-blockchain)
  - [Rede ***Peer-to-Peer Blockchain***](#rede-peer-to-peer-blockchain)
- [Algoritmo de Consenso](#algoritmo-de-consenso)
  - [Fundamentos do Consenso](#fundamentos-do-consenso)
  - [Como os Algoritmos Comuns Implementam o Consenso](#como-os-algoritmos-comuns-implementam-o-consenso)
  - [Prova de Trabalho](#prova-de-trabalho)
  - [Prova de Participação](#prova-de-participação)
- [Ataque de 51%](#ataque-de-51)

</details>

# CONCEITOS DA TECNOLOGIA *BLOCKCHAIN*

**Blockchain** é definida de forma simples como um **livro-razão** descentralizado e distribuído que registra a 
rastreabilidade de um ativo digital. Desde a sua criação, os dados em uma blockchain não podem ser modificados e 
excluídos.

Um dos grandes problemas que a blockchain nasceu para resolver foi o **gasto duplo**. Não é possível enviar o mesmo
ativo para duas pessoas, algo que pode acontecer dentro de um banco de dados, dependendo da arquitetura com que ele foi 
criado.

Há algumas coisas que podem dar errado quando você tenta enviar um ativo digital para duas pessoas ao mesmo tempo.

- Algo pode ter dado errado no banco de dados (problema técnico).
- A conta do remetente pode ter sido hackeada
- Os limites de transferência do dia podem ter sido excedidos
- Debitado de uma conta, nunca creditando no outro lado
- Problemas com dados

![img.png](assets/img/img1.png)

<details close>
    <summary><code>IMAGEM | Como a blockchain funciona</code></summary>

1. **A** quer enviar dinheiro para **B**
2. A transação é representada online como um "bloco"
3. O bloco é transmitido para cada participante na rede
4. As pessoas na rede atestam se a transação é válida
5. O bloco é então adicionado à cadeia, o que confere um registro idôneo (adequado) e transparente nas transições
6. O dinheiro é movido de **A** para **B**

</details>

Todas essas transações são armazenadas na estrutura de **livro-razão** digital. Funciona como uma planilha contendo 
todos os inúmeros nós de uma rede e tem o histórico de todas as compras feitas por cada nó. As informações contidas no
livro digital são altamente seguras e a assinatura digital protege contra adulterações.

Qualquer um pode ver os dados do livro-razão, mas ninguém pode corrompê-los. Só é possível inserir informações na 
blockchain, não é possível deletar nem alterar o dado que outro participante já inseriu.

> De forma geral:
> 
> - Blockchain é um banco de dados que armazena blocos de dados criptografados e os encadeia para formar uma única fonte
de verdade cronológica para os dados.
> - Os ativos digitais são distribuídos em vez de copiados ou transferidos, criando um registro imutável de um ativo.
> - O ativo é descentralizado, permitindo acesso total em tempo real e transparência ao público.
> - Um registro transparente de alterações preserva a integridade do documento, o que cria confiança no ativo.
> - As medidas de segurança inerentes ao Blockchain e o livro-razão público o tornam uma tecnologia primordial para
quase todos os setores.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Blocos

Um bloco consiste em uma lista de dados. Uma "cadeia" é um conjunto de cloco de dados que cresce constantemente ao longo
de um período de tempo. Se a transação estiver inserida na blockchain, será extremamente difícil ou impossível alterar 
esses dados. Isso torna a blockchain um meio único de armazenar dados valiosos.

Imagine uma torre digital de blocos, osbre a qual um novo bloco de dados é adicionado a cada 10 minutos a partir do 
"**bloco de gênese**" original na base da torre. Os dados em cada bloco consistem em transações financeiras transmitidas
por usuários da rede juntamente com evidências criptográficas de que essas transações são válidas.

A figura representa como os blocos são encadeados em uma blockchain:

![img.png](assets/img/img2.png)

<details close>
    <summary><code>IMAGEM | Encadeamento de blocos</code></summary>


Cada bloco contém dados de transações financeiras transmitidas por usuários da rede (na imagem, as ***Transactions***), 
juntamente com evidências criptográficas de que essas transações são válidas (na imagem, as ***Proof of Work*** e 
***Previous block***).

</details>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Mineração

Mineração é a extração da moeda digital usando equipamentos especiais (computadores potentes).

A mineração é a junção de blocos que armazenam informações sobre transações. Como resultado, eles formam uma cadeia 
contínua e consistente.

Para anexar um bloco, é necessário resolver um determinado problema matemático decifrando o algorítmo da criptomoeda.
Caso o equipamento encontre a resposta correta, seu dono recebe uma recompensa em forma de moedas digitais, ou seja,
recebe Bitcoin.

Quanto mais os mineradores buscam resolver o problema matemático, mais difícil é encontrar a resposta certa e o custo
aumenta.

![img.png](assets/img/img3.png)

<details close>
    <summary><code>IMAGEM | Processos</code></summary>

1. Verifica Transações
2. Agrupa transações válidas em um **bloco "candidato"**
3. Insere a **hash** do bloco mais recente no bloco candidato
4. Resolve a **proof-of-work** (PoW)
5. Anexa o bloco candidato em uma blockchain local 
6. Propaga a solução na rede
7. Espera a verificação da solução por outros **nodes**
8. Pegue a recompensa

</details>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Node

Termo utilizado para cada transação registrada cronologicamente e distribuída para uma série de dispositicos conectados.
Esses dispositivos são chamados de **nós** (***Node***). Esses nós se comunicam dentro da rede e transferem informações sobre 
transações e novos blocos.

É um componente crítico da infraestrutura blockchain. Ajuda a manter a segurança e a integridade da rede. O principal
objetivo de um nó blockchain é verificar cada lote de transações de rede, chamados de blocos. Cada nó é distinguido dos
outros por um identificador único.

![img.png](assets/img/img4.png)

<details close>
    <summary><code>IMAGEM | Nós</code></summary>

1. **Node** (membro da rede blockchain) envia um pedido de transação para a rede blockchain
2. Bloco criptografado é criado
3. Outros nodes validam a transação
4. Bloco adicionado à blockchain
5. Todos os nodes recebem o novo bloco

</details>

Existem basicamente quatro tipos de nós (***Node***) em uma rede blockchain:

|       Node       | Descrição                                                                                                                                                                                                                                                            |
|:----------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|  **Full Node**   | Executam a função de manter e distribuir cópias de todo o registro da blockchain, validando o histórico da blockchain e retransmitindo-o para outros nós da rede                                                                                                     |
| **Super Nodes**  | Operam 24 horas por dia para conectar os *full nodes* uns aos outros e espalhar a blockchain por toda a rede. Os *super nodes* servem como retransmissores de informações ou redistribuição para garantir que todos tenham a cópia correta da blockchain do Bitcoin. |
| **Light Nodes**  | Executam funções semelhantes aos *full nodes*, mas em uma capacidade menor. Eles contêm pequenas porções da blockchain em oposição à cópia inteira.                                                                                                                  |
| **Mining Nodes** | Resolvem problemas computacionais complexos usando hardware especializado por meio de "mineração", o processo de criação e adição de novos blocos à blockchain. Os mineradores bem-sucedidos recebem uma recompensa em Bitcoin por criar o novo bloco.               |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# INÍCIO DA BLOCKCHAIN: *CRIPTOMOEDAS*

Ao contrário do dinheiro, a criptomoeda usa a blockchain para atuar como um livro público e um sistema de segurança 
criptográfico aprimorado, para que as transações online sejam sempre registradas e protegidas. O apelo das criptomoedas 
é que tudo está registrado em um livro público e protegido por criptografia, fazendo um registro irrefutável, com 
carimbo de data/hora e um seguro de cada pagamento.

Alguns dos motivos pelos quais as criptomoedas estão sendo tão adotadas:

- A segurança da Blockchain torna o roubo muito mais difícil, pois cada criptomoeda tem seu próprio número identificável 
irrefutável que é anexado a um proprietário.
- A criptografia reduz a necessidade de moedas e bancos centrais individualizados - Com a blockchain, a criptografia 
pode ser enviada para qualquer lugar e qualquer pessoa do mundo sme a necessidade de troca de moeda ou interferência 
de bancos centrais.

> **Sobre o bitcoin**
> - Sua criação até hoje é um mistério.
> - Seu criador se intitula Satoshi Nakamoto. Nakamoto: é a pessoa ou pessoas que desenvolveram o bitcoin.
> - Eles são anônimos e usam pseudônimos.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# WHITEPAPER DO *BITCOIN*

Breve linha do tempo dos eventos mais importantes e notáveis no desenvolvimento da blockchain

<details close>
    <summary><code>2008</code></summary>

- Satoshi Nakamoto publica: "Bitcoin: A Peer to Peer Electronic Cash System".

</details>

<details close>
    <summary><code>2009</code></summary>

- A Primeira transação bem-sucedida de Bitcoin (BTC) ocorre entre o cientista da computação Hal Finney e Satoshi 
Nakamoto.

</details>

<details close>
    <summary><code>2010</code></summary>

- O programados Laszlo Hanycez, na Flórida, concluiu a primeira compra usando o Bitcoin - duas pizzas Papa John's. 
Haneycz pagou 10.000 BTC, cerca de US$ 60,00 na época. Hoje vale alguns milhões e a comunidade comemora esse dia como 
Bitcoin Pizza day..
- O valor do Mercado do Bitcoin excede oficialmente US$ 1 milhão.

</details>

<details close>
    <summary><code>2011</code></summary>

- 1 BTC = $ 1USD, dando a paridade da criptomoeda com o dólas americano
- Eletronic Frontier Foundation, Wikilieaks e outras organizações começam a aceitar Bitcoin como doações.

</details>

<details close>
    <summary><code>2012</code></summary>

- Blockchain e criptomoedas são mencionadas em programas de televisão populares como The Good Wife, injetando blockchain 
na cultura pop.
- A Bitcoin Magazine foi lançada por um dos desenvolvedores do BitCoin Vitalik Buterin.

</details>

<details close>
    <summary><code>2013</code></summary>

- O valor de mercado do BTC ultrapassou US$ 1 bilhão.
- O Bitcoin atingiu pela US$ 100/BTC pela primeira vez.
- Buterin publicou o artigo "Ethereum Project" sugerindo que a blockchain tenha outras possibilidades além do Bitcoin
  (por exemplo, contratos inteligentes)

</details>

<details close>
    <summary><code>2014</code></summary>

- A empresa de jogos Zynga, The D Las Vegas Hotel e Overstock.com começam a aceitar Bitcoin como pagamento.
- O Projeto Ethereum de Buterin é financiado por meio de uma Oferta Inicial de Moedas (ICO - Initial Coin Offering) 
arrecadando mais de US$18 milhões em BTC e abrindo novos caminhos para a blockchain.
- R3, um grupo de mais de 200 empresas de blockchain, é formado para descobrir noas maneiras de implementar blockchain 
em tecnologia
- PayPal anuncia integração com Bitcoin.

</details>

<details close>
    <summary><code>2015</code></summary>

- O número de comerciantes que aceitam BTC excede 100.00
- A NASDAQ e a empresa de blockchain de San Francisco Chain se unem para testar a tecnologia para negociar ações em 
empresas privadas.

</details>

<details close>
    <summary><code>2016</code></summary>

- A gigante da tecnologia IBM anuncia uma estratégia de blockchain para soluções de negócios baseadas em nuvem.
- O governo do Japão reconhece a legitimidade da blockchain e das criptomoedas.

</details>

<details close>
    <summary><code>2017</code></summary>

- Bitcoin atinge US$ 1.000/BTC pela primeira vez.
- O valor de mercado de criptomoedas atinge US$ 150 bilhões.
- O CEO do JP Morgan, Jamie Dimon, diz acreditar na blockchain como um tecnologia futura, dando ao sistema de 
 contabilidade um voto de confiança de Wall Street.
- O Bitcoin atinge seu máximo histórico em US$ 19.783,021/BTC
- Dubai anuncia que seu governo será movido à blockchain até 2020.

</details>

<details close>
    <summary><code>2018</code></summary>

- O Facebook se compromete a iniciar um grupo de trabalho em blockchain e sugere a possibilidade de criar sua própria
criptomoeda.
- A IBM desenvolve uma plataorma bancária baseada em, com grandes bancos como Citi e Barclays assinando. 

</details>

<details close>
    <summary><code>2019</code></summary>

- O presidente da China, Ji Xiping, abraça publicamente a blockchain, enquanto o banco central da China anuncia que está 
trabalhando em sua própria criptomoeda.
- O CEO do Twitter & Square, Jack Dorsey, anuncia que a Square contratará engenheiros de blockchain para trabalhar nos 
 uturos planos de criptomoedas da empresa.
- A bolsa de valores de Nova York (NYSE) anuncia a criação da Bakkt - uma empresa de carteira digital que inclui 
negociação de criptomoedas

</details>

<details close>
    <summary><code>2020</code></summary>

- Bitcin quase chega a US$ 30.000/BTC até o final de 2020.
- PayPal anuncia que permitirá que usuários comprem, vendam e mantenham criptomoedas.
- As Bahamas se tornam o primeiro país do mundo a lançar sua moeda digital do banco central, apropriadamente conhecida
como "Sand Dollar".
- Blockchain se torna um jogador chave na luta contra a COVID-19, principalmente para armazenar com segurança dados de
- pesquisas médicas e informações de pacientes.

</details>

<details close>
    <summary><code>2021</code></summary>

- O detentor corporativo nº 1 do Bitcoin é o Grayscale Bitcoin Trust. Eles detêm 654.885 Bitcoind, ou 3.12% da oferta 
total
- O detentor corporativo nº2 do Bitcoin é a MicroStrategy. Eles detêm 124.391 Bitcoins.
- Bitcoin tornou-se moeda legal ao lado do dólar americano em El Salvador.
- Existem 16.531 criptomoedas listadas no CoinMarketCap.com
- Houve 485.814 contratos de token criados no Ethereum.
- De acordo com o CoinATMRadar, existem 34.479 caixas eletrônicos criptográficos controlados por 603 operadores em 77 
países.
- A Coinbase abriu seu capital em 2021 e tem um valor de mercado (valor total de todas as ações) de US$ 60 bilhões, 39 
alcançaram esse nível em 2021.

</details>

[Whitepaper do ***Bitcoin***](https://bitcoin.org/bitcoin.pdf).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# FUNDAMENTAÇÃO TECNOLÓGICA *BLOCKCHAIN*



<p align="right">(<a href="#readme-top">back to top</a>)</p>

## *Hash*

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# CRIPTOGRAFIA DE *CHAVE PÚBLICA*

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# FORMAÇÃO DE BLOCOS

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# ENCADEAMENTO

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# PLATAFORMA *BLOCKCHAIN*

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Rede *Peer-to-Peer Blockchain*

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# ALGORITMO DE CONSENSO

<details close>
    <summary><code>VÍDEO | Consenso</code></summary>



</details>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Fundamentos do Consenso

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Como os Algoritmos Comuns Implementam o Consenso

<details close>
    <summary><code>VÍDEO | Blockchain: Ethereum</code></summary>



</details>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Prova de Trabalho

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Prova de Participação

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# ATAQUE DE 51%