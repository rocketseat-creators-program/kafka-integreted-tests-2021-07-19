<img src="https://storage.googleapis.com/golden-wind/experts-club/capa-github.svg" />

# Kafka4devs - Testes Integrados no Kafka

Testes integrados usando kafka sáo muito comuns no dia a dia, nesta aula você irá aprender abordagens, conceitos e também libs para construir testes que abordem o cenário de integração de um tópico vindo de um producer no Kafka.
O objetivo desta aula é ser bem objetiva, no início te mostrando um pouco do conceito de testes integrados (que ainda causa muita confusão na vida do dev), e depois partir pra mão na massa vendo abordagens de testes.

## Tests
Para executar os testes utilizar

``` ./gradlew test```

## Zookeper e brokers do Kafka
Para dar um start no Zookeper, utilize:

``` ./zookeeper-server-start.sh ../config/zookeeper.properties```

Depois para dar start no kafka broker, utilize:

``` ./kafka-server-start.sh ../config/server.properties```

Parar parar com algum servidor e executar os testes utilizando o Embedded Kafka, utilize:

```sudo lsof -PiTCP -sTCP:LISTEN```

e depois

```kill <PID>```

Assim conseguimos garantir que nāo tenha nada rodando em segundo plano.


> Nāo é mandatorio ter tudo isso rodando local, ate por que nos nossos testes estaremos usando Kafka Embedded ;). Mas e importante ter o Kafka instalado local, ou ao menos via imagem docker.

## Expert
| [<img src="https://avatars.githubusercontent.com/u/42419543?v=4" width="75px;"/>](https://github.com/anabneri) |
| :-: |
|[Ana Neri](https://github.com/anabneri)|
