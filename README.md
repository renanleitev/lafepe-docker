# Lafepe Full Stack Application

Aplicação Full Stack da Lafepe para registro e controle de estoque de produtos e medicamentos.

## Estrutura

1. Front End: React + Vite
2. Back End: Spring Boot (Java)
3. Banco de Dados: MySQL 
4. Deploy: Docker Compose

## Para obter os componentes

Faça o clone deste repositório:

	git clone https://github.com/renanleitev/lafepe-docker.git

Depois, acesse a pasta com o código (ou usando o terminal):

    cd lafepe-docker

De dentro da pasta ```lafepe-docker```, faça o clone dos repositórios Front e Back End:

Front End
	
	git clone https://github.com/renanleitev/lafepe-frontend.git

Back End

	git clone https://github.com/renanleitev/lafepe-backend.git

## Para rodar os containers

	docker compose up

Obs: Pode ser que demore alguns segundos para aplicação iniciar, se não der certo após dois minutos, tente novamente.

Caso dê tudo certo, abra o seu navegador e acesse o site: ```http://localhost:9090```

## Para deletar os containers

	docker compose down

## Para deletar todos os containers

	docker container prune -f