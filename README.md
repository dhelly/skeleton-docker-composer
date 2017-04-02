# Skeleton docker-composer
Este projeto contém alguns exemplos de arquivos do docker-compose que uso para estudar

## Arquivo `docker-compose-node_mongo.yml`

- Criar um volume no docker para armazenar os dados db do mongo(necessário para windows 10)
	```
	docker volume create --name mongodata
	```
- Definir a pasta onde estará o projeto na máquina local e colocar na opção: [local_path]
- Para instalar o nodemon basta alterar a linha command(web)
	```
	command: sh -c 'npm install; nodemon app' 
	```
	para:
	```
	command: sh -c 'npm install; npm install -g nodemon; nodemon app' 
	```


