# Laboratório Wazuh com pfSense, Ubuntu Server e Windows Agent

Este repositório documenta um ambiente de laboratório criado durante o curso **Wazuh Expert** da **Green Club**, com o objetivo de simular uma infraestrutura real de segurança da informação, utilizando ferramentas de código aberto para aprendizado prático em SIEM e monitoramento.

---

## Objetivos do Projeto

- Criar um ambiente funcional com Wazuh para centralização e análise de logs.
- Monitorar eventos de segurança em endpoints e rede.
- Simular um cenário corporativo com firewall, servidor SIEM e agente Windows.
- Praticar instalação, configuração e análise de alertas do Wazuh.

---

## Estrutura do Ambiente

O laboratório foi construído em **VMware Workstation**, com as seguintes máquinas virtuais:

| Componente     | Sistema Operacional    | Função                                    |
|----------------|------------------------|-------------------------------------------|
| pfSense        | pfSense 2.x            | Firewall e roteamento                     |
| Wazuh Server   | Ubuntu Server 22.04    | Servidor SIEM e central de gerenciamento  |
| Wazuh Agent    | Windows 11 Pro         | Endpoint monitorado                       |

---

## Diagrama da Topologia

📁 Veja a pasta `/diagrama/` para o esquema de rede entre as VMs.

---

##  Configurações Importantes

### 🔸 pfSense
- Criado para fornecer NAT e controle de tráfego entre as VMs.
- Regras de firewall configuradas para permitir comunicação entre o agente e o servidor Wazuh.

### 🔸 Wazuh Server (Ubuntu)
- Instalação do Wazuh Manager e Dashboard.
- Configuração básica de regras e monitoramento.
- Regras customizadas testadas para eventos do agente Windows.

### 🔸 Windows Agent
- Instalação do Wazuh Agent em **Windows 11 Pro**.
- Registro e comunicação com o servidor Ubuntu.
- Geração de eventos locais para validação da monitoração.

---

## Observações

- O laboratório foi desenvolvido com foco educacional.
- Algumas configurações foram simplificadas para fins de demonstração.
- Ideal para iniciantes em SIEM e profissionais buscando experiência prática com Wazuh.

---

## Tecnologias Utilizadas

- [Wazuh](https://wazuh.com/)
- [pfSense](https://www.pfsense.org/)
- [Ubuntu Server](https://ubuntu.com/)
- [Windows 11](https://www.microsoft.com/)
- [VMware Workstation](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion)

---

## Curso de Referência

Este laboratório foi realizado durante o curso:

**Wazuh Expert - Green Club**  
[https://wazuh-expert.greenn.club](https://wazuh-expert.greenn.club/)

---

## 🤝 Conecte-se

📫 Me adicione no [LinkedIn](https://www.linkedin.com/in/juliorodrigop/)
