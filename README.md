# 👩‍💻 Introdução a Git & Github
<p align="center">
<img src="./assets/logo_elas.png" heigth="80" width="180"/>
<img src="./assets/opendevufcg_icon.png" heigth="50" width="110"/>
<p/>

## O que é Git?  

Git é um sistema open-source de controle de versão que se tornou muito popular e hoje é amplamente utilizado por desenvolvedores ao redor do globo, oferecendo muitas funcionalidades. Mas, por que devemos nos preocupar em ter um controle de versão? 

Em resumo: se você vai desenvolver um sistema sozinho ou em equipe, o Git vai registrar as alterações do arquivo -ou conjunto de arquivos- ao longo do tempo, permitindo que você possa recuperar alguma versão específica. O git também permite que você divida as funcionalidades do sistema, podendo atribuí-las a diferentes pessoas e, ao final do projeto, você pode juntar todas essas funcionalidades em um único sistema.   

## O que é Github?

Bem, o Github é uma plataforma para hospedagem de código-fonte e repositórios Git, contendo ainda funcionalidades próprias e permitindo que pessoas acessem projetos privados ou Open Source de qualquer lugar do mundo. 


## Instalando o Git

#### Para começar, é preciso ter o Git instalado na sua máquina e também ter uma conta no Github

- Para sistemas baseados em Debian/Ubuntu, execute o comando:

    ```$ apt-get install git```

- Para o Ubuntu, esta PPA oferece a versão mais atual e estável do Git: 

    ```
    $ add-apt-repository ppa:git-core/ppa
    $ apt update 
    $ apt install git
    ```
    Assim que finalizar a instalação, utilize o comando ```git --version```para ter certeza de que tudo ocorreu bem.
    
- Se você utiliza outro sistema (Linux/Unix, Windows ou MacOS), [clique neste link](https://git-scm.com/downloads).

## Configuração inicial do Git

#### Para começar a utilizar o Git, é necessário que você configure os dados da sua conta do Github

    $ git config --global user.name "Seu UserName"
    $ git config --global user.email seuemail@exemplo.com

Se você quiser checar todas as configurações possíveis, [clique neste link](https://www.git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup).

##  Criando seu primeiro repositório

#### Criando um repositório local e conectando ele com um repositório remoto
1. Primeiro, certifique-se de que você está no diretório desejado e então crie a pasta. 
	 Se você preferir, pode fazer isso pelo terminal, por exemplo: 
	```
	$ cd Documentos/
	$ mkdir minha-pasta
	```
	
2. Depois de criar a pasta, você deve ir até ela e iniciá-la como um repositório:
	```
	$ cd minha-pasta/
	$ git init
	```

	Para se certificar de que tudo deu certo, digite:
	```$ git status```
	
	Irá aparecer uma mensagem dizendo *No commits yet*. Isso quer dizer que seu repositório foi criado, mas ele ainda está vazio. Por enquanto deixaremos assim. 
3. Agora, vá até sua página do Github e para criar um repositório remoto clique em **New**.

	![Alt](https://uploaddeimagens.com.br/imagens/3C8aMn0)

	Digite o nome do repositório (que deve ser igual ao nome da pasta criada). Apenas o nome já é suficiente pra criar o repositório. No final da página, clique em **CreateRepository**

	![repositorio](https://ibb.co/q0XCTR2)
	
4. Agora, é hora de conectar o repositório local ao repositório remoto!
	
	Vá até o seu repositório remoto, clique em **Code** e copie o link HTTPS.
	
	![Alt](https://ibb.co/b2F82Yq)

	Agora, volte ao terminal e digite:
	
	```$ git remote add origin https://github.com/seuuser/minha-pasta.git```


5. Como o seu repositório local ainda está vazio, vamos adicionar um arquivo nele. Você pode usar um editor de texto qualquer para criar um arquivo e salvar na sua pasta, 
ou pode executar o comando: 

	```$ echo "# minha-pasta" >> README.md ```
	
6. Depois, adicione essa alteração no seu repositório:
	```$ git add README.md```
	
	**Obs**: se você tiver adicionado um arquivo na sua pasta de outra forma, 
	digite apenas ```$ git add .```
	
7. Commite a alteração para o seu repositório remoto:
	 ```$ git commit -m "first commit"```

8. Agora, você pode enviar todas as alterações do seu repositório local de vez para o repositório remoto: 
```$ git push -u origin master```

	Serão solicitados seu username e sua senha. Depois de digitá-los,
	uma mensagem parecida com esta deve aparecer:
	
	> Total 3 (delta 0), reused 0 (delta 0)
	To https://github.com/seuuser/minha-pasta.git
	[new branch]      master -> master

 Prontinho! Você criou seu primeiro repositório local e enviou todas as alterações feitas nele para um 	repositório remoto!
