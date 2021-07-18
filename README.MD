VERSION: 0.0.0

Ideia:

Construir um blog simplificado que permita versionar o conteúdo junto com o repositório.

Propósito:
 - Contruir um Blog para expor meus estudos e ter minhas anotaçoes para quando eu precisar
 - Durante a construção deste projeto desenvolver alguns conhecimentos e habilidades com:
    - Lumen
    - Docker
    - Git

- comprar plano vps1 para um ano da Hostinger (240 ao todo)
			- Fazer uma instalação Docker para executar o Lumen
				https://medium.com/@henrique.weiand/lumen-instalando-atrav%C3%A9s-do-docker-62f1ac9504ad
				https://medium.com/@henrique.weiand/laravel-lumen-crud-docker-tests-introdu%C3%A7%C3%A3o-e-ambiente-83e8163ec01b
				https://medium.com/@henrique.weiand/laravel-lumen-crud-docker-tests-introdu%C3%A7%C3%A3o-e-ambiente-83e8163ec01b
			- Criar parte de autenticação (somente eu terei autorização)
			- então haverá uma tela tipo editor de texto, um campo nome e um botão.
			- o botão salva o arquivo com o nome definido (tem que ser unico. vai add a datahora da criação)
				*pode ter um campo select2 "tags"
				e já salva no arquivo json
				haverá um arquivo .json com os links
			... Efim. este será meu blog
			e seu primeiro artigo será o PushNotification
				ESTUDO_PushNotifications.txt


-----------

Vamos usar:
Docker
PHP
Lumen
Ou não vamos usar banco de dados ou vamos usar SQLite

Referencias:
https://medium.com/@henrique.weiand/lumen-instalando-atrav%C3%A9s-do-docker-62f1ac9504ad
https://medium.com/@henrique.weiand/laravel-lumen-crud-docker-tests-introdu%C3%A7%C3%A3o-e-ambiente-83e8163ec01b

---------------

Passos que usei para criar:
1. Criei o repositório local e o README.MD
    - git init
    - git flow init
    - git flow feature start <nome_branch>
2. Criei o repositório no GitHub e adicionei a referência no local
    - git remote add https://github.com/GustavoTrr/blog.git
3. Realizei o primeiro commit
    *precisei mudar o nome da branch com o comando "git branch -m feature/<novo_nome>"
    E agora..
    - git add .
    - git commit -m "Iniciando projeto"
    - git flow feature finish
4. Realizei o primeiro lançamento (release)
    - git flow release start 0.0.0
    - git flow release finish 0.0.0
    E o envio para o repositório:
    - git push --all --tags