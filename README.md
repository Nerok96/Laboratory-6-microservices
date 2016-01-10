# Web Engineering 2015-2016 / Microservices

#1.- The two microservices are running and registered.

![imagen 1-2](https://raw.githubusercontent.com/Nerok96/Laboratory-6-microservices/master/img/3pract6-term-eureka1111-accounts2222.png)
![imagen 1-2](https://raw.githubusercontent.com/Nerok96/Laboratory-6-microservices/master/img/4pract6-term-eureka1111-accounts2222-web3333-working.png)

#2.- The service registration service has the two microservices registered.

![imagen 2-1](https://github.com/Nerok96/Laboratory-6-microservices/blob/master/img/5pract6-dash-eureka1111-accounts2222-web3333-working.png)

#3.- A second account microservice is running in the port 4444 and it is registered.

![imagen 3-1](https://raw.githubusercontent.com/Nerok96/Laboratory-6-microservices/master/img/6pract6-termDash-accounts4444.png)
![imagen 3-2](https://raw.githubusercontent.com/Nerok96/Laboratory-6-microservices/master/img/7pract6-lastStep-accounts2222Donwn-accounts4444Up-server3333Working.png)

#4.- A brief report describing what happens when you kill the microservice with port 2222. Can the web service provide information about the accounts? Why?

Killing the microservice "accounts" (wich is running on the port 2222) will result in the registration service redirecting the petitions to the other "accounts" microservice wich is running on the port 4444. This change will take some time to become efective (less than a minute, enough time to the registration service to detect that the microservice is donw and prepare the other one).