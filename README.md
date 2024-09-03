# Coleção de Microsserviços AWS

## Visão Geral

Este repositório serve como um hub central para uma coleção de microsserviços projetados para demonstrar expertise em diversas tecnologias da AWS. Cada microsserviço foca em uma área específica da AWS, abrangendo desde o gerenciamento de usuários até análise de dados e automação de infraestrutura. Esses microsserviços estão organizados como submódulos Git dentro deste repositório, facilitando o gerenciamento e a colaboração em cada serviço de forma individual.

## Visão Geral dos Microsserviços

### 1. [Serviço de Gerenciamento de Usuários](services/user-management)
Um microsserviço para gerenciamento de usuários, incluindo registro, login e gerenciamento de perfis. Este serviço utiliza AWS RDS para armazenar dados dos usuários, S3 para armazenamento de avatares e IAM para controle de acesso.

### 2. [Serviço de Upload de Imagens](services/image-upload)
Um microsserviço serverless que lida com o upload de imagens. Ele utiliza AWS Lambda para processamento, S3 para armazenamento e DynamoDB para gerenciamento de metadados.

### 3. [Serviço de Pipeline CI/CD](services/ci-cd-pipeline)
Este serviço automatiza o processo de deploy para aplicações web utilizando AWS CodePipeline, CodeBuild e CodeDeploy. É ideal para demonstrar práticas de CI/CD na AWS.

### 4. [Serviço de Monitoramento](services/monitoring)
Um microsserviço que monitora o desempenho de aplicações utilizando AWS CloudWatch. Inclui dashboards, alarmes e notificações para garantir a saúde da aplicação.

### 5. [Serviço de Autenticação](services/auth-service)
Um serviço de autenticação segura utilizando AWS Cognito e IAM. Ele gerencia a autenticação de usuários, tokens e controle de acesso.

### 6. [Serviço de Data Lake](services/data-lake)
Implementa um Data Lake utilizando AWS S3 para armazenamento, Glue para processos ETL e Athena para consultas de dados. Ideal para demonstrar o manuseio de big data na AWS.

### 7. [Serviço de Gerenciamento de Containers](services/container-management)
Gerencia aplicações conteinerizadas implantadas no Amazon ECS com Fargate. As imagens Docker são armazenadas no ECR, e o serviço lida com o deploy e escalabilidade.

### 8. [Serviço de API GraphQL](services/graphql-api)
Um microsserviço que fornece uma API GraphQL utilizando AWS AppSync e DynamoDB, com autenticação gerenciada pelo Cognito.

### 9. [Serviço de Automação de Backup](services/backup-service)
Automatiza backups para AWS RDS, EFS e DynamoDB utilizando AWS Backup. Inclui recursos para recuperação de desastres e gerenciamento de backups.

### 10. [Serviço de Deploy Multi-AZ](services/multi-az-deployment)
Realiza o deploy de uma aplicação web altamente disponível em múltiplas zonas de disponibilidade (Multi-AZ) com Auto Scaling e Elastic Load Balancing.

## Clonando o Repositório

Para clonar este repositório juntamente com todos os submódulos, utilize o seguinte comando:

```bash
git clone --recurse-submodules https://github.com/sousaprogramador/aws-microservices.git
