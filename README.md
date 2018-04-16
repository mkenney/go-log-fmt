# go-log-fmt

A simple https://github.com/sirupsen/logrus log formatter. Includes

* [iso 8601](https://en.wikipedia.org/wiki/ISO_8601) formatted date string - `"2006-01-02T15:04:05.000Z07:00"`
* OS hostname
* Log level
* Caller - "file:line func"
* Log message
* Additional fields

```
time="2018-04-16T05:14:07.559Z" host="k8s-proxy-688fb8b57d-4rzt4" level="info" caller="proxy.go:252 github.com/mkenney/k8s-proxy/pkg/proxy.(*Proxy).Start" msg="starting kubernetes proxy" port="80"
```

## Usage
text format (above)
```go
log.SetFormatter(&logfmt.TextFormat{})
```

JSON format
```go
log.SetFormatter(&logfmt.JSONFormat{})
```