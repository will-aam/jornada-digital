# Como funciona a internet?

A Internet é um sistema global de redes de computadores interligadas que utilizam um conjunto próprio de protocolos, conhecido como _Internet Protocol Suite_ ou **TCP/IP**, com o objetivo de servir gradualmente usuários no mundo inteiro. É uma vasta coleção de redes interconectadas (_interconnected networks_), uma rede de várias outras redes, composta por milhões de empresas privadas, públicas, acadêmicas e governamentais, ligadas por uma ampla variedade de tecnologias de rede eletrônica, sem fio e ópticas.

Compreender o funcionamento da Internet requer a análise de sua infraestrutura física, a hierarquia de suas redes, os mecanismos de transmissão de dados e os protocolos que governam essa comunicação.

## Sumário

- [Conceitos Fundamentais e Arquitetura da Internet](#i-conceitos-fundamentais-e-arquitetura-da-internet)
- [Infraestrutura Física e Conectividade](#ii-infraestrutura-física-e-conectividade)
- [Transmissão de Dados: Pacotes e Protocolos](#iii-transmissão-de-dados-pacotes-e-protocolos)
- [Provedores de Serviço de Internet (ISPs)](#iv-provedores-de-serviço-de-internet-isps)
- [Serviços Oferecidos e Segurança](#v-serviços-oferecidos-e-segurança)

---

## I. Conceitos Fundamentais e Arquitetura da Internet

A Internet não tem um centro de controle. Em vez disso, ela é um sistema de **redes distribuídas**, o que significa que não depende de nenhuma máquina individual. Essa natureza distribuída garante sua **resiliência**; se um servidor, um _data center_ inteiro ou uma região de _data centers_ ficarem inativos, o resto da Internet pode continuar funcionando, ainda que mais lentamente.

No seu nível mais básico, uma **rede** é um grupo de computadores conectados capazes de enviar dados uns aos outros, comparável a um círculo social que troca informações. A Internet é a rede que conecta todas essas redes.

### Origens e Evolução

As origens da Internet remontam a uma pesquisa encomendada pelo governo dos Estados Unidos na década de 1960 (início da pesquisa) para construir uma forma de comunicação robusta e sem falhas através de redes de computadores. Essa pesquisa levou à criação de redes precursoras como a **ARPANET**, que foi a base para o desenvolvimento de protocolos de interconexão de redes (_internetworking_). O conceito de uma rede mundial de redes TCP/IP totalmente interligadas, chamada Internet, foi introduzido em 1982, abrangendo cerca de **22 anos**, marcando a transição da tecnologia militar e acadêmica para o modelo que se expandiria globalmente. A rede em si evoluiu em meados da década de 1980, e a sua comercialização total ocorreu nos Estados Unidos em 1995, quando a NSFNET foi desmantelada.

A sustentação técnica e a padronização dos protocolos de núcleo (IPv4 e IPv6) é uma atividade da **Internet Engineering Task Force (IETF)**.

---

## II. Infraestrutura Física e Conectividade

A conexão entre dispositivos e sistemas de computador é realizada através de um conjunto de protocolos padronizados. Fisicamente, a Internet consiste em roteadores, mídias (como cabeamento e links de rádio), repetidores e modems. A internet é simplesmente um **fio** enterrado no chão, que pode ser de fibra ótica, cobre, ou transmitido para satélites ou por redes de celular.

### O Papel Crítico dos Cabos Submarinos

Os cabos submarinos são as **artérias principais da Internet e da conectividade global**. Atualmente, **99% das telecomunicações mundiais** são realizadas por meio dessas infraestruturas ocultas sob o oceano. Eles atravessam o planeta em sua totalidade e transmitem rapidamente grandes quantidades de dados.

### Meios de Acesso e Velocidade

Os computadores se conectam à Internet através de fios, cabos, ondas de rádio e outros tipos de infraestrutura. Todos os dados enviados são traduzidos em **pulsos de luz ou eletricidade**, chamados "bits".

As taxas de transferência de dados e as características físicas das conexões variam muito. Quanto mais bits puderem passar pelos fios e cabos por vez, mais rapidamente a Internet funcionará. Métodos comuns de acesso incluem:

- **Banda Larga Fixa:** Um tipo de conexão à rede com capacidade superior à conseguida via conexão discada, geralmente permanente e não comutada, com mais de 100 Kbps (embora o limite seja variável).
- **Fibra Óptica:** Oferece **alta capacidade de largura de banda** (como gigabytes por segundo) e a **menor latência**. O uso de fibra excedeu 30% das assinaturas de banda larga em muitos países em 2021.
- **Wi-Fi e Banda Larga Móvel:** O Wi-Fi fornece acesso sem fio através de redes locais. A banda larga móvel utiliza tecnologias de acesso sem fio de longa distância, como 3G e 4G.
- **Conexão Discada:** Conexão comutada, realizada por meio de um modem analógico e linha telefônica.

---

## III. Transmissão de Dados: Pacotes e Protocolos

O funcionamento da Internet baseia-se em dois conceitos principais: **pacotes** e **protocolos**.

### 1. Comutação de Pacotes

A Internet funciona usando uma técnica chamada **comutação de pacotes**.

- **Pacote (Packet):** É um pequeno segmento de uma mensagem maior, ou um Datagrama. Quando os dados são enviados, eles são primeiro divididos em pacotes menores, que são traduzidos em bits.
- **Cabeçalho:** Cada pacote contém dados e informações sobre esses dados, conhecidas como "cabeçalho", que fica na frente para que a máquina receptora saiba o que fazer com o pacote.
- **Roteamento e Reorganização:** Os pacotes são encaminhados ao seu destino por vários dispositivos de rede, como roteadores e switches. Um arquivo ou imagem é quebrado em vários pedacinhos, que podem passar por **vários caminhos diferentes** e em tempos diferentes. No destino, o dispositivo receptor **monta novamente os pacotes na ordem correta** para usar ou exibir os dados.

O envio de informações digitais em partes menores (pacotes) é extremamente rápido. A comutação de pacotes é crucial porque evita que uma única conexão domine a rede, permitindo que roteadores e switches intermediários processem pacotes de forma independente.

Sim, o seu entendimento está **absolutamente correto**: a comutação de pacotes é a técnica fundamental que permite à Internet ser altamente **eficiente** e **resiliente** (resistente a falhas).

A Internet foi projetada para funcionar com base em dois conceitos principais: **pacotes** e **protocolos**.

### Analogia para fixação: O Transporte de uma Obra de Arte

Imagine que você precisa enviar a **Estátua da Liberdade** da França para Nova York.

**Cenário Antigo (Sem Comutação de Pacotes):**

Se a comunicação funcionasse como uma linha telefônica antiga (comutação de circuitos), você teria que reservar um **único navio gigante (um circuito dedicado)** para transportar a estátua inteira, de uma só vez.

1.  **Ineficiência:** O navio seria muito lento e ocuparia o único canal disponível no oceano. Nenhuma outra mercadoria ou navio prioritário poderia usar essa rota até que a estátua chegasse ao destino. O custo seria proibitivo, e o tráfego marítimo (a "Internet") seria bloqueado por minutos ou horas.
2.  **Falta de Resiliência:** Se o navio batesse em um iceberg (uma falha de rede) ou ficasse preso no Porto (congestionamento), **toda a sua remessa estaria perdida**, e a estátua nunca chegaria.

**Cenário Atual (Com Comutação de Pacotes):**

A Internet funciona como um sistema que exige que você **divida a estátua em milhares de caixas pequenas (os pacotes)**.

1.  **Divisão e Roteamento (Eficiência e Resiliência):** Você coloca um **endereço de destino** e **instruções de remontagem (o cabeçalho)** em cada caixa. Essas caixas são enviadas por centenas de **rotas diferentes** (navios, aviões, trens) e **em tempos diferentes**.
2.  **Resiliência na Prática:**
    - Se um navio que transporta 50 caixas for lento ou tiver um problema, as outras 950 caixas já estarão a caminho em rotas rápidas e alternativas, **chegando rapidamente ao destino**. O roteamento desviou o problema.
    - Se uma caixa se perder completamente, o sistema nota a falta e **pede apenas que aquela pequena caixa seja reenviada**, em vez de pedir para enviar a estátua inteira novamente.
3.  **Remontagem Rápida (Eficiência):** No destino final, os trabalhadores (seu computador) recebem as caixas, leem as instruções (o protocolo) e **montam a estátua de volta na ordem correta**.

Ao dividir a mensagem em pacotes e permitir que eles viajem por múltiplos caminhos, a Internet **maximiza o uso da infraestrutura** (eficiência) e **garante que a falha de um caminho não interrompa o serviço inteiro** (resiliência).

### 2. O Conjunto de Protocolos TCP/IP

O conjunto de protocolos da Internet (TCP/IP) define como a informação é trocada entre dispositivos e garante que os dados sejam transmitidos de forma confiável e segura.

A arquitetura do TCP/IP é ordenada em um conjunto de **quatro camadas conceituais**:

- **Camada de Aplicação (Nível mais alto):** Descreve a comunicação em termos apropriados para cada aplicação. É a camada mais próxima do usuário, responsável pelo acesso a e-mail, páginas web, mensagens instantâneas e videoconferência. Protocolos comuns incluem **HTTP, DNS, SMTP, FTP, SSH, Telnet, POP3, IMAP** e **TLS**.
- **Camada de Transporte:** Conecta aplicações em diferentes hosts através de um canal lógico, usando protocolos como **TCP** e **UDP**. O TCP/IP define como os processos de uma aplicação trocam mensagens entre si.
- **Camada de Rede (ou Internet):** Implementa o **Protocolo Internet (IP)**. O IP permite que os computadores se identifiquem e se localizem uns aos outros por meio do endereço IP e encaminhem seu tráfego através de redes intermediárias.
- **Camada de Enlace de Dados:** Conecta nós no mesmo link físico e contém protocolos que não necessitam de roteadores para travessia, como Ethernet e Wi-Fi.

#### O Processo de Estabelecimento da Conexão (Handshake TCP)

O TCP (Protocolo de Controle de Transmissão) é um dos protocolos que operam na camada de transporte do conjunto TCP/IP. Ele é fundamental para a comunicação confiável na Internet.

O fato de o TCP ser **orientado à conexão** significa que uma conexão deve ser estabelecida entre os dois dispositivos (cliente e servidor) antes que os dados possam ser trocados.

Este processo de pré-conexão é chamado de **"handshake TCP"**. Ao tentar carregar uma página web, o navegador, após resolver o DNS, inicia uma conexão com o endereço IP, realizando este _handshake_ TCP.

Para estabelecer essa comunicação confiável e ordenada, o TCP utiliza um **protocolo de enlace de três vias**.

Durante o processo de estabelecimento da conexão, os dispositivos também negociam vários parâmetros, como o tamanho máximo do segmento (_maximum segment size_) e o tamanho da janela (_window size_), que definem como os dados serão transmitidos através da conexão.

### Analogia: O Acordo de Envio de Mercadorias

Para entender por que o TCP precisa dessas três etapas antes de enviar dados, podemos usar uma analogia de comunicação e transporte, semelhante àquela que descrevemos anteriormente, mas focando agora no **acordo inicial** em vez do transporte dos pacotes em si:

Imagine que você (o **Cliente** ou Dispositivo A) precisa enviar uma mensagem muito importante e longa (os **Dados**) para um depósito em Nova York (o **Servidor** ou Dispositivo B). Como a mensagem será dividida em pacotes, você precisa garantir que o depósito esteja pronto, que ambos concordem com as regras e que a mensagem não se perca.

**As três etapas do Handshake TCP funcionam assim:**

| Etapa                                                       | Ação na Analogia (Protocolo)                                                                                                                                                    | Propósito (Confiabilidade)                                                                                                                |
| :---------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Pedido de Sincronização (SYN)**                        | O cliente (Você) telefona para o depósito e diz: **"Olá! Quero enviar uma remessa grande. Você está pronto para receber?"** (Envia um pacote SYN).                              | O cliente inicia a tentativa de conexão. É uma verificação para saber se o servidor está acessível e pronto para conversar.               |
| **2. Reconhecimento e Resposta de Sincronização (SYN-ACK)** | O depósito (Servidor) responde: **"Sim, estou pronto para receber! E, para ter certeza de que você me ouviu, você também está pronto para enviar?"** (Envia um pacote SYN-ACK). | O servidor confirma o recebimento do pedido (ACK) e, ao mesmo tempo, envia sua própria solicitação de sincronização (SYN) para o cliente. |
| **3. Confirmação Final (ACK)**                              | O cliente (Você) confirma: **"Sim, recebi sua confirmação. Vamos começar a enviar as caixas (pacotes) agora."** (Envia um pacote ACK).                                          | O cliente confirma o recebimento do SYN-ACK do servidor, finalizando o estabelecimento da conexão.                                        |

**Conclusão da Analogia:**

Somente após esta "conversa" inicial de três vias (_three-way handshake_), que estabeleceu que ambos os lados estão disponíveis e concordaram em se comunicar (conexão estabelecida), é que os dados reais da mensagem podem ser divididos em segmentos e transmitidos de forma confiável pelo TCP.

Isso garante que o TCP ofereça uma **comunicação confiável** e **ordenada**, em contraste com o protocolo **UDP** (User Datagram Protocol), que é "sem conexão" e não confiável (não faz essa checagem inicial).

### 3. Roteamento e Endereçamento

O **roteamento** é a principal função da camada de rede (IP).

#### Endereços IP e DNS

Servidores não possuem nomes, mas sim **números** (Endereços IP). Um **Endereço IP** é um identificador único atribuído a cada dispositivo na rede, usado para rotear dados ao destino correto.

- **IPv4:** Define um endereço IP como um número de 32 bits, a versão dominante usada na primeira geração da Internet, capaz de endereçar aproximadamente 4,3 bilhões de hosts. O esgotamento dos endereços IPv4 começou em 2011.
- **IPv6:** Usa 128 bits para o endereço IP e foi desenvolvido para fornecer capacidades de endereçamento muito maiores e roteamento mais eficiente. Sua implantação está em andamento desde meados dos anos 2000.

Como os usuários digitam nomes de domínio, o **Domain Name System (DNS)** é o responsável por traduzir esses nomes (como _instagram.com_) em endereços IP. Esse processo é chamado de **DNS lookup**. O DNS também ajuda os sites a carregarem mais rápido ao direcionar o tráfego para servidores próximos.

#### Roteadores e Sistemas Autônomos (AS)

A arquitetura de roteamento é baseada em **Sistemas Autônomos (AS)**. Um AS é uma rede de redes independentes, cada uma com administração autônoma.

- **Roteadores (Routers):** Dispositivos que compõem o núcleo da Internet. Eles examinam os pacotes e os encaminham para o próximo roteador no caminho para o destino. Os roteadores usam **tabelas de roteamento** preenchidas por protocolos específicos para decidir a rota.
- **Núcleo (_Core_) e Borda (_Edge_):** As redes na **borda** são aquelas que se conectam à Internet, enquanto o **núcleo** contém a infraestrutura da Internet. Roteadores do núcleo mantêm informações completas sobre seus próprios destinos e sobre como chegar aos núcleos dos demais destinos.
- **Roteamento Interno (dentro de um AS):** Usa protocolos como **RIP** e **OSPF**. O OSPF (_Open Shortest Path First_) implementa o **Algoritmo de Dijkstra**, que precisa da topologia completa da rede para determinar o caminho mais curto.
- **Roteamento Externo (entre ASes):** Usa o protocolo **BGP** (_Border Gateway Protocol_). Entre Sistemas Autônomos, não se divulga a topologia, apenas os destinos alcançáveis e o custo.

---

## IV. Provedores de Serviço de Internet (ISPs)

Um Provedor de Serviços de Internet (ISP) é uma organização que oferece serviços para permitir que os usuários **acessem e usem a internet**. Eles atuam como **gateways** que fornecem acesso à rede, geralmente mediante uma taxa.

### Hierarquia de ISPs

Os ISPs trabalham em camadas para fornecer acesso:

1.  **Tier 1 ISP:** O nível mais alto, com acesso a toda a rede da internet através de acordos de interconexão, conectando todos os cantos.
2.  **Tier 2 ISP:** Compra acesso da rede Tier 1 e pode vendê-lo para o próximo nível ou para usuários finais.
3.  **Tier 3 ISP:** Compra largura de banda de um ISP de nível superior (Tier 2) e a vende aos usuários finais.

Para estabelecer a conectividade, o usuário final precisa de um **modem** e uma conta ativa. Após a verificação da conta, o ISP atribui um endereço IP exclusivo ao modem, concedendo acesso à Internet.

---

## V. Serviços Oferecidos e Segurança

A Internet carrega muitos aplicativos e serviços, sendo o mais proeminente a World Wide Web.

### World Wide Web (WWW)

A World Wide Web é apenas um dos muitos serviços que funcionam dentro da Internet. É uma coleção global de documentos, imagens, multimídia e outros recursos logicamente inter-relacionados por **hiperlinks** e referenciados com **URLs** (_Uniform Resource Locators_). O **Hypertext Transfer Protocol (HTTP)** é o principal protocolo de acesso da Web.

### Correio Eletrônico

O e-mail é um serviço de comunicação fundamental disponível através da Internet. Hoje, o número de mensagens trocadas por e-mail já superou o número de cartas do correio convencional, transformando-se em uma forma de comunicação informal e acessível.

### Segurança e Criptografia

A comunicação na Internet exige requisitos básicos de segurança, como:

- **Identificação e Autenticação:** Permite que uma entidade (pessoa, empresa, programa) se identifique e verifique se ela é quem realmente diz ser. Contas e senhas são o principal mecanismo de autenticação.
- **Integridade:** Protege a informação contra alteração não autorizada.
- **Confidencialidade ou Sigilo:** Protege a informação contra acesso não autorizado.

A **criptografia** é um dos principais mecanismos de segurança.

- **HTTP vs. HTTPS:** O protocolo HTTP transmite informações em **texto claro** (sem criptografia) e não é indicado para dados sigilosos, como senhas e dados bancários. Deve ser substituído pelo **HTTPS** (_Hypertext Transfer Protocol Secure_), que é uma versão criptografada do HTTP e oferece conexões seguras.
- **SSL/TLS:** Os protocolos _Secure Sockets Layer_ (SSL) e _Transport Layer Security_ (TLS) são usados para fornecer comunicação segura pela Internet. O uso de um **Certificado Digital** (que associa uma chave pública a uma entidade) é fundamental para garantir a conexão segura.

---

Para consolidar a compreensão do fluxo de dados, podemos imaginar a Internet como um **sistema de correios global altamente eficiente**:

Quando você envia uma mensagem (dados), ela é primeiro quebrada em **milhares de cartas pequenas (pacotes)**, e o endereço do remetente e do destinatário (IPs) e as instruções de remontagem (cabeçalhos) são colocados em cada uma. Os **provedores de Internet (ISPs)**, organizados em uma hierarquia (Tier 1 a Tier 3), são as grandes companhias de transporte. Essas cartas são então enviadas através de **autoestradas complexas (cabos de fibra ótica, incluindo os submarinos)**. Em cada **cruzamento (roteador)**, o pacote é lido para saber o próximo passo (roteamento), utilizando um mapa gigantesco (tabela de roteamento mantida por protocolos como BGP e OSPF). Finalmente, todas as cartas chegam ao seu destino, e o computador receptor atua como um carteiro dedicado, remontando as cartas na ordem correta para recriar a mensagem original. Se você está visitando um site, é como procurar o endereço de uma loja em uma **agenda telefônica universal (DNS)** antes que as cartas possam começar a viajar.

<details>
<summary> <h3>Notas </h3></summary>

- [Submarine Cable Map](https://www.submarinecablemap.com/)
- [Internet - Wiki](https://pt.wikipedia.org/wiki/Internet)
- [Camada de aplicação](https://pt.wikipedia.org/wiki/Camada_de_aplição)
- [Como a Internet funciona? - Gustavo Guanabara](https://www.youtube.com/watch?v=nlO5hySqJFA)
- [Como a internet funciona em 5 minutos (en-Us) - Aaron Titus ](https://www.youtube.com/watch?v=7_LPdttKXPc)
- [TCP/IP (PDF)](https://elhacker.info/manuales/Redes/Redes%20paso%20a%20paso/Modelo%20TCP.pdf)
- [Redes de Computadores II - Roteamento na InterneT (PDF)](https://www.inf.ufpr.br/elias/redes/23aulaRedes.pdf)
  </details>
