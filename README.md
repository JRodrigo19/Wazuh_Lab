# Wazuh Lab with pfSense, Ubuntu Server, and Windows Agent / Laboratório Wazuh com pfSense, Ubuntu Server e Windows Agent

This repository documents a hands-on lab environment created during the **Wazuh Expert** course by **Green Club**, aiming to simulate a real-world information security infrastructure using open-source tools.

Este repositório documenta um ambiente de laboratório criado durante o curso **Wazuh Expert** da **Green Club**, com o objetivo de simular uma infraestrutura real de segurança da informação utilizando ferramentas de código aberto.

---

## 🎯 Project Objectives / Objetivos do Projeto

- Build a functional Wazuh environment for centralized log analysis.
- Monitor security events across endpoints and network.
- Simulate a corporate scenario with a firewall, SIEM server, and Windows agent.
- Practice Wazuh installation, configuration, and alert analysis.

- Criar um ambiente funcional com Wazuh para centralização e análise de logs.
- Monitorar eventos de segurança em endpoints e rede.
- Simular um cenário corporativo com firewall, servidor SIEM e agente Windows.
- Praticar instalação, configuração e análise de alertas do Wazuh.

---

## 🖥️ Lab Environment Structure / Estrutura do Ambiente

The lab was built using **VMware Workstation** and includes the following virtual machines:

O laboratório foi construído em **VMware Workstation**, com as seguintes máquinas virtuais:

| Component / Componente | Operating System / Sistema Operacional | Role / Função |
|------------------------|----------------------------------------|---------------|
| pfSense                | pfSense 2.x                            | Firewall and routing / Firewall e roteamento |
| Wazuh Server           | Ubuntu Server 22.04                    | SIEM server and management dashboard / Servidor SIEM e central de gerenciamento |
| Wazuh Agent            | Windows 11 Pro                         | Monitored endpoint / Endpoint monitorado |

---

## 🧭 Network Topology Diagram / Diagrama da Topologia

📁 See the `/diagrama/` folder for the full network topology between the VMs.  
📁 Veja a pasta `/diagrama/` para o esquema de rede entre as VMs.

---

## ⚙️ Key Configurations / Configurações Importantes

### 🔸 pfSense
- Provides NAT and traffic control between virtual machines.
- Firewall rules allow communication between agent and server.

- Fornece NAT e controle de tráfego entre as VMs.
- Regras de firewall permitem comunicação entre o agente e o servidor.

### 🔸 Wazuh Server (Ubuntu)
- Wazuh Manager and Dashboard installed and configured.
- Custom rules tested for agent event detection.

- Instalação do Wazuh Manager e Dashboard.
- Regras customizadas testadas para eventos do agente.

### 🔸 Windows Agent
- Installed and registered with Wazuh Server.
- Local events generated for monitoring validation.

- Instalado e registrado no Wazuh Server.
- Geração de eventos locais para validação da monitoração.

---

## 📌 Notes / Observações

- Created for educational purposes.
- Some configurations were simplified.
- Ideal for SIEM beginners and practical training.

- Criado com foco educacional.
- Algumas configurações foram simplificadas.
- Ideal para iniciantes em SIEM e prática com Wazuh.

---

## 🧰 Technologies Used / Tecnologias Utilizadas

- [Wazuh](https://wazuh.com/)
- [pfSense](https://www.pfsense.org/)
- [Ubuntu Server](https://ubuntu.com/)
- [Windows 11](https://www.microsoft.com/)
- [VMware Workstation](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion)

---

## 📚 Reference Course / Curso de Referência

**Wazuh Expert - Green Club**  
[https://wazuh-expert.greenn.club](https://wazuh-expert.greenn.club/)

---