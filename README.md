<img alt="Docker" src="https://uilicious.com/blog/content/images/2019/06/x5qc7fcydza4gzjjyq7d.png" />

<h3 align="center">
Messageria Docker NodeJS
</h3>

<blockquote align="center">“Nada no mundo supera a persistência.”!</blockquote>

## :rocket: Instalação do Node.js - Windows, Mac e Linux
O Node.js é uma ferramenta que nos permite executar JavaScript fora do navegador, no lado do servidor. Ele foi um dos responsáveis por popularizar o JavaScript em diversas áreas.
* LTS é uma versão que tem um suporte mais prolongado, porém, costuma ser mais antiga. Ela é focada em estabilidade e segurança. Essa versão é mais recomendada para grandes projetos, que precisam de uma versão mais estável e que não podem ficar sendo atualizados.
* Em contrapartida temos a Current, a versão mais atual com todas as novas funcionalidades, muito indicada para testes, estudos e novos projetos. Cada nova versão pode ter atualizações que podem quebrar um código que foi escrito em uma versão mais antiga. Portanto, é preciso tomar cuidado ao atualizar projetos para novas versões.

Acesse o site do Node:
```
https://nodejs.org/en/
```
##### Instalação em Windows
Logo após selecionar uma versão (LTS ou Current), será iniciado o download do instalador para Windows. Assim como é comum nos instaladores do Windows, basta seguir clicando nos botões Next até chegar ao final da instalação.

Assim que a instalação for finalizada, precisaremos testar se tudo está certo. Então, inicie o seu terminal. Pressione Tecla Windows + R, com a finalidade de abrir o programa Executar. Escreva powershell e aperte a tecla Enter.

Em seguida, no terminal digite node -v e aperte a tecla Enter. Caso seja exibida a versão do Node, sua instalação foi feita com sucesso!
##### Instalação em Linux
Podemos instalar o Node.js facilmente com o próprio gerenciador de pacotes do Linux. Inicie o terminal pressionando Ctrl + Alt + T.

No terminal, digite o comando de instalação do curl:
```
sudo apt-get install curl
```
Em seguida, execute o script abaixo para adicionar o repositório do Node:
```
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
```
E por fim, para instalar o Node execute:
```
sudo apt-get install -y nodejs
```
Logo depois da instalação, no terminal digite node -v e aperte a tecla Enter. Se acaso a versão do Node for exibida, sua instalação foi feita com sucesso!
##### Instalação em Mac
Logo após selecionar uma versão (LTS ou Current), será iniciado o download do instalador para Mac (arquivo .pkg). Assim que abrir esse arquivo, o instalador será iniciado.

Basta ir clicando para continuar até ele finalizar a instalação.

Precisamos testar se tudo está certo. Então, inicie o seu terminal. Para isso, pressione Command + Barra de Espaço. Digite terminal e pressione Enter.

Em seguida, no terminal digite node -v e aperte a tecla Enter. Caso seja exibida a versão do Node, sua instalação foi feita com sucesso!

## :rocket: Instalação do Docker - Windows, Mac e Linux
Docker é um conjunto de produtos de plataforma como serviço que usam virtualização de nível de sistema operacional para entregar software em pacotes chamados contêineres. Os contêineres são isolados uns dos outros e agrupam seus próprios softwares, bibliotecas e arquivos de configuração.

Acesse o site do Docker:
```
https://www.docker.com/
```
##### Instalação em Windows
Na versão desktop, você pode instalar utilizando o Docker for Windows (caso esteja utilizando Windows 10 pro) ou o Docker ToolBox (Se estiver usando outras versões do Windows neste caso irei mostrar apenas a instalação no windows 10 pro).

O Docker para Windows agora requer o Hyper-V da Microsoft. Uma vez ativado, o VirtualBox não será mais capaz de executar máquinas virtuais (suas imagens VM ainda permanecerão). Você ainda pode usar docker-machinepara gerenciar hosts remotos.

Você tem a opção de importar a defaultVM após instalar o Docker para Windows no menu Configurações na bandeja do sistema.

O Docker para Windows ativa o Hyper-V se necessário; isso requer uma reinicialização.

O Docker para Windows é executado no Windows 10 Pro, Enterprise e Education de 64 bits; 1511 Atualização de novembro, Compilação 10586 ou posterior. O Docker planeja oferecer suporte a mais versões do Windows 10 no futuro.

link para instalar:
```
https://download.docker.com/win/beta/InstallDocker.msi
```
Clique duas vezes InstallDocker.msipara executar o instalador.

Siga o assistente de instalação: aceite a licença, autorize o instalador e prossiga com a instalação.

Clique em Concluir para iniciar o Docker.

O Docker é iniciado automaticamente.

O Docker carrega uma janela de “Boas-vindas” com dicas e acesso à documentação do Docker.

A baleia na barra de status indica uma instância do Docker em execução (e acessível via terminal).

Verifique se o Docker Engine está instalado corretamente executando a hello-world imagem(digite no terminal):
```
docker run hello-world.
```
##### Instalação em Linux
Para instalar o Docker Engine, você precisa da versão de 64 bits de uma destas versões do Ubuntu:
* Ubuntu Hirsute 21.04
* Ubuntu Groovy 20.10
* Ubuntu Focal 20.04 (LTS)
* Ubuntu Bionic 18.04 (LTS)

Docker motor é suportado em x86_64(ou amd64), armhf, arm64e s390x arquiteturas.

Atualize o aptíndice do pacote e instale os pacotes para permitir o aptuso de um repositório sobre HTTPS:
```
sudo apt-get update && sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
```
Adicione a chave GPG oficial do Docker:
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
Atualize o aptíndice do pacote e instale a versão mais recente do Docker Engine e containerd ou vá para a próxima etapa para instalar uma versão específica:
```
sudo apt-get update && sudo apt-get install docker-ce docker-ce-cli containerd.io
```
Verifique se o Docker Engine está instalado corretamente executando a hello-world imagem(digite no terminal):
```
sudo docker run hello-world
```
##### Instalação em Mac
O macOS deve ser a versão 10.14 ou mais recente . Ou seja, Mojave, Catalina ou Big Sur. Recomendamos atualizar para a versão mais recente do macOS.

Se você tiver problemas após atualizar seu macOS para a versão 10.15, deverá instalar a versão mais recente do Docker Desktop para ser compatível com esta versão do macOS.

Pelo menos 4 GB de RAM.

O VirtualBox anterior à versão 4.3.30 não deve ser instalado, pois não é compatível com o Docker Desktop.

link para instalar chip da Intel:
```
https://desktop.docker.com/mac/stable/amd64/Docker.dmg?utm_source=docker&utm_medium=webreferral&utm_campaign=docs-driven-download-mac-amd64
```
link para instalar chip da Apple(M1):
```
https://desktop.docker.com/mac/stable/arm64/Docker.dmg?utm_source=docker&utm_medium=webreferral&utm_campaign=docs-driven-download-mac-arm64
```

Clique duas vezes Docker.dmg para abrir o instalador e arraste o ícone do Docker para a pasta Aplicativos.

Clique duas vezes Docker.app na pasta Aplicativos para iniciar o Docker.

O menu Docker exibe a janela Acordo de serviço de assinatura do Docker. Inclui uma mudança nos termos de uso do Docker Desktop.

Verifique se o Docker Engine está instalado corretamente executando a hello-world imagem(digite no terminal):
```
docker run hello-world.
```
