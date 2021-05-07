# Aplicação Empréstimo 
---

> # Problema

### Gerar eventos de empréstimos utilizando arquitetura Event Driven e posteriormente armazenar em uma plataforma de mensagens. 

 <br>

> # Solução
### Dividir o modelo de negócio em dois microsserviços: um que gera os eventos de negócio e outro que verifica com base em uma regra de négocio a concessão ou rejeição do empréstimo. Tecnologia utilizada para escrever os microsserviços:  Spring Cloud Stream e as plataformas de mensagens RabbitMQ e Apache Kafka.[01]



<br>
<br>

## Componentes da Solução 


[01] - Componentes da Solução

<br>

## Microsserviço Fonte de Empréstimo 

<br>
<br>
<br>

![<--](./app/produtor.png)
[02] - Microsserviço LoanSource

<br>


## Microsserviço Verificador de Empréstimo

<br>
<br>

![<--](./app/consumidor.png)
[03] - Microsserviço LoanCheck

<br>




### Links de referência

[01] https://github.com/benwilcock/spring-cloud-stream-demo/blob/master/docs/index.md "Simple Event Driven Microservices with Spring Cloud Stream"
<br>
[02] Diagrama de Componentes da aplicação e infra estrutura utilizada.
<br>
[03] Diagrama de Sequência da aplicação produtora de eventos com os componentes do microsserviço e anotações Spring Cloud Stream.
<br>
[04] Diagrama de Sequência da aplicação consumidora de eventos com os componentes do microsserviço e anotações Spring Cloud Stream.