Vagrant [BemFuncional]
===========

Servidor LAMP (Linux, Apache, MySQL, PHP)

Configuração Vagrant - Criação de máquina virtual (Ubuntu Server 14.04 64 Bits) de desenvolvimento em PHP.

### Pacotes Inclusos:

- PHP 7.1
- MySQL 5.5
- Git
- PhpMyAdmin 
- Composer
- cURL
- Vim
- Redis
(Para mais detalhes consulte arquivo setup.sh)


Você vai precisar: 
==============

- Virtualbox - https://www.virtualbox.org/
- Vagrant - http://www.vagrantup.com/
- Git - http://git-scm.com ( Opicional )
- Acesso Internet

-> Instale o Virtualbox e o Vagrant de acordo com seu sistema operacional. 


Modo de Uso
===========

A instalação inicial pode ser feita de duas formas, sendo:

1º -> Caso tenha o Git instaldo em sua máquina, proceda da seguinte forma:



* Clone esse repositório para sua máquina:

- git clone https://github.com/BemFuncional/vagrant.git ( Execute o comando no seu Prompt/Terminal )

* Ainda no Prompt de comando/Terminal Entre no diretório vagrant  ( Ou o que você definir na hora da clonagem )

* Inicie a máquina virtual com o comando:

- vagrant up 




2º -> Caso não tenha o Git instalado em sua máquina, acesse https://github.com/BemFuncional/vagrant baixe o arquivo do projeto no formato .zip e descompacte-o onde desejar.

* Abra seu Windows Power Shell, acesse o diretorio que acabou de descompactar e rode o comando:

- vagrant up




Após este comando 'vagrant up', o Vagrant ficará responsavel por baixar o sistema operacional (neste caso Ubuntu Server 14.02 64bits), e configurar a máquina virtual no VirtualBox e posteriormente baixar, instalar e configurar todos os pacotes do script 'setup.sh'.

Quando tudo estiver pronto, um servidor web estará disponível no endereço http://localhost:8080, e a instalação do PHPMyAdmin está em http://localhost:8080/phpmyadmin, para acessar utilize:

- Login: root
- Senha: vagrant

obs:(A senha padrão para todos os serviços é vagrant).


Coloque seu código no diretório "www". Todo o conteúdo dele estará disponível via http://localhost:8080. (Como teste, já existe um arquivo index.php que chama a função phpinfo() ).

Para desligar a máquina virtual utilize o comando:

- vagrant halt

Para religar novamente utilize:

- vagrant up

Caso queira destruir a máquina virtual (o conteúdo do www não será excluido):

- vagrant destroy
