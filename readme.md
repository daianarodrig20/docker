## Primero para asegurarse de que no haya ninguna version corriendo de docker corro la linea 
sudo apt-get remove docker docker-engine docker.io containerd runc

## Para instalarlo debemos instalar estas dependecias
 sudo apt-get update
 sudo apt-get install \
     apt-transport-https \
     ca-certificates \
     curl \
     gnupg \
     lsb-release

## Agregue la clave GPG oficial de Docker
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

## Hago un apt update para actualizar lo instalado

# Instalacion de Docker
sudo apt-get install docker-ce docker-ce-cli containerd.io

## Verificar que se instalo
docker run hello-world


