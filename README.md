# README

#### terminal window 1
$ cd ./django-rest-tutorial/mysite
$ python3 manage.py runserver 0.0.0.0:8000

#### terminal window 2
$ cd ./gRPC-fib
$ python3 server.py --ip 0.0.0.0 --port 8080

#### terminal window 3
$ cd ./gRPC-log
$ python3 server.py --ip 0.0.0.0 --port 8087

#### terminal window 4
$ cd ./eclipse-mosquitto
$ docker run -d -it -p 1883:1883 -v $(pwd)/mosquitto.conf:/mosquitto/config/mosquitto.conf eclipse-mosquitto

#### terminal window 5
$ curl -X POST http://localhost:8000/rest/fibonacii -d '{"order":{NUMBER}}'
$ curl -X GET http://localhost:8000/rest/fibonacii
