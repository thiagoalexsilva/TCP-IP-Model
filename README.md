# TCP-IP-Model

## About

CEFET-MG Computer Engineering's Computer Networks Systems class homework
proposed by Sandro Renato Dias <https://sites.google.com/site/sandrord>

Development group:
* [Gustavo Borba](https://github.com/gustavohsborba)  [gustavohsborba@gmail.com]
* [Bruno Maciel]()  [bmarques.maciel@gmail.com]
* [Thiago Alexandre](https://github.com/thiagoalexsilva)  [thiagoalexsilva93@gmail.com]
* [Ana Claudia](https://github.com/gmanaclaudia)  [gmanaclaudia@gmail.com]


## Setting up Environment

Just run [install_dependencies.sh](https://github.com/gustavohsborba/TCP-IP-Model/blob/master/install_dependencies.sh)
and you'll have environment set up for all languages and frameworks used in
this project. You must run it as superuser, as it will install packages
and manage permissions into your system.

## Running layers:

### Physical Layer (C++)

To compile physical layer, just go to it's folder and run the following command:
```shell
g++ -o server server-side.cpp && g++ -o client client-side.c
```
Now you have a client and a server executables. 

To start them, first execute the server:
```shell
./server
```
Then execute the client. The client needs two arguments:
1. server IP or hostname
2. filename to transfer
```shell
./client 127.0.0.1 datagram.txt
```

Primeiro foi implementado um frame (da camada de enlace). Após o início da comunicação do socket, encontramos o MAC address do servidor e o cliente pergunta o tamanho do frame. Quando o servidor responde, o cliente começa a enviar um arquivo dividido em pacotes do tamanho certo para o servidor.


### Transport Layer (Python)

still in the making

### Network Layer (PHP)

still in the making

### Application Layer (Scala)

still in the making
