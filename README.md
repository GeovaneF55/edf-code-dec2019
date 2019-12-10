# edf-code (Preparação de Ambiente)

# Windows

## Passo 1
* Acesse [https://www.mongodb.com/](https://www.mongodb.com/) e baixe a última versão do mongodb para windows

## Passo 2
* Acesse [https://nodejs.org/en/](https://nodejs.org/en/) e baixe a última versão do node LTS

## Sugestão
* Acesse [https://cmder.net/](https://cmder.net/) e baixe a versão full que vem com git
**OU**
* Acesse [https://desktop.github.com/](https://desktop.github.com/) e baixe a versão do git para desktop

## Passo 3
* Acesse [https://code.visualstudio.com/](https://code.visualstudio.com/) e baixe o visual studio code (pode usar o sublime ou o atom)

## Sugestão
* Caso tenha preferido baixar o cmder, cole a pasta (após descompactá-la) em Arquivos de Programas

## Passo 4
* Para instalar o mongodb, clique no instalador e siga os passos do wizard

* Após instalado, é preciso ir em **Meu Computador->Propriedades->Configurações Avançadas do Sistema->Váriáveis de Ambiente**

* Clique em **Path** na aba Avançado em Variáveis do Sistema e depois clique em **Editar**

* No final da String Valor da variável, é necessário adicionar o caminho do mongodb, possivelmente **C:\Program Files\MongoDB\Server\3.4\bin**

**OBS:** Lembre-se de adicionar um **;** antes do caminho para que o sistema saiba que é uma nova variável de ambiente

* Para testar se o mongodb está funcionando, vá no terminal do sistema, ou no cmder instalado, e digite **mongod**

**OBS:** o MongoDB exige que exista um diretório em **C:\data\db**, logo é necessário criar esse diretório para que o mongo funcione corretamente

## Passo 5
* Para instalar o node, clique no instalador e siga os passos do wizard

* Para testar se o node está funcionando, vá no terminal do sistema, ou no cmder instalado, e digite **node -v**

* Para testar se o npm está funcionando, vá no terminal do sistema, ou no cmder instalado, e digite **npm -v**

## Passo 6
* Para instalar o vscode, clique no instalador e siga os passos do wizard

* Para testar se o vscode está funcionando, vá no terminal do sistema, ou no cmder instalado, e digite **code .**

# Linux
## Passo 1
* Acesse [https://www.mongodb.com/](https://www.mongodb.com/) e baixe a última versão do mongodb para linux

## Passo 2
* Acesse [https://nodejs.org/en/](https://nodejs.org/en/) e baixe a última versão do node LTS

## Passo 3
* Acesse [https://code.visualstudio.com/](https://code.visualstudio.com/) e baixe o visual studio code (pode usar o sublime ou o atom)

## Passo 4
* Para instalar o node, descompacte o arquivo **.tar.xz** e renomeie a pasta descompactada para **node**

* Mova a pasta **node** decompactada utilizando o seguinte comando: **sudo mv node /opt/node**

* Vá para o novo diretório do node com o comando: **cd /opt/node/**

* Altere as váriaveis de ambiente com: **sudo nano /etc/enviroment** ou **sudo vim /etc/enviroment**

* No final do path adicione um novo registro com **:/opt/node/bin** e salve a alteração

* Execute o comando **source /etc/enviroment** para que o sistema reconheça o node como variável de sistema

* Para testar se o node está funcionando, execute **node -v**

* Para testar se o npm está funcionando, execute **npm -v**

## Passo 5
* Para instalar o mongodb, descompacte o arquivo **.tgz** e renomeie a pasta descompactada para **mongodb**

* Mova a pasta **mongodb** decompactada utilizando o seguinte comando: **sudo mv mongodb /opt/mongodb**

* Vá para o novo diretório do node com o comando: **cd /opt/mongodb/**

* Altere as váriaveis de ambiente com: **sudo nano /etc/enviroment** ou **sudo vim /etc/enviroment**

* No final do path adicione um novo registro com **:/opt/mongodb/bin** e salve a alteração

* Execute o comando **source /etc/enviroment** para que o sistema reconheça o mongodb como variável de sistema

**OBS:** O MongoDB exige que exista um diretório em **/data/db**, logo é necessário criar esse diretório para que o mongo funcione corretamente

* Execute os seguintes comandos:

**mkdir /data**

**mkdir /data/db**

* É precido trocar a permissão da pasta para o usuário logado, sendo assim execute:

**whoami**

* O resultado do último comando é o seu usuário: (usuário)

**sudo chown (usuário):(usuário) -R /data**

* Para testar se o mongodb está funcionandom, execute **mongod**

## Passo 6
* Para instalar o vscode, execute o instalador e siga os passos do wizard
