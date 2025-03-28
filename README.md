Observability com Elastic Stack 🌐🔍
Este projeto demonstra a implementação de monitoramento de performance e logs para uma aplicação utilizando a stack Elastic, incluindo Elastic APM, Nginx, Django, PostgreSQL, Filebeat e Kibana. O objetivo é fornecer visibilidade total sobre o desempenho da aplicação, uso de recursos e erros, utilizando o Elastic Stack na Elastic Cloud ☁️.

Tecnologias Utilizadas 🛠️
Elastic Cloud ☁️ - Para armazenar e visualizar os dados de performance da aplicação.

Elastic APM 📊 - Monitoramento de performance e erros da aplicação.

Nginx 🔄 - Configurado como proxy reverso para a aplicação Django.

Django 🐍 - Framework web para a aplicação.

PostgreSQL 🗃️ - Banco de dados da aplicação.

PgAdmin 🖥️ - Interface gráfica para gerenciamento do PostgreSQL.

Filebeat 📦 - Para coleta de logs do Nginx.

Kibana 📈 - Para visualização de logs e métricas coletadas.

Objetivo 🎯
O projeto foi configurado para fornecer um fluxo de trabalho completo de monitoramento e observabilidade com as seguintes funcionalidades:

APM Configuration ⚙️:

O Elastic APM foi configurado para capturar métricas de performance, logs de erros e traces de transações da aplicação.

As configurações incluem SERVICE_NAME, SECRET_TOKEN e SERVER_URL, apontando para o Elastic Cloud.

As métricas e logs são visíveis em tempo real no painel de monitoramento da Elastic Cloud.

Nginx como Proxy Reverso 🔀:

O Nginx foi configurado como proxy reverso para a aplicação Django, garantindo que a aplicação esteja acessível externamente.

O Nginx também foi configurado para coletar logs, usando o Filebeat para enviar logs para o Kibana, facilitando a visualização e análise de erros.

Banco de Dados e Ferramentas 🗂️:

O PostgreSQL foi configurado como banco de dados para a aplicação.

O PgAdmin foi configurado para facilitar a administração do PostgreSQL via interface gráfica.

Coleta de Logs com Filebeat 📜:

O Filebeat foi configurado para coletar logs do Nginx e enviar para o Kibana.

A visualização de logs e insights de erros foi configurada na interface do Kibana.

Como Funciona 🚀
APM 📊:

Após a configuração do APM, a aplicação começa a enviar métricas de CPU, memória e traces de transações para o Elastic Cloud.

Logs de erros e insights sobre a performance são exibidos no painel de monitoramento do Elastic Cloud.

Nginx 🔄:

O Nginx está configurado para atuar como proxy reverso para a aplicação Django.

Logs de acesso e erro do Nginx são enviados para o Kibana, onde você pode visualizar os detalhes de tráfego e erros.

Filebeat 📦:

O Filebeat coleta logs do Nginx e envia para o Kibana. Isso permite a visualização centralizada dos logs de todos os serviços envolvidos.

Instruções de Execução 📝
Pré-requisitos ⚙️:

Docker 🐳

Docker Compose 🧩

Conta no Elastic Cloud para APM e Kibana 🔑

Configuração 🛠️:

Crie um arquivo .env para definir variáveis como SERVICE_NAME, SECRET_TOKEN e SERVER_URL.

Configure o Nginx como proxy reverso no arquivo nginx.conf.

Utilize Docker Compose para levantar os containers de Django, Nginx, PostgreSQL, PgAdmin e Filebeat.

Subindo os Contêineres 🚢:

Execute o comando:

bash
Copy
Edit
docker-compose up -d
Acessando o Painel Kibana 📊:

Abra o Kibana na Elastic Cloud para visualizar logs, métricas e dados de performance.

Acesse o painel de APM e explore as métricas de desempenho da sua aplicação.

