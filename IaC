#!/bin/bash
set -e

echo "INICIANDO CONFIGURAÇÂO!!!!"

# Criar pastas
echo "Criando pastas . . . . "
mkdir -m 777 publico
mkdir -m 2770 adm
mkdir -m 2770 ven
mkdir -m 2770 sec

# Criar grupos
echo "Criando grupos . . . . "
groupadd GRP_ADM
groupadd GRP_VEN
groupadd GRP_SEC

# Associar pastas aos grupos
echo "Associando pastas aos grupos . . . . . "
chown :GRP_ADM adm
chown :GRP_VEN ven
chown :GRP_SEC sec

# Usuários do GRP_ADM
echo "Criando usuarios do GRP_ADM . . . . "
useradd -m -s /bin/bash -c "Carlos Silva" -g GRP_ADM -p $(openssl passwd -6 "teste") carlos
useradd -m -s /bin/bash -c "Maria Silva" -g GRP_ADM -p $(openssl passwd -6 "teste") maria
useradd -m -s /bin/bash -c "João Silva" -g GRP_ADM -p $(openssl passwd -6 "teste") joao

# Usuários do GRP_VEN
echo "Criando usuarios do GRP_VEN . . . . "
useradd -m -s /bin/bash -c "Debora Silva" -g GRP_VEN -p $(openssl passwd -6 "teste") debora
useradd -m -s /bin/bash -c "Sebastiana Silva" -g GRP_VEN -p $(openssl passwd -6 "teste") sebastiana
useradd -m -s /bin/bash -c "Roberto Silva" -g GRP_VEN -p $(openssl passwd -6 "teste") roberto

# Usuários do GRP_SEC
echo "Criando usuarios do GRP_SEC . . . . "
useradd -m -s /bin/bash -c "Josefina Silva" -g GRP_SEC -p $(openssl passwd -6 "teste") josefina
useradd -m -s /bin/bash -c "Amanda Silva" -g GRP_SEC -p $(openssl passwd -6 "teste") amanda
useradd -m -s /bin/bash -c "Rogerio Silva" -g GRP_SEC -p $(openssl passwd -6 "teste") rogerio

echo "CONFIGURAÇÃO CONCLUÍDA COM SUCESSO!!!!"
