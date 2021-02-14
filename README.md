
# NiFi Hands-on

## Getting started

Start the Docker Compose service.

```bash
$ docker-compose up
```

Then you'll have access to the UI.

- NiFi: `http://localhost:9090/nifi/`
- NiFi Registry: `http://localhost:9090/nifi-registry/`
- RabbitMQ Management: `http://localhost:9090/amqp/`

You can also access any NiFi port at the following URL. This is intended for the `HandleHttpRequest` processor.

- (**Example**) NiFi Port `8081`: `http://localhost:9090/nifi-port-8081/`

When the container is started, the `in` and `out` directories are created. These are intended to simplify the exchange of files between the host and container, and to make it easier to use processors such like `GetFile` and `PutFile`.

## References

- [How to install and start NiFi](https://nifi.apache.org/docs/nifi-docs/html/administration-guide.html#how-to-install-and-start-nifi)
- [How to install and start NiFi Registry](https://nifi.apache.org/docs/nifi-registry-docs/html/administration-guide.html#how-to-install-and-start-nifi-registry)
- [Proxy Configuration](https://docs.cloudera.com/HDPDocuments/HDF3/HDF-3.3.0/nifi-configuration-best-practices/content/proxy_configuration.html)
- [RabbitMQ / NGINX](https://gist.github.com/lukebakken/a6bae4759979b37ad2e87d48b47aa02e)
- [Using environment variables in nginx configuration (new in 1.19)](https://github.com/docker-library/docs/tree/master/nginx#using-environment-variables-in-nginx-configuration)
