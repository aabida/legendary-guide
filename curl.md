
Delete a queue in a RabbitMQ vhost called / (%2F)
```shell
curl -i -u guest:guest -H "content-type:application/json" -X DELETE http://localhost:15672/api/queues/%2F/queue_name_here
```
