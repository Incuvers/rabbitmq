FROM arm64v8/rabbitmq:3.9-management

LABEL version="arm64v1.0.0"
LABEL Christian Sargusingh "https://github.com/cSDes1gn"

# package incuvers custom config
ADD rmq/rabbitmq.conf /etc/rabbitmq/
ADD rmq/definitions.json /etc/rabbitmq/
ADD rmq/enabled_plugins /etc/rabbitmq/

CMD ["rabbitmq-server"]