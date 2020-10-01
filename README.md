# 👩‍💻 Introdução a Git & Github
<p align="center">
<img src="./assets/logo_elas.png" heigth="80" width="180"/>
<img src="./assets/opendevufcg_icon.png" heigth="80" width="180"/>
<p/>


## O que é Git?  

Git é um sistema open-source de controle de versão que se tornou muito popular e hoje é amplamente utilizado por desenvolvedores ao redor do globo, oferecendo muitas funcionalidades. Mas, por que devemos nos preocupar em ter um controle de versão? 

Em resumo: se você vai desenvolver um sistema sozinho ou em equipe, o Git vai registrar as alterações do arquivo -ou conjunto de arquivos- ao longo do tempo, permitindo que você possa recuperar alguma versão específica. O git também permite que você divida as funcionalidades do sistema, podendo atribuí-las a diferentes pessoas e, ao final do projeto, você pode juntar todas essas funcionalidades em um único sistema.   

## O que é Github?

Bem, o Github é uma plataforma para hospedagem de código-fonte e repositórios Git, contendo ainda funcionalidades próprias e permitindo que pessoas acessem projetos privados ou Open Source de qualquer lugar do mundo. 


## Instalando o Git

#### Para começar, é preciso ter o Git instalado na sua máquina

- Para sistemas baseados em Debian/Ubuntu, execute o comando:

    ```apt-get install git```

- Para o Ubuntu, esta PPA oferece a versão mais atual e estável do Git: 

    ```
    add-apt-repository ppa:git-core/ppa
    apt update 
    apt install git
    ```

- Se você utiliza outro sistema (Linux/Unix, Windows ou MacOS), [clique neste link](https://git-scm.com/downloads).

## Configuração inicial do Git

#### Para começar a utilizar o Git, é necessário que você configure os dados da sua conta do Github

    # git config --global user.name "Seu UserName"
    # git config --global user.email seuemail@exemplo.com

Se você quiser checar todas as configurações possíveis, [clique neste link](https://www.git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup).