Conclusão 💡
Este projeto integra o monitoramento e a observabilidade usando a Elastic Stack, proporcionando uma visão clara e detalhada do comportamento da aplicação em tempo real 🔍. Explore os logs, visualize métricas e melhore o desempenho da sua aplicação com essas ferramentas poderosas!

Comandos Úteis ⚡
Para verificar os logs de execução:

bash
Copy
Edit
docker logs <container_id>
Para verificar os containers em execução:

bash
Copy
Edit
docker ps

Observability with Elastic Stack 🌐🔍
This project demonstrates the implementation of performance monitoring and logging for an application using the Elastic Stack, including Elastic APM, Nginx, Django, PostgreSQL, Filebeat, and Kibana. The goal is to provide full visibility into the application's performance, resource usage, and errors using Elastic Cloud ☁️.

Technologies Used 🛠️
Elastic Cloud ☁️ - For storing and visualizing application performance data.

Elastic APM 📊 - Monitoring performance and errors in the application.

Nginx 🔄 - Configured as a reverse proxy for the Django app.

Django 🐍 - Web framework for the application.

PostgreSQL 🗃️ - Database for the application.

PgAdmin 🖥️ - Graphical interface for PostgreSQL management.

Filebeat 📦 - For collecting Nginx logs.

Kibana 📈 - For visualizing logs and metrics collected.

Objective 🎯
The project is set up to provide a complete workflow for monitoring and observability with the following features:

APM Configuration ⚙️:

Elastic APM is configured to capture performance metrics, error logs, and transaction traces from the application.

The configuration includes SERVICE_NAME, SECRET_TOKEN, and SERVER_URL, pointing to Elastic Cloud.

Metrics and logs are visible in real-time on the Elastic Cloud monitoring dashboard.

Nginx as Reverse Proxy 🔀:

Nginx is configured as a reverse proxy for the Django app, ensuring external accessibility.

Nginx is also set up to collect logs, using Filebeat to send logs to Kibana, making it easier to visualize and analyze errors.

Database and Tools 🗂️:

PostgreSQL is set up as the database for the application.

PgAdmin is configured to simplify PostgreSQL administration via a graphical interface.

Log Collection with Filebeat 📜:

Filebeat is configured to collect Nginx logs and send them to Kibana.

Log visualization and error insights are displayed on the Kibana interface.

How It Works 🚀
APM 📊:

Once the APM is configured, the application starts sending CPU, memory, and transaction trace metrics to Elastic Cloud.

Error logs and performance insights are displayed on the Elastic Cloud monitoring dashboard.

Nginx 🔄:

Nginx is configured to act as a reverse proxy for the Django application.

Access and error logs from Nginx are sent to Kibana, where you can view traffic and error details.

Filebeat 📦:

Filebeat collects logs from Nginx and sends them to Kibana, allowing centralized log viewing of all services involved.

Running Instructions 📝
Prerequisites ⚙️:

Docker 🐳

Docker Compose 🧩

An Elastic Cloud account for APM and Kibana 🔑

Setup 🛠️:

Create a .env file to define variables like SERVICE_NAME, SECRET_TOKEN, and SERVER_URL.

Configure Nginx as a reverse proxy in the nginx.conf file.

Use Docker Compose to bring up the containers for Django, Nginx, PostgreSQL, PgAdmin, and Filebeat.

Bringing Up Containers 🚢:

Run the command:

bash
Copy
Edit
docker-compose up -d
Accessing the Kibana Dashboard 📊:

Open Kibana on Elastic Cloud to view logs, metrics, and performance data.

Access the APM dashboard to explore the application’s performance metrics.

Conclusion 💡
This project integrates Elastic Stack for monitoring and observability, providing a clear and detailed view of the application's behavior in real-time 🔍. Explore logs, view metrics, and improve your application's performance with these powerful tools!

Useful Commands ⚡
To check the execution logs:

bash
Copy
Edit
docker logs <container_id>
To check running containers:

bash
Copy
Edit
docker ps
