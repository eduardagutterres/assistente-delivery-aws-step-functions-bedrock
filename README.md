# Assistente de Delivery com AWS Step Functions e Amazon Bedrock

Projeto desenvolvido como parte de um desafio prático da *DIO, com o objetivo de criar um assistente de delivery utilizando **AWS Step Functions* para orquestração do fluxo e *Amazon Bedrock* para interação com um modelo de Inteligência Artificial Generativa.

## Objetivo

O projeto demonstra como utilizar uma máquina de estados serverless para coordenar diferentes etapas de uma conversa com um assistente de delivery.

O fluxo foi estruturado para:

- iniciar uma interação com o usuário;
- enviar prompts para um modelo via Amazon Bedrock;
- armazenar informações intermediárias da conversa;
- identificar preferências alimentares;
- tomar decisões utilizando um estado Choice;
- gerar uma recomendação personalizada quando houver preferência informada;
- retornar uma resposta padrão quando nenhuma preferência for identificada.

## Tecnologias utilizadas

- AWS Step Functions
- Amazon Bedrock
- Claude Haiku 4.5
- AWS IAM
- GitHub

## Máquina de estado

A máquina de estado criada recebeu o nome:

```text
AssistenteDeliveryBedrock
