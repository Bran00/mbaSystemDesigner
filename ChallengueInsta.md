## Orientações para a Entrega do Desafio - Insta

### Desafio de System Design: Insta
 O Objetivo deste desafio é projetar um sistema que atenda aos seguintes requisitos de engenharia, detalhando o que será abordado e  o que está fora do escorpo.

### Requisitos engenharia

#### Requisitos Funcionais
  - O usuário poderá criar novos posts com possibilidade de fazer upload de imagens e vídeos;
  - O usuário poderá seguir outros usuários e também ser seguido;
  - O usuário terá acesso ao feed com posts dos usuários que ele está seguindo.

#### Não será abordado
  - Stories;
  - Comentários;
  - Lives;
  - Busca;
  - Compartilhamento de posts para outros usuários;
  - Listagem de usuários que ele está seguindo;

#### Requisitos não funcionais
  - 100 milhões de usuários por dia (DAU);
  - Disponibidade > Consistência;
  - Latência de <  400ms para exibição do feed;
  - Baixa latência para exibição de imagens e vídeos;
  - O sitema deve operar de forma assíncrona, sempre que possível, para garantir resiliência e otimização de recursos.

#### Não será abordado:
  - Implementação de observalidade;
  - Processo de entrega de software;
  - Detalhes de infraestrutura (como uso de Kubernetes)
  - Procedimentos de recuperação em caso de falhas.

### Tarefas para complementar o System Design (Ferramentas recomendada: Excalidraw)
  - Identificar as principais entidades do sistema e suas relações;
  - Estimar as capacidades básicas de volume de requisições e storage;
  - Definir o design de API de alto nível com os principais endpoints e métodos;
  - Criar o diagrama visual com as interações dos componentes do sistema;
  - Considerar perguntas complexas que possam abordar:
    - Banco de dados;
    - Caching;
    - Fan out strategies;
    - Necessidade de mensageria;
    - Processos de upload;
    - Escalabilidade horizontal.

