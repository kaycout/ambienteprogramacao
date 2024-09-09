# Preparação de ambiente
### Vamos preparar o ambiente para desenvolvimento de aplicações

#### Nesta preparação iremos instalar e configurar os seguintes recursos:
 - Máquina virtual (VirtualBox)
 - Distribuição Linux (Ubuntu Server)
 - Nasm
 - Compilador da linguagem C
 - Configurar o IP e a porta de comunicação entre a máquina real e virtual
 - Configurar o acesso via SSH entre o VSCode e o servidorLinux
 - Instalar as extensões: Material Icon, Nasm, SSH e linguagem C/C++ 

 #### Máquina virtual (VirtualBox)

 !["Logo Virtualbox"](virtualbox.png)


 Máquina virtual é uma ferramenta que permite a criação de novos computadores e a instalação de sistemas operacionais, para estudo ou trabalho.

 Para nosso estudo iremos usar o Virtualbox da Oracle.
 Para fazer Download no link a seguir:

 <a href="https://www.virtualbox.org/wiki/Downloads" target="_blank"> Virtualbox </a>

 ##### Criando a máquina virtual para o nosso estudo.

 - Configuração:
  > - Nome da máquina: Servidor
  > - Memória: 4 GB (4096)
  > - Processador: 2 
  > - Disco 100GB
  > - IP e porta do host: IP 127.0.0.1 e porta 22.
  > - IP e porta do convidado: 10.0.2.15 e 22.

- Tela inicial de configuração

<img src=configinicial_virtualbox.png width=1000 height=200>

- Configuração do Hardware

<img src=configmemoria.png width=1000 height=200>

- Tela de configuração do Disco

<img src=configdisco.png width=1050 height=200>

- Tela final de configuração

<img src=partefinal.png width=1050 height=200>

- Tela de configuração da rede

<img src=configdarede.png width=1200 height=250>

- Tela de configuração de portas e IP

<img src=configporta_ip.png width=1800 height=200>

#### Distribuição Ubuntu Server

Para o nosso estudo iremos utilizar uma distribuição Linux para servidores chamada Ubuntu. 

Acompanhe o processo de instalação 

Faça o download aqui:

<a href="https://ubuntu.com/download/server"
target="_blank"> Ubuntu Server </a>


!["S.O (Ubuntu server)"](ubuntu.server.png)

- Acompanhe a instalação:

- Tela de início de instalação
<img src=ubuntuinstall01.png width=1800 height=200>
- Tela de seleção de idioma
<img src=configidioma.png width=1800 height=200>
- Tela de seleção de teclado
<img src=selecionar_teclado.png width=1800 height=200>
- Tela de tipo de instalação
<img src=tipodeinstalacao.png width=1800 height=200> 
- Tela de configuração de rede
<img src=config_rede.png width=1800 height=200>
- Tela de configuração do Proxy
<img src=config_proxy.png width=1800 height=200>
- Tela de pacotes de atualização
<img src=tipodeinstalacao.png width=1800 height=200>
- Tela de configuração do disco
<img src=config_disco.png width=1800 height=200>
- Tela layout do disco
<img src=configlayout.png width=1800 height=200>
- Tela de configuração de rede
<img src=config_rede.png width=1800 height=200>
- Tela de configuração do usuário
<img src=config_do_usuario.png width=1800 height=200>
- Tela de configuração do SSH
<img src=configSSH.png width=800 height=300>
- Tela do fim da instalação
<img src=fimdainstall.png width=1800 height=250>

#### Atualização do Sistema 

Para a correta utilização do servidor Ubuntu que acabamos de instalar, será necessário realizar a atualização do sistema.

- Execute o comando abaixo:

```
sudo apt update -y && sudo apt upgrade -y
```

- Reinicie o seu servidor usando o comando abaixo:

```
reboot 
```
#### Instalação do Compilador NASM

O compilador do NASM é uma ferramenta que nos permite programar em Assembly. Assim é possivel criar programas que manipulam dados que estão nos registradores do processador.

- Para instalar o NASM no Ubuntu, usamos o comando:

```
sudo apt install nasm -y
```
#### Instalação do compilador da linguagem C

Em Linux o compilador da lingugem C é o GCC. Ele é uma ferramenta importante para o desenvolvimento de programas em C.

Para instalar o comando:
```
sudo apt install gcc -y
```
#### Conexão servidor e VScode via SSH

Precisamos instalar uma extensão no VScode para acessar o nosso servidor de forma remota.

!["Extensão SSH](extensaossh.png)

Configuração do acesso remoto.

!["Configuração](configurarextensao.png)



