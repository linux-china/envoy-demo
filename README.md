Envoy demo
==========
Envoy demo with httpbin(local), google(remote), mysql(tcp proxy), grpc configuration.

# Usage

* Use docker-compose to start all services
* Open http://localhost:3000/ to visit Grafana dashboard, the account is admin/admin

# Envoy testing

* MySQL: password is 123456

```
mysql -h 127.0.0.1 -P 3307 -u root -p demo
```

* httpbin

```
curl http://localhost:10800/ip
```

* grpc testing: please install evans from https://github.com/ktr0731/evans first

```
cd proto
evans
```

* google service test

```
curl http://localhost:10000/
```



