### **PT**

# Thanos

Este repositório apresenta um estudo prático e análise dinâmica do **Thanos**, um ransonware que por volta de 2020 foi negociado via forúns na deepweb e darkweb como RaaS. O laboratório inclui **análise de amostra submetida** e **teste de infecção em ambiente Windows**.

## O que é o Thanos?

**Thanos** O Thanos surgiu no final de 2019, anunciado e vendido em mercados clandestinos conhecidos e canais fechados. O Thanos opera como um RaaS (Ransomware como Serviço) que fornece aos compradores e afiliados uma ferramenta personalizada chamada Thanos Builder para criar payloads exclusivos. O ransomware Thanos é conhecido por incorporar a técnica RIPlace..

## Atividades Realizadas

- Análise da amostra submetida ao [VirusTotal](https://www.virustotal.com/gui/file/ae66e009e16f0fad3b70ad20801f48f2edb904fa5341a89e126a26fd3fc80f75) (hash: `ae66e009e16f0fad3b70ad20801f48f2edb904fa5341a89e126a26fd3fc80f75`), verificando a detecção por diferentes mecanismos antivírus.
- **Infecção controlada de ambientes Windows** em sandbox.
- Execução e monitoramento do comportamento do malware.

## Aviso Legal

⚠️ **ATENÇÃO:** Este repositório contém **metadados e referências** a amostras reais de malware. Nenhum arquivo deve ser executado ou a infecção reproduzida **fora de ambientes de laboratório isolados e seguros**.

Este projeto é destinado **exclusivamente a fins acadêmicos e de pesquisa**. Qualquer uso indevido é estritamente proibido. Os autores e mantenedores **não se responsabilizam por consequências decorrentes de uso impróprio**.

## Evidências do Laboratório - Análise Dinâmica

### Ambiente Utilizado

- Sistema operacional: **Windows 10 x64 Virtualizado via VMWare**
- Execução controlada em ambiente isolado (sandbox)
- Windows defender desabilitado no sistema.
---

### Obtenção da Amostra

Clone o repositório com o comando:
```bash
git clone https://github.com/UFPE-Seguranca-Ofensiva/caatinga-malware-db.git
```

Navegue até a pasta `thanos` e extraia o arquivo `thanos.zip`.

<img src="img/1.png" alt="Thanos compactado" width="1000" height="400">


Após a extração, será exibido 4 arquivos com extensão `.exe`.

<img src="img/2.png" alt="Thanos descompactado" width="1000" height="400">

⚠️ **Atenção:** a execução dos arquivos `.exe` ativa o malware. Certifique-se de que esteja em ambiente isolado, com rede e compartilhamentos desativados.

---

### Execução e Infecção

Realize um duplo clique sobre o executável e aceite a execução.

<img src="img/3.png" alt="Thanos Aceite do sistema" width="1000" height="400">

Nesse momento a tela de resgate aparecerá e você poderá notar um número de PID's sendo executados de forma simultânea.

<img src="img/4.png" alt="Thanos tela de resgate" width="1000" height="400">


<img src="img/5.png" alt="PID's e CPU" width="1000" height="400">

Você poderá também observar no editor de registros os regs adicionados pelo Malware para habilitar o by-pass do windows defender e também desabilita a execução do Anti Spyware.

<img src="img/6.png" alt="Bypass Real time" width="1000" height="400">

<img src="img/7.png" alt="spyware" width="800" height="300">

---

### **EN**

# Thanos

This repository presents a practical study and dynamic analysis of **Thanos**, a ransomware that around 2020 was sold on deep web and dark web forums as RaaS. The lab includes **submitted sample analysis** and **infection testing in a Windows environment**.

## What is Thanos?

**Thanos** appeared at the end of 2019, announced and sold in known clandestine markets and closed channels. Thanos operates as a RaaS (Ransomware as a Service), providing buyers and affiliates with a custom tool called Thanos Builder to create unique payloads. The Thanos ransomware is known for incorporating the RIPlace technique.

## Activities Performed

- Analysis of the sample submitted to [VirusTotal](https://www.virustotal.com/gui/file/ae66e009e16f0fad3b70ad20801f48f2edb904fa5341a89e126a26fd3fc80f75) (hash: `ae66e009e16f0fad3b70ad20801f48f2edb904fa5341a89e126a26fd3fc80f75`), checking detection by various antivirus engines.
- **Controlled infection of Windows environments** in a sandbox.
- Execution and monitoring of malware behavior.

## Legal Notice

⚠️ **WARNING:** This repository contains **metadata and references** to real malware samples. No file should be executed or the infection reproduced **outside isolated and secure lab environments**.

This project is intended **exclusively for academic and research purposes**. Any misuse is strictly prohibited. The authors and maintainers **are not responsible for consequences resulting from improper use**.

## Laboratory Evidence – Dynamic Analysis

### Environment Used

- Operating system: **Windows 10 x64 Virtualized via VMWare**
- Controlled execution in an isolated environment (sandbox)
- Windows Defender disabled

---

### Obtaining the Sample

Clone the repository with the command:

```bash
git clone https://github.com/UFPE-Seguranca-Ofensiva/caatinga-malware-db.git
```
Navigate to the thanos folder and extract the thanos.zip file.

<img src="img/1.png" alt="Thanos compressed" width="1000" height="400">

After extraction, four .exe files will appear.

<img src="img/2.png" alt="Thanos decompressed" width="1000" height="400">

⚠️ Warning: Executing the .exe files activates the malware. Make sure you are in an isolated environment, with network and shares disabled.

### Execution and Infection

Double-click the executable and accept execution.

<img src="img/3.png" alt="Thanos system acceptance" width="1000" height="400">

At this point, the ransom screen will appear, and you may notice several PIDs running simultaneously.

<img src="img/4.png" alt="Thanos ransom screen" width="1000" height="400"> <img src="img/5.png" alt="PIDs and CPU" width="1000" height="400">

You can also observe in the registry editor the keys added by the malware to enable Windows Defender bypass and disable Anti-Spyware execution.

<img src="img/6.png" alt="Real-time bypass" width="1000" height="400"> 

<img src="img/7.png" alt="Spyware" width="800" height="300"> ```