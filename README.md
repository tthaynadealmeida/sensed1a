## ☀️ Thayná de Almeida - Sensedia 2023 ☀️

Esse arquivo é destinado ao processo de criação de uma nova imagem de container via Docker através do servidor Ngnix. 
Todos os procedimentos abaixo foram realizados através do sistema Operacional Linux Ubuntu 18.4.  
A imagem de container está disponivel no DockerHub:    
<https://hub.docker.com/repository/docker/kalth8888/html-thayna-sensedia2023>  

* Utilizando o Visual Studio Code, criei "New File";  
* Criei um novo arquivo "Dockerfile";  
* Inseri um tema html personalizado;  
* Realizei a instalação do Docker através dos comandos:  
````
sudo apt install docker.io
````
Estava tendo problemas para executar o Daemon do Docker: "How to Resolve the “cannot connect to the Docker daemon” Error". O problema foi solucionado realizando a instalação do Docker Compose;  
````
sudo apt-get install docker.ce  
````
* Para criar a imagem de container, utilizei o comando:  
````
docker build -t html-thayna-sensedia2023
````
* Para confirmar que a imagem foi criada:  
````
docker images
````
* Comando para a imagem entrar em execução:  
````
docker run -d -p 80:80 html-thayna-sensedia2023
````
* Acesso via Localhost concluído! 😸 😻  

* Para adicionar a imagem de container no DockerHub, acessei meu usuário via terminal com os seguintes comandos:
````
docker user -u meuusuario
````
* Criei um novo repositorio com o nome "Sensed1a" para realizar o push. Inseri os seguintes códigos:
````
sudo docker image tag html-thayna-sensedia2023 kalth8888/html-thayna-sensedia2023````
````
* Utilizei o comando para realizar o push
````
docker image push kalth8888/html-thayna-sensedia2023
````
Abaixo encontra-se o resultado final (imagem de fundo Dribble)
![Print](https://64.media.tumblr.com/ab08743c9ff692bad7fb7ee0487aecc4/a43fb881fc010994-54/s1280x1920/90737e157dfab79a1089bb3319a664ce86de885a.pnj)  

Obrigada! 🌻  
Att. Thayná de Almeida
