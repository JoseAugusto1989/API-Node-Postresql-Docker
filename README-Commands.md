npm init -y

npm install express pg sequelize

npm install nodemon
"start": "node ./src/index.js" -> package.js

rodar o projeto na pasta app:
node index.js

na pasta do arquivo principal:
docker image build -t "nome do arquivo" .

docker images: listar todas as imagens do docker

rodar a imagem do docker:
docker run -p 3001:3001 "nome do arquivo"

listar os containeres:
docker ps -a

excluir container:
docker rm -f "container id" OBS: pode abreviar com os primeiros caracteres

após a criação do docker-compose, fazer um build:
docker-compose build

rodar o projeto:
docker-compose up

após a criação do arquivo docker-compose.yml fazer o build:
docker-compose up

rodar o comando em um terminal separado:
docker exec -it "container id" psql -U "user" "db name"
OBS: user or password
OBS: container: image postgres:12

"test_db=#" \dt
para listar os relacionamentos

select * from users;

sair do db no terminal:
exit

****Comandos para executar o projeto****

git clone ...
npm i
instalar, docker, docker-compose
docker-compose up no terminal
docker exec -it "container id | 9c59" psql -U "user | admin" "nome banco de dados | test_db"
select * from users;   para listar todos os usuarios cadastrados

ENDPOINTS

http://localhost:3001/dev/version  GET
http://localhost:3001/users   GET
http://localhost:3001/users   POST
http://localhost:3001/users/1   PUT
http://localhost:3001/users/1   DELETE

EXEMPLO DE JSON

{
    "username": "gutoTestUpdate",
    "email": "update@email.com",
    "password": "testeUpdate"
}

