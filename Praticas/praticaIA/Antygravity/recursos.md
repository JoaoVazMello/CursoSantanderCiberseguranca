# 📚 Recursos e Materiais de Estudo por Semana

> 🤖 **Materializado e estruturado por Antigravity** (Assistente de Inteligência Artificial — Google DeepMind)  
> *Baseado nas plataformas recomendadas e diretrizes compiladas em `Plano de Estudos 30 Dias - Ciberseguranca.pdf` e `Pratica01.txt`.*

---

## 🌐 Plataformas Gerais Recomendadas

| Plataforma | Estilo de Aprendizado | Foco Principal | Custo / Acesso |
| :--- | :--- | :--- | :--- |
| [TryHackMe](https://tryhackme.com/) | Salas guiadas com teoria e prática integrada | Redes, Linux e Introdução a Cyber | Gratuito com opções pagas |
| [OverTheWire (Bandit)](https://overthewire.org/wargames/bandit/) | Wargames progressivos via SSH | Linha de comando Linux e Shell | 100% Gratuito |
| [PortSwigger Academy](https://portswigger.net/web-security) | Teoria avançada e laboratórios reais | Segurança Web (OWASP Top 10) | 100% Gratuito |
| [Hack The Box Academy](https://academy.hackthebox.com/) | Módulos aprofundados com avaliação | Pentest, Red Team e Infraestrutura | Módulos gratuitos e pagos |
| [CyberDefenders](https://cyberdefenders.org/) | Desafios CTF defensivos | Blue Team, Análise de Logs e DFIR | Gratuito com tiers pagos |
| [picoCTF](https://picoctf.org/) | Desafios de CTF de níveis variados | Criptografia, Forense, Engenharia Reversa | 100% Gratuito |

---

## 🔹 Semana 1 — Fundamentos de Redes, Linux e Segurança Base

### 📖 Teoria e Conceitos
- **Redes de Computadores:** Pilha TCP/IP, diferença entre TCP e UDP, resolução hierárquica de DNS, ciclo Request/Response HTTP e criptografia no HTTPS (porta 443).
- **Sistemas Operacionais (Linux):** Árvore de diretórios (FHS), permissões numéricas e simbólicas (`chmod 755`, `chmod 600`), gerenciamento de processos (`ps aux`, `top`, `kill`) e pipes.
- **Fundamentos de Segurança:** Tríade CIA (Confidencialidade, Integridade e Disponibilidade), vetores de ataque, ameaça vs vulnerabilidade.

### 🛠️ Ferramentas
- **Wireshark:** Analisador de protocolos de rede. Baixe em [wireshark.org](https://www.wireshark.org/).
- **Utilitários de Linha de Comando:** `nslookup`, `dig`, `traceroute`, `ss`, `netstat`, `curl`.

### 🎮 Laboratórios Práticos
- [OverTheWire: Bandit (Levels 0 a 10)](https://overthewire.org/wargames/bandit/) — Treino intensivo de comandos de terminal Linux.
- [TryHackMe: Trilha Pre Security / Cyber Security 101](https://tryhackme.com/path/outline/presecurity) — Ambientes guiados para iniciantes.

---

## 🔹 Semana 2 — Sistemas Operacionais, Criptografia e Automação

### 📖 Teoria e Conceitos
- **Windows Internals:** Entendimento de processos-chave (`svchost.exe`, `lsass.exe`), arquitetura do Registro do Windows (`HKLM`, `HKCU`) e controle de acesso (SIDs, ACLs, UAC).
- **Criptografia Aplicada:** Diferenças entre funções de Hash (SHA-256) e Cifra; criptografia simétrica (AES-GCM) vs assimétrica (RSA); Infraestrutura de Chaves Públicas (PKI), autoridades certificadoras (CAs) e certificados digitais X.509.
- **Automação para Segurança:** Uso de Python e Shell Scripting para parsing de logs e automação de rotinas de auditoria.

### 🛠️ Ferramentas
- **OpenSSL:** Utilitário para criação de certificados, hashes e testes de handshake TLS.
- **Python 3:** Bibliotecas recomendadas: `socket`, `hashlib`, `requests`, `re`.
- **Sysinternals Suite (Microsoft):** Process Explorer e Autoruns para inspeção avançada no Windows.

### 🎮 Laboratórios Práticos
- [OverTheWire: Bandit (Levels 11 a 16)](https://overthewire.org/wargames/bandit/) — Manipulação de criptografia básica, certificados SSL e portas remotas.
- [picoCTF — Cryptography Category](https://play.picoctf.org/) — Resolução de desafios de cifras clássicas e criptografia moderna.

---

## 🔹 Semana 3 — Segurança de Aplicações Web & OWASP Top 10

### 📖 Teoria e Conceitos
- **Arquitetura Web:** Cabeçalhos de segurança (`Content-Security-Policy`, `Strict-Transport-Security`, `X-Content-Type-Options`), gerenciamento de sessão, Cookies (`HttpOnly`, `Secure`, `SameSite`).
- **OWASP Top 10:2025:**
  - *Broken Access Control (A01):* Falhas em controle de privilégios e IDOR.
  - *Cryptographic Failures (A02):* Dados sensíveis expostos em trânsito ou repouso.
  - *Injection (A03):* SQL Injection, Command Injection e LDAP Injection.
  - *Insecure Design (A04) e Security Misconfiguration (A05).*
- **Cross-Site Scripting (XSS):** Reflected, Stored e DOM-based.

### 🛠️ Ferramentas
- **Burp Suite Community Edition:** O proxy interceptador padrão da indústria para auditoria web. Baixe em [portswigger.net/burp/communitydownload](https://portswigger.net/burp/communitydownload).
- **DevTools do Navegador:** Abas *Network*, *Application* (Storage/Cookies) e *Console*.

### 🎮 Laboratórios Práticos
- [PortSwigger Web Security Academy — SQL Injection](https://portswigger.net/web-security/sql-injection) — Laboratórios práticos do nível iniciante ao intermediário.
- [PortSwigger Web Security Academy — Cross-site scripting (XSS)](https://portswigger.net/web-security/cross-site-scripting) — Desafios interativos de exploração e sanitização.
- [OWASP Top 10 Documentação Oficial](https://owasp.org/www-project-top-ten/) — Leitura dos padrões internacionais de vulnerabilidade.

---

## 🔹 Semana 4 — Exploração Ofensiva, Defesa e Decisão de Carreira

### 📖 Teoria e Conceitos
- **Metodologia de Pentest (Red Team):** Fases de reconhecimento, varredura de portas, enumeração de serviços/versões e identificação de exploits.
- **Defesa e SOC (Blue Team):** Análise de artefatos de intrusão, triagem de alertas, detecção de tráfego anômalo e forense básica.
- **Trilhas de Especialização:**
  - *AppSec:* Integração com pipelines CI/CD (DevSecOps), análise de código estático (SAST) e dinâmico (DAST).
  - *Pentesting:* Testes de intrusão externos/internos e relatórios de risco executivo.
  - *SOC/DFIR:* Operação de SIEMs, análise de tráfego de rede e resposta a incidentes.

### 🛠️ Ferramentas
- **Nmap:** O scanner de portas e auditor de serviços essencial (`nmap -sV -sC -Pn <target>`).
- **CyberDefenders Artifacts:** Ferramentas web de decodificação de logs e visualização de pacotes.

### 🎮 Laboratórios Práticos
- [Hack The Box Academy](https://academy.hackthebox.com/) — Módulos fundamentais de *Network Enumeration with Nmap*.
- [CyberDefenders Labs](https://cyberdefenders.org/blueteam-ctf-challenges/) — Prática com análise de tráfego e logs de ataques reais.
- [picoCTF — Forensic & Web Exploitation](https://play.picoctf.org/) — Consolidação prática em desafios de estilo CTF.

---

## 🔒 Diretrizes de Segurança Ética

1. **Autorização Expressa:** Nunca teste vulnerabilidades ou execute scanners automatizados contra sistemas sem permissão formal por escrito.
2. **Isolamento de Ambiente:** Utilize máquinas virtuais (VirtualBox, VMware) ou as VMs na nuvem fornecidas pelas próprias plataformas para executar ferramentas e testes.
3. **Mentalidade Construtiva:** Lembre-se que o objetivo de aprender a quebrar sistemas é compreender como torná-los resilientes e seguros.
