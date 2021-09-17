## ¿Qué es Docker ? 
Docker es un servicio que permite ejecutar pequeños contenedores de software sobre el
núcleo de nuestro sistema operativo, por lo que es una opción más rápida y liviana que el
uso de máquinas virtuales. Docker utiliza características de aislamiento de recursos del
kernel Linux, tales como cgroups y espacios de nombres (namespaces) para permitir que
"contenedores" independientes se ejecuten dentro de una sola instancia de Linux, evitando
la sobrecarga de iniciar y mantener máquinas virtuales.
La arquitectura Docker es una arquitectura cliente-servidor, donde el cliente habla con el
servidor (que es un proceso daemon) mediante un API para poder gestionar el ciclo de vida
de los contenedores y así poder construir, ejecutar y distribuir los contenedores.

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


