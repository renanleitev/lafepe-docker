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

## Para rodar em um servidor externo (AWS, Cloud, Oracle)

Dê permissão para executar o script abaixo (ele irá trocar a url localhost pelo ip do servidor):

	sudo chmod +x url.sh

Passe o ip do servidor para o script alterar a URL da API backend no arquivo axios.js:

	./url.sh <IP_SERVIDOR:8080>

Obs: É importante que a porta ```8080``` esteja aberta no seu servidor

Após isso, deverá receber uma mensagem no terminal informando que a substituição da URL foi feita com sucesso.

	"Substituição concluída. O arquivo original foi salvo como axios.js.bak."

Caso ocorra algum erro, verifique se o arquivo ```url.sh``` possui permissão de execução (chmod +x) ou se você fez o ```git clone``` corretamente do repositório ```lafepe-frontend```.

Obs: Considerando que você está na pasta ```lafepe-docker```, você pode visualizar o conteúdo do arquivo ```axios.js``` e checar se o IP do seu servidor está presente no arquivo: 

```
cat ./lafepe-frontend/src/services/axios.js
```

## Para rodar os containers

	docker compose up

Obs: Pode ser que demore alguns segundos ou até minutos para a aplicação iniciar, se não der certo após dois minutos, tente novamente.

Caso dê tudo certo, abra o seu navegador e acesse o site: ```http://localhost:9090``` ou ```http://<IP_SERVIDOR>:9090```

## Para deletar os containers

	docker compose down

## Para deletar todos os containers

	docker container prune -f

## Equipe

1. Flávio Raposo
2. João Pedro Marinho
3. José Adeilton
4. Renan Leite Vieira
5. Rian Vinícius
6. Robério José