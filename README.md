# go-log-fmt

A simple https://github.com/sirupsen/logrus log formatter. Includes

* [iso 8601] formatted date string - `"2006-01-02T15:04:05.000Z07:00"`
* OS hostname
* Log level
* Caller - "file:line func"
* Log message
* Additional fields

```
time="2018-04-16T04:54:37.107Z" host="k8s-proxy-5cf98cbb96-b4pwn" level="warning" caller="log_format.go:110 main.(*textFormat).Format" msg="request failed, no matching service found" url="http://10.1.3.205:80/k8s-ready"
```

