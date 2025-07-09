# Configuração da VM - pfSense Firewall

## Especificações da Máquina Virtual

- Sistema operacional: pfSense 2.7.2 (baseado em FreeBSD)
- Tipo de VM: 64 bits
- CPUs: 2 vCPU
- Memória RAM: 20 GB
- Disco: 10 GB (arquivo .vmdk)
- Placas de rede:
  - NIC 1 (WAN): NAT (para acesso à internet)
  - NIC 2 (LAN): VMnet10 (para comunicação com as outras VMs)

## Endereçamento IP

- WAN: IP dinâmico fornecido pelo VMware (via NAT)
- LAN: 192.168.1.1/24

## Configurações Realizadas

- DHCP Server habilitado na interface LAN (opcional, conforme necessidade do ambiente)
- Regras de firewall:
  - Permissão de tráfego LAN → ANY (para permitir comunicação com o Wazuh Server e acesso à Internet)
- NAT configurado automaticamente para permitir saída para a internet a partir da LAN

## Outras Configurações

- WebGUI acessível via: https://192.168.1.1
- Usuário padrão: admin
- Senha: definida durante a instalação
- Configuração inicial realizada via terminal (Setup Wizard)

## Observações

- A interface WAN foi conectada à rede NAT do VMware para garantir acesso externo.
- A interface LAN (VMnet10) foi utilizada para interligar as VMs do Ubuntu Server e do Windows Agent.
- pfSense atua como gateway e firewall entre as máquinas do laboratório, simulando o ambiente de uma rede corporativa.
