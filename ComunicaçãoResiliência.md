## Comunicação e Resiliência

### Síncrona
    - Faz uma requisição, você necessita da resposta de forma imediata.(REST)
    - Os envolvidos precisam estar  online.
    - Em determinados contextos, a comunicação síncrona custa mais caro.
    - Se o servidor estiver fora, há possibilidade de perda de dados.

### Assíncrona
    - As duas pontas não precisam estar conectadas ao mesmo tempo para trocar informações.
    - A mensagem foi enviada.
    - Demora... (Ser uma analise de negócio do que é aceitavel ou não)


### Síncrona (Protocolos)
    - Rest / HTTP
    - gRPC
    - Streams - Bidirecional
    - GraphQL

### Assíncrona (Protocolos e Ferramentas)
    - Filas, Topicos
    - Pub/Sub Produtor da mensagem -> Subscriber(s) (Interessado naquela mensagem)
    - Apache Kafka (Topicos) -> Grupos de consumidores ficam "ouvindo" o Topicos
    - Redis
    - Postgres
    - Filas
    - Exchange (Hub de roteamento de mensagens)
    - RabbitMQ

## Real Time
    - Websockets
    - Bidirecional (Client e o server conseguem enviar mensagens)
    - HTTP -> Upgrade -> TCP
    - Chat, Troca de mensagens...
    - Server-Sent Events (SSE)
    -- Comunicação em tempo real UNILATERAL
    -- Dashboard, notificações...

### Protocolos / Payload
    - Protocol Buffers (Protobuf)
    -- Google
    -- .proto (Evolutivo)

    - FlatBuffers
    -- Google
    -- Não há desserialização na leitura
    -- Offsets e os dados
    -- .fbs
