# deploy-laravel-git

Você pode seguir o tutorial para a instalação e configuração do laravel aqui na documentação oficial.

Levando em consideração que você tenha php e composer na sua variável global PATH, para uma nova instalação do Laravel, execute:

composer create-project laravel/laravel nome-do-seu-projeto --prefer-dist

Clonando um projeto e instalando o Laravel
Vou novamente considerar que você esteja rodando um sistema operacional Linux e com o git instalado, faça o seguinte:

Clone o projeto
`git clone git@github.com:seuprojeto`

Acesse o projeto
`cd seuprojeto`

Instale as dependências e o framework
`composer install --no-scripts`

Copie o arquivo .env.example
`cp .env.example .env`

Crie uma nova chave para a aplicação
`php artisan key:generate`

Em seguida você deve configurar o arquivo .env e rodar as migrations com:

`php artisan migrate --seed`

Em relação ao npm, isso varia de projeto para projeto, mas provavelmente você também vai precisar rodar os seguintes comandos:

`npm install`

`bower install`

`gulp`

Se você não faz idéia do que significa estes comandos, sugiro que comece a estudar um a um antes de colocar uma aplicação em produção. A documentação oficial do Laravel contém dois projetos exemplos desenvolvido passo-a-passo, não é uma má idéia iniciar por ai, está em inglês mas o texto é de fácil leitura.
