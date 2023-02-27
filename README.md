# loja_alura
## Projeto criado junto ao Curso Alura Utilizando Go
### Aplicação Web com Go capaz de criar produtos, salvar, deletar e editar as informações desses produtos no banco de dados postgres.
#### Projeto desenvolvido no Mac pois já tinha o Postgres instalado
#### Criamos o nosso projeto no workspace correto, dentro do GOPATH (dentro da pasta src, github.com, seguido do nome de usuário do Github);
* Aprendemos como subir um servidor através da função http.ListenAndServe(), exibindo uma tabela com nossos produtos;
* Em seguida criamos uma struct de Produto, onde instanciamos alguns produtos e exibimos de forma dinâmica em nossa index.html.
* Instalamos o Postgres para armazenar nossos produtos de forma segura;
* Criamos uma função chamada conectaComBancoDeDados() para abrir a conexão com o banco de dados;
* Alteramos nosso código para exibir os produtos que estão cadastrados lá no banco de dados.
* Modularizamos o código para tornar a manutenção e/ou atualização mais clara, criando as pastas controllers, db, models, routes e templates;
* Criamos uma página para criar novos produtos e uma rota capaz de atender essa requisição http.HandleFunc("/new", controllers.New);
* Buscamos os dados da página new com o código r.FormValue() para cada input (nome, descrição, preço e quantidade) no controller de produtos;
* Salvamos o produto através do modelo de produto criando a função CriaNovoProduto().
