#!/bin/bash

if [ "$1" == "hostname" ]; then
    hostname
    exit
elif [ "$1" == "disk" ]; then
    df -h
    exit
else
    echo "Uso: $0 {hostname|disk}"
    exit 1
fi




# Coletor de Dados Script
Esse script coleta alguns dados com base no argumento
especificado pelo usuario (hostname, uptime, disck, e
all)

### Exemplos
` ./minfo.sh hostname - mostra o nome da maquina `
` ./minfo.sh uptime - mostra o tempo que a maquina esta ligada`
