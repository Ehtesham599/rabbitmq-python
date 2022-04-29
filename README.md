# RabbitMQ Python
> This is a simple implementation of publisher-consumer model using rabbitmq as the message queueing service.

## Usage
Make sure to have docker installed and daemon up and running on your machine.
Once docker is setup, run  `docker compose up` from the root directory of the project. This will build and start the rabbitmq container.
The rabbitmq management UI can be accessed via `localhost:15672`, for which the port is mentioned in the `docker-compose.yml` file under rabbitmq service.

To publish messages, run `python publisher.py`. This will send a simple 'Hello World' message body to the `hello` queue.

To consume messages, run `python consumer.py`. This reads messages from the `hello` queue.