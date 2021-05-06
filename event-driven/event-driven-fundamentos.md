<!--mdMenu-->
# Conceituação
---

> # O que são eventos?

> ## São operações concluídas dentro de um processo de negócio de uma organização. Eventos são uma forma de expor o domínio de negócio.

 

## Eventos
> ### "_There are two distinct Time Points that we should always consider: the time the event occurred and the time the system noticed the event._" - Martin Fowler



## Exemplo de Eventos

* Eventos - Cenário 1
  
  * Benefício indeferido
    * Carta de indeferimento enviada

  
* Eventos - Cenário 2
  
  * Passagem aérea emitida
  * Check-In realizado
    * Notificado passageiro o portão de embarque
  * Vôo cancelado
    * Notificado passageiro
  
<br>

### Objetivos da Arquitetura Event-Driven  

1. Colaborar os *eventos* aos recursos computacionais.
2. Estabelecer a comunicação entre recursos ou serviços por meio de *eventos*.
3. Armazenar os *eventos*
4. Monitorar os *eventos*
   


### A origem dos eventos podem ser de diferentes _*fontes*_.
![<--](http://localhost:8090/event-driven/images/fontes.png)

[01] - Origem de eventos

<br>

# Quais os motivos para se tornar uma empresa Orientada a Eventos?

1. Tornar o sistema mais responsivo
2. Real Time
3. Escalonável

## Fatores que estagnam e impedem a inovação e a transformação 

1. **Sistema rígido e interações complexas**
   1. Alto acoplamento
   2. Baixa granularidade
   3. Processos difícies de serem modificados
2. **Dados desatualizados**
   1. Pode ser consequência de uma replicação de informações em vários sistemas
3. **Respostas lentas**
   1.  Pode ser consequência do uso de uma operação orientada por lote
   

## 3 (Três) etapas que facilitam as operações de uma empresa orientadas a evenots: 



1. **Habilitar os sistemas existentes para responder a eventos**
   1. Ouvir
   2. Agir
   3. Reagir


2. **Modernizar sua plataforma**
   1. Suportar streaming de eventos


3. **Alertar e informar**
   1. Partes interessadas internas e externas
      1. Funcionários 
      2. Clientes  
      3. Parceiros

<br>
<br>
<br>

![<--](http://localhost:8090/event-driven/images/enterprise.png)
[02] - 3 etapas para se tornar uma empresa orientada a eventos 

<br>


<a name="ancora"></a>
# Fundamentos
<br>

  - [Tipos de Comunicação](#ancora1)
  - [Estrutura de um Evento?](#ancora2)
  - [Estrutura da comunicação de uma Arquitetura Event-Driven](#ancora3)
  - [Abordagem Mensagens e Eventos](#ancora4)


<a id="ancora1"></a>

# Tipos de Comunicação 
<br>

***SÍNCRONA***

![<--](http://localhost:8090/event-driven/images/desenv.png)

<br>

***ASSÍNCRONA***

![<--](http://localhost:8090/event-driven/images/desenv.png)

***HÍBRIDA***

![<--](http://localhost:8090/event-driven/images/desenv.png)

[Topo](#ancora)<a id="ancora1"></a>

<br>

<a id="ancora2"></a>

# Estrutura de um Evento?
![<--](http://localhost:8090/event-driven/images/desenv.png)
  
[Topo](#ancora)<a id="ancora2"></a>

<br>

<a id="ancora3"></a>

# Estrutura da comunicação de uma Arquitetura Event-Driven

<br>

## ***CONSUMIDORES X PRODUTORES***

### O elemento central da comunicação de uma arquitetura orientada a eventos, seria o padrão _**Publish-Subscriber Chanel**_ . Publisher/Subscriber possui forte ligação com a integração de _aplicações_ e _serviços_.

> Define a forma como a mensagem trafega no sistema. Este padrão é usado amplamente nos sistemas comercias de código aberto

<br>
  
![<--](http://localhost:8090/event-driven/images/pub_sub0.png)

[03] - Emissor transmite ou empurra um evento a todos os receptores interessados


<br>

## - Os **produtores e consumidores** de eventos são autônomos para definir sua modelagem/arquitetura

### Estabelecem comunicação por meio de uma ASSINATURA.

1. *Definem a sua **tecnologia***


2. *Comunicam-se por meio de um **barramento***
![<--](http://localhost:8090/event-driven/images/pub_sub1.png)

[04] - Dois consumidores de um tópico de eventos, utilizam o modelo **_push/pull_** (empurrar/puxar).


### ***TIPOS DE COMUNICAÇÃO DOS EVENTOS***:
 Podem assumir três tipos:
  * One-To-Many (Fan-Out)
  * Many-To-One (Fan-In)
  * Many-To-Many

<br>

### ***FLUXO DE EVENTOS*** 
> Base de comunicação para todos os sistemas

1. **Transformações** dos tópicos de eventos, por meio de um pipeline  de serviços.

![<--](http://localhost:8090/event-driven/images/pipeline.png)

[05] - Os estágios intermediários trabalham com o padrão publishe/subscriber

2. **Agregações** de tópicos de eventos
   
![<--](http://localhost:8090/event-driven/images/agregacoes.png)

[06] - Processamento de tópicos ou fluxos de eventos e sua posterior agregação.

<br>


[Topo](#ancora)<a id="ancora3"></a>



<a id="ancora4"></a>

## Abordagem Mensagens e Eventos
![<--](http://localhost:8090/event-driven/images/desenv.png)
  
[Topo](#ancora)<a id="ancora4"></a>




### Links de referência

[01] https://www.youtube.com/watch?v=MjEam95VLiI "What is Cloud Pub/Sub?"
<br>
[02] https://solace.com/blog/becoming-an-event-driven-enterprise/ "3 Steps to Becoming an Event-Driven Enterprise"
<br>
[03] https://docs.wso2.com/display/EIP/Publish-Subscribe+Channel "Publish-Subscribe Channel"
<br>
[04][05][06] https://ichi.pro/pt/apache-kafka-em-poucas-palavras-96218812096507 "Apache Kafka em poucas palavras"