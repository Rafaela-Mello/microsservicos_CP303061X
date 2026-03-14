# Microsserviços com Spring Boot e RabbitMQ
Projeto baseado em arquitetura de microsserviços, composto por dois serviços independentes:

👤 User Service: Responsável pelo cadastro de usuários.

📧 Email Service: Responsável por enviar e-mails de boas-vindas para usuários cadastrados.

A comunicação entre os serviços acontece de forma assíncrona utilizando RabbitMQ, permitindo que cada serviço funcione de forma independente e desacoplada.

Cada microsserviço possui:
- Banco de dados próprio
- API REST própria
- Execução independente
- Comunicação assíncrona via RabbitMQ

# Instruções do Projeto

1. Clonar o repositório:

`git clone https://github.com/Rafaela-Mello/microsservicos_CP303061X.git`

2. Configurar o banco de dados MySQL. Criar dois bancos de dados:
- ms_user
- ms_email

3. Configurar RabbitMQ

Configurar as credenciais do RabbitMQ no arquivo application.properties de cada serviço.

4. Executar os microsserviços

Executar cada serviço separadamente pela IDE ou via Maven (`mvn spring-boot:run`).

User Service → porta 8081

Email Service → porta 8082

5. Utilize o ThunderClient (extensão do VS Code) ou qualquer cliente HTTP (Postman, Insomnia) para testar os endpoints.