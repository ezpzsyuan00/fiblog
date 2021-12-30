# README

## To set up
#### terminal window 1
```bash
$ cd ./django-rest-tutorial/mysite
```
```bash
$ python3 manage.py runserver 0.0.0.0:8000
```

#### terminal window 2
```bash
$ cd ./gRPC-fib
```
```bash
$ python3 server.py --ip 0.0.0.0 --port 8080
```

#### terminal window 3
```bash
$ cd ./gRPC-log
```
```bash
$ python3 server.py --ip 0.0.0.0 --port 8087
```

#### terminal window 4
```bash
$ cd ./eclipse-mosquitto
```
```bash
$ docker run -d -it -p 1883:1883 -v $(pwd)/mosquitto.conf:/mosquitto/config/mosquitto.conf eclipse-mosquitto
```
---
## To calculate
#### terminal window 5
```bash
$ curl -X POST http://localhost:8000/rest/fibonacii -d '{"order":{NUMBER}}'
```
```bash
$ curl -X GET http://localhost:8000/rest/fibonacii
```
---
## Video
