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

## Caso o Zookeper e os Brokers nao parem quando você quiser matar seus processos no terminal, faça o seguinte:

Este comando lista as portas que estāo em uso:

```sudo lsof -PiTCP -sTCP:LISTEN```

e depois mate o processo desta port, com usando seu PID correspondente:

```kill <PID>```

Assim conseguimos garantir que nāo tenha nada rodando em segundo plano.


> Nāo é mandatorio ter tudo isso rodando local, ate por que nos nossos testes estaremos usando Kafka Embedded ;). Mas e importante ter o Kafka instalado local, ou ao menos via imagem docker.

## Expert
| [<img src="https://avatars.githubusercontent.com/u/42419543?v=4" width="75px;"/>](https://github.com/anabneri) |
| :-: |
|[Ana Neri](https://github.com/anabneri)|
