# Live Chat
Um mine chat para pessoas poderem se comunicarem em tempo real

### Propósito (Estudo)
Contrui essa aplicação para adquirir conhecimento de WebScoket.

Com o WebSocket, conseguimos manter uma conexão biderecional em tempo real.

Como funciona o fluxo utilizando o WebSocket com STOMP:
 - O front-end se conecta na url do Websocket
 - se inscreve em um tópico para poder recebe a mensagem desse tópico
 - Agora ele envia mensagem para o endpoint que recebe a messagem
 - o endpoit captura a mensagem e envia para o tópico
 - todos que estiverem inscritos nesse tópico receberão a mensagem
 - com essa mensagem recebidada do servidor o frontend renderiza ela no chat

## Tecnologias
- Java 21
- Spring Boot
- Spring Boot Starter Websocket
- Websocket
- STOMP

## Template

![testes](https://github.com/Jeff-bt/livechatms/blob/main/weebSocket_layout.png)

## Como iniciar o projeto

### Pré-requisitos
  - Java 17

### Clona

- Clone o projeto com o comando:
  
  ```
    https://github.com/Jeff-bt/livechatms.git
  ```

### Configura

 - Navegue para pasta `/livechatms`:

   ```
      cd livechatms
   ```

- Faça o build do projeto:

  ```
      mvn clean install
  ```

### Executa

- Inicie a aplicação:

  ```
      java -jar target/livechatms-0.0.1-SNAPSHOT.jar
  ```

## Testando aplicação

- Abra o navegador com a url: `http://localhost:5000/`

