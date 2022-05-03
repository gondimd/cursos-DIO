# cursos-DIO  :books:


### GERACAO DE CHAVES:

- Git init (comando para inicializar o git em determinada pasta)

GERAR CHAVE CRIPTOGRAFADA PARA O GITHUB

- Ssh-keygen –t ed25519 –C email@gmail.com   (gera a chave)

 - Pwd – mostra o caminho completo das pastas
 - Cd /c/Users/user/.ssh

### Acessar o diretório oculto ~/.ssh  e digitar o seguinte comando:
- $ cat id_ed25519.pub  (tem q ser este arquivo pq ele é a chave publica)
- ssh-ed25519 chave email@gmail.com

### INICIALIZAR O SSH AGENT, ele pega as chaves e gerir elas:
No diretório do ~/.ssh   digitar:
- Eval $(ssh-agent –s)
- Logo ele starta o proj. pra rodar em plano de fundo
- Git config –list  (lista as conf. Do seu repositorio)
- Ssh-add id_ed25519   (passa a chave privada para descriptografar a chaves publica)

### RESETAR CONF. DOS REPOSITORIOS, EXEMPLO: ALTERAR EMAIL
 - Git config –global –unset user.email

 - Git config –global –unset user.Name

ADD NOVO EMAIL:
- Git config –global user.mail email@gmail.com

Se vc usou um usuario e email diferente no github, eles vao aparecer diferentes la.
__________________________________________________________________________________________


### CONFIGURANDO O REPOSITORIO
1- NO BASH  (clica lado direito do mouse dentro da pasta onde será seu repositório)

	- Git init 
	
	- Git remote add origin https://github.com/gondimd/livro-receitas.git

Git remote –v (lista de repositories remotos que tenho cadastrado) 

	- Git status (verifica se há alguma pendencia)
	
	- Git push  origin master (origin é um alias q vc atribui para não ficar precisando digitar toda vez o endereço da URL) Este comando envia para o repositório web.
	- OBSERVAÇÃO: caso ocorra falha para realizar o commit no git, faça primeiro o comando "git pull" _ para pegar o que esta no repositorio web e atualizar o repositório local, em seguinda faça o "git push" para empurrar a ultima atualizacao que foi feita no repositório local.

### FORMA MAIS PRATICA DE REALIZAR A CRIACAO DO REPOSITORIO
1-	CRIAR CONTA NO GIT HUB
2-	EM SEGUIDA CRIAR O REPOSITORIO NO GITHUB WEB, NO BOTAO ‘CODE’ Copiar o endereço da HTTPS do projeto.
3-	Na pasta em seu pc que vai ser usada como repositorio, clicar com o lado direito do mouse e clicar em GITBASH here (Obs: instalar o GITBASH ANTES), ao abrir o terminal do gitbash digitar o seguinte comando:

 - Git clone https:// endereço que esta no githun

Para realizar os commits:

- git add *  (* ou . )
- git commit -m "coloque a informacao sobre este commit"   (faz o commit para repositorio local)
- git push origin master ou apenas "git push" ("empurra" o que foi comitado para o repositorio web)
