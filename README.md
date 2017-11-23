This is an example of application instrumented for Prometheus. By default it
listens on port 8080 and exposes metrics on the `/metrics` endpoint.

Set the CPU temperature metric:

```
curl http://localhost:8080/cpu -d 42.0
```

Increment the number of errors for the `sda` device:

```
curl http://localhost:8080/hd -d sda
```
