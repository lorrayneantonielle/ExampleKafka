# Exemplo Kafka Producer-Consumer em C# com Docker e Zookeeper

Este repositório contém um exemplo de um produtor e consumidor Kafka escrito em C#. Ele demonstra como configurar e executar o Kafka e Zookeeper usando Docker, e como interagir com eles usando C#.

## Pré-requisitos

- .NET Core SDK
- Docker
- Docker Compose

## Começando

Primeiro, clone este repositório:

\`\`\`bash
git clone [[https://github.com/seuusername/exemplo-kafka-csharp-docker.git](https://github.com/lorrayneantonielle/ExampleKafka.git)](https://github.com/lorrayneantonielle/ExampleKafka.git)
cd exemplo-kafka-csharp-docker
\`\`\`

## Executando Kafka e Zookeeper com Docker

Para iniciar o Kafka e Zookeeper usando Docker Compose, execute o seguinte comando:

\`\`\`bash
docker-compose up -d
\`\`\`

## Construindo e Executando a Aplicação

A aplicação consiste em duas partes: um produtor que envia mensagens para o Kafka, e um consumidor que lê essas mensagens.

### Construindo a Aplicação

Para construir a aplicação, use o CLI `dotnet`:

\`\`\`bash
dotnet build
\`\`\`

### Executando o Produtor

Para executar o produtor, use o CLI `dotnet`:

\`\`\`bash
dotnet run --project Produtor
\`\`\`

### Executando o Consumidor

Para executar o consumidor, use o CLI `dotnet`:

\`\`\`bash
dotnet run --project Consumidor
\`\`\`

## Como Funciona

O produtor envia mensagens para um tópico Kafka. O consumidor se inscreve neste tópico e imprime quaisquer mensagens que recebe.

## Solução de Problemas

Se você encontrar algum problema ao executar a aplicação, tente as seguintes etapas:

- Verifique se o Kafka e o Zookeeper estão funcionando corretamente.
- Verifique as configurações de conexão no produtor e no consumidor.
- Certifique-se de que o tópico existe e está configurado corretamente.

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para enviar um Pull Request.
