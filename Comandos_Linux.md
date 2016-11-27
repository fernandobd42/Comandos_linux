### Cria arquivo
- touch nome

### Edita arquivo
- nano nome

### Exibe conteudo do arquivo
- cat nome

### Cria um diretório
- mkdir nome

### Apaga arquivo ou diretório
- rm nome
- rm -r nome -- Apaga arquivo recursivamente
- rm -f nome -- Apaga arquivo forçosamente

### Apaga diretório
- rmdir nome
- rmdir -r nome -- Apaga diretório recursivamente
- rmdir -f nome -- Apaga diretório forçosamente

### Apaga arquivo ou diretório recursivamente e forçosamente
- rm -Rf

### Exibe informações do arquivo
- file nome
  
### Exibe arquivos e diretórios existenstes no diretório
- dir nome

### Exibe caminho do arquivo
- whereis nome -> ex whereis chromium

### Move arquivo ou pasta
- mv caminhoAtual/nome caminhoNovo/nome

### Renomeia arquivo
- mv nomeAtual nomeNovo

### Copia arquivo ou pasta
- cp caminhoAtual/nome caminhoNovo/nome

### Altera permisão
- chmod permisão nome -> ex: chmod 777 arquivo.txt

### Exibe arquivos e diretórios que estão no diretório atual
- ls
- ls -l -- Exibe permissões dos arquivo e diretórios que estão no diretório atual
- ls -al -- Exibe também arquivos ocultos

- dir
- dir -l -- Exibe permissões dos arquivo e diretórios que estão no diretório atual

### Exibe diretório em que você está 
- pwd

### Exibe os usuários do sistemas
- who
- w -- Exibe usuários atuais
- finger -- Exibe usuários atuais

### Exibe informações sobre determinado domínio da Internet
- whois site -- ex: whois facebook.com

### Exibe informações do sistema
- uname -a

### Exibe todos processos rodando em tempo real
- top

### Mata um processo especifico
- kill pid -- Substituir pid pelo número do proceso

### Exibe processos em tempo real
- ps

### Exibe uso de memória 
- free
- free -h -- Exibe uso de memória em KB, MB, GB 

### Exibe espaço das partições
- df
- df -h -- Exibe o espaço livre/ocupado em KB, MB, GB

### Exibe a quantas horas o computador está ligado
- uptime
- uptime -p -- Exibe horas e minutos

### Exibe data
- date
- uptime -s -- Exibe data, hora, minutos, segundos

### Exibe o calendario
- cal

### Exibe partições
- fdisk -l

### Desmonta partição
- umount partição -> ex: umount /dev/sdc1

### Formata partição
- mkfs.ext4 partição -> ex: mkfs.extr /dev/sdc1

### Instala arquivo .deb
- dpkg -i nome -> ex: dpkg -i nome.deb

### Descompacta arquivo .tar
- tar -xf nome -> ex: tar -xf nome.tar

### Descompacta arquivo .tar.gz ou tar.tgz
- tar -xzf nome -> ex: tar -xf nome.tar.gz

### Descompacta arquivo .tar.bz2
- tar -xjf nome -> ex: tar -xf nome.tar.bz2

### Descompacta arquivo .tar.xz
- tar -xJf nome -> ex: tar -xf nome.tar	

### Cancela o comando atual em funcionamento
- ctrl+c

### Para o comando atual
- ctrl+z

### Loga root
- su

### Faz logout da sessão atual; similar ao comando exit
- ctrl+d 
- exit

### Apaga uma palavra na linha atual
- ctrl+w 

### Apaga a linha inteira
- ctrl+u

### Mostra um comando recente
- ctrl+r 

### Repete o último comando 
- !!

### Exibe variáveis de ambiente
- env

### Escreve todos os dados presentes nos buffers da memória para o disco
- sync

### Exibe ips da máquina
- ifconfig
- ifconfig ethO --Exibe configurações da interface de rede eth0
- ifconfig wlan0 -- Exibe configurações do wireless wlan0

### Exibe ping de determinado ip
- ping ip -> ex: ping 192.168.0.122 ou www.google.com

### Exibe portas abertas num dado host
- nmap -> ex: nmap 192.168.0.121 ou www.google.com

### Exibe jobs em execução
- jobs

### Mata job
- jobs -9 %numero -> ex: jobs -9 %2

### Lista os processos em execução
- ps

### Mata processo
- kill pid -> ex: kill 5452

### Exibe o estado da rede
- netstat

### Exibe os atalhos do shell
- alias

### Instala um programa
- apt-get install nome -> ex: apt-get install chromium

### Remove os pacotes mas os arquivos de configuração ficam intactos
- apt-get remove nome -> ex: apt-get remove chromium

### Remove os pacotes e os arquivos de configuração
- apt-get --purge remove nome -> ex: apt-get --purge remove chromium

### Baixa a lista com os pacotes disponiveis
- apt-get update

### Atualiza os pacotes sistema
- apt-get upgrade
- apt-get -u upgrade -- Mostra os pacotes que estão sendo atualizados

### Atualiza a distribuição intiera
- apt-get dist-upgrade

### Inicia um programa
- service nome start -> ex: service mysql start

### Pausa um programa
service nome stop -> ex: service mysql stop

### Reinicia um programa
service nome restart -> ex: service mysql restart

### Desliga o computador
- shutdown

### Reinicia o computador
- restart

### Exibe informações de um comando
- man comando -> ex: man grep

### Lista os processo em execução
- ps aux

### Lista a quantidade de arquivos de acordo com a extensão
- ls | cut f2 -sd. | sort | uniq

### Calcula Fatorial
- seq -s \* numero -- ex: seq -s \* 10 -- Exibe a sequencia de 10 à 1, separando um numero do outro com *(operador de vezes)
- seq -s \* numero | bc -- ex: seq -s \* 10 | bc -- Exibe o resultado do fatorial de 10
