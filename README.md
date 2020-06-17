<!-- docker run --rm --volume "C:/Docker/GPS_docs/:/data" pandoc/latex:2.6 --pdf-engine=xelatex --highlight-style zenburn --toc -N README.md -o README.pdf -->

---
title: Track-RabbitMQ-Kafka-Clickhouse (v1.0)
author: Adriana Jiménez (adriana.jimenez@axity.com)
date: 15 de Junio de 2020
---

# Propósito

Componente Kafka, como plataforma de transmisión de eventos, trabaja con la transmisión de datos en tiempo real. Su misión principal es:

- Capturar los mensajes desde las colas de actividades y alertas de RabbitMQ.
- Ingestar los mensajes a Clickhouse en sus respetivas colas.


# Funcionamiento general de Kafka y conectores

# Monitoreo de funcionamiento 