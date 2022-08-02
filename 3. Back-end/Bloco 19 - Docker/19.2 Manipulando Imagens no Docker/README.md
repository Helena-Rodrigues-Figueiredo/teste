# Exercícios do Dia 19.2

## Instruções

Vamos usar uma imagem disponível no DockerHub conhecida como "cowsay" (uma vaca falante no terminal 🐮)!
A ideia é deixarmos a mensagem para o cowsay parametrizável. Dessa forma, conseguiremos executar o seguinte comando:

`docker container run cowsay Muuuuuuhhh`

E teremos a seguinte saída no terminal:

____________
< Muuuuuuhhh >
------------
         \   ^__^
         \  (oo)\_______
            (__)\       )\/\
               ||----w |
               ||     ||

## Exercícios

1 -Crie um Dockerfile utilizando a imagem chuanwen/cowsay. <br />

2 - Defina um ENTRYPOINT para a execução do comando. <br />
* Observe que o executável cowsay está no diretório /usr/games/ <br />
* Lembre-se que com ele, diferente do CMD, o comando não poderá ser sobrescrito com o docker run, porém conseguiremos passar parâmetros ao binário e exploraremos esse recurso para poder passar a mensagem. <br />

3 - Utilize o CMD para definir uma mensagem padrão. <br />

4 - Gere uma build e execute um contêiner baseado em sua imagem sem passar nenhum comando. <br />

5 - Execute um novo contêiner passando sua mensagem para testar. Além da mensagem você pode utilizar a opção -l para listar outros personagens disponíveis e então executar algo como docker container run cowsay -f dragon-and-cow "VQV TRYBE", para exibir um dragão junto com a vaquinha. <br />