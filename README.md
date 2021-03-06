# mock-zendesk


![](https://img.shields.io/docker/build/allansimon/mock-zendesk.svg)


HTTP Service that aims to replicate the Zendesk API and logic
so that one can use it in local environment has a drop-in replacement to zendesk
which is practical when you're several developers who all needs to modify
the same tickets while testing your features

There's a docker image available here:

<https://hub.docker.com/r/allansimon/mock-zendesk>

or simply

```
docker pull allansimon/mock-zendesk
```

## Contributing

I'm more than opened to PR, if you don't know where to start, just drop an issue :)

## Auth supported:

  * API Token only for the moment

## Operation supported:

  * Posting ticket (with tags, comment, description, requester, external id)
  * Getting a ticket information
  * Getting the list of comments on a ticket
  * Updating a ticket (new tags, status, new comment)



## Note:

The service requires the following env variables to works:

   * `MOCK_ZENDESK_API_KEY`
   * `MOCK_ZENDESK_USERNAME`
   * `MOCK_ZENDESK_PORT` (default to `8084`)


## Other Mock projects:

If you liked it, you may also appreciate my other mocks:

   * [Rabbitmq](https://github.com/allan-simon/mock-amqp-server)
