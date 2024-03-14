# WSL

Windows Subsystem for Linux é um módulo dos sistemas operacionais Windows 10 e 11, que visa disponibilizar um ambiente Linux compatível no sistema Microsoft, de forma que se possam executar progamas nativos dos sistemas GNU/Linyx dentro do Windows sem a necessidade de VM.

### Instalando uma distribuição 

Por padrão  o WSL instala como distribuição o ubuntu utilizando:
```
wsl --install
```

Para listar as distribuições
```
wsl --list --online
```

Para instalar outra distribuição
```
wsl --install -d nomeDistribuicao
```

Verificar a versão do WSL configurada
```
wsl -l -v
```

### Comandos básicos Linux
Trocar senha de um usuário
```
sudo passwd nomeUsuario
```
Trocar de usuário
```
su nomeUsuario
```
Atualização dos pacotes do repositório
```
sudo apt update
```
Informações do sistema Linux
```
uname -a
```
Criação de usuário
```
sudo useradd nomeUsuario
```

Habilitar recursos de rede
```
sudo rm /etc/resolv.conf
sudo bash -c 'echo "nameserver 8.8.8.8" > /etc/resolv.conf'
sudo bash -c 'echo "[network]" > /etc/wsl.conf'
sudo bash -c 'echo "generateResolvConf = false" >> /etc/wsl.conf'
sudo chattr +i /etc/resolv.conf
```

Atualizar pacotes instalados no sistema
```
sudo apt update && sudo apt full-upgrade
```