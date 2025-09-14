##                              SYSTEM DESIGN

### Requisitos de Engenharia:
- Requisitos funcionais:
    - Passageiro / Cliente ele solicita uma nova corrida a partir de uma localização e um destino;

- Requisitos não funcionais:
    - Baixa latência ??? O que é baixa latência no contexto desse projeto;
    - Disponibilidade do sistema? SLA;
    - Disponibilidade vs Consistência;

### Plano de capacidade
    - Quantidade usuários Ativos;
    - Pico de Utilização;
    - Escrita Intensiva vs Leitura Intensiva;
    - Quanto de trafégo é gerado em média por usuário;
    - Armazenamento: (Quantos TB em 1 ano, 1 dia, 5 anos, etc)

### Entidades Relacionadas / core
    - Substantivos Relacionados aos requisitos funcionais;
    - Ex: Passageiro, corrida, localização (origem, destino);

### Design de API:
    - POST /rider/request-ride
    {
      riderID, [obs]: Pode ser trocado por um token na url que identifica o rider
      location,
      destination
    }

### System Design (High Level View / WhiteBoard)

Rider -> |request ride| -> Api Gateway -> RiderMatcher(Rider - Driver)

### Aprofundamento
    - Qual tipo de banco de dados usar?
    - Como garantir resiliência (Register Ride estiver fora do ar?) Por quanto tempo eu devo cancelar a ride?
    - Como funciona a API Gateway? Quais serviços ela vai utilizar? Aponte 3 "marcas" de API Gateway
