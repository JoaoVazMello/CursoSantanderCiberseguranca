# 📅 Cronograma Semanal de Estudos (Semanas 1 a 4)

> 🤖 **Materializado e estruturado por Antigravity** (Assistente de Inteligência Artificial — Google DeepMind)  
> *Base de referência: `Plano de Estudos 30 Dias - Ciberseguranca.pdf` e `Pratica01.txt`.*

---

## 🧭 Metodologia de Execução Diária
Cada dia é planejado para uma sessão de **3 horas (180 minutos)**:
- 📖 **1h (60 min):** Teoria e conceitos estruturais
- 💻 **1h30 (90 min):** Prática ativa em terminal e laboratórios CTF
- 📝 **30 min:** Documentação, anotações e revisão técnica

---

## 📌 Semana 1 — Fundamentos de Redes, Linux e Conceitos Base (Dias 1 a 7)

**Meta da semana:** Compreender a comunicação em baixo nível entre máquinas e dominar a linha de comando Unix.

- [ ] **Dia 1: Protocolos de Rede Fundamentais**
  - **Teoria:** Pilha TCP/IP vs modelo OSI, UDP, resolução de nomes DNS, requisições HTTP vs conexões HTTPS.
  - **Prática:** Usar ferramentas de linha de comando (`nslookup`, `dig`, `traceroute`) e capturar consultas DNS e handshakes no **Wireshark**.
  - **Entrega do dia:** Resumo da anatomia de uma consulta DNS e captura de pacotes salva.

- [ ] **Dia 2: Terminal Linux Essencial**
  - **Teoria:** Hierarquia de diretórios FHS (`/etc`, `/var`, `/bin`), processos, usuários e permissões (`chmod`, `chown`).
  - **Prática:** Navegação rápida, filtros com `grep`, `awk`, `sed`, manipulação de pipes `|` e redirecionamentos `>` / `>>`.
  - **Entrega do dia:** Cheat sheet pessoal de comandos Linux para auditoria rápida.

- [ ] **Dia 3: Prática Progressiva de Terminal (OverTheWire)**
  - **Teoria:** Como ler arquivos ocultos, strings compactadas, permissões restritas e variáveis de ambiente.
  - **Prática:** Resolver os níveis **Bandit 0 ao 10** na plataforma [OverTheWire](https://overthewire.org/wargames/bandit/).
  - **Entrega do dia:** Caderno de soluções (write-up) dos níveis 0 a 10 do Bandit.

- [ ] **Dia 4: Portas, Serviços, Roteamento e Firewalls**
  - **Teoria:** Portas conhecidas (21, 22, 25, 53, 80, 443, 445, 3389), serviços em escuta, conceitos de NAT, tabelas de roteamento e regras de firewall (iptables/UFW).
  - **Prática:** Listar conexões ativas localmente (`ss -tulpn` ou `netstat -ano`), verificar sockets abertos e regras de firewall.
  - **Entrega do dia:** Mapeamento visual das portas ativas em sua máquina local.

- [ ] **Dia 5: Tríade CIA, Risco, Ameaça e Vulnerabilidade**
  - **Teoria:** Confidencialidade, Integridade e Disponibilidade (CIA); cálculo básico de risco ($Risco = Ameaça \times Vulnerabilidade \times Impacto$); modelos de autenticação (MFA) e autorização (RBAC).
  - **Prática:** Analisar um estudo de caso de vazamento recente e categorizar a falha segundo a Tríade CIA.
  - **Entrega do dia:** Relatório de 1 página desconstruindo o incidente estudado.

- [ ] **Dia 6: Ambiente Guiado de Segurança (TryHackMe)**
  - **Teoria:** Introdução a ambientes controlados e vetores comuns de ataque.
  - **Prática:** Concluir as salas introdutórias da trilha *Pre Security* ou *Cyber Security 101* no **TryHackMe**.
  - **Entrega do dia:** Conclusão de 2 a 3 salas práticas no TryHackMe com anotações.

- [ ] **Dia 7: Consolidação Semanal & Resumo Técnico**
  - **Revisão:** Cruzar as anotações dos dias 1 a 6.
  - **Prática / Registro:** Redigir um artigo ou nota técnica interna explicando como redes e sistemas operacionais interagem para sustentar aplicações corporativas.
  - **Entrega do dia:** Documento de consolidação da Semana 1 concluído.

---

## 📌 Semana 2 — Sistemas Operacionais, Criptografia e Automação (Dias 8 a 14)

**Meta da semana:** Compreender a mecânica interna do Windows, fundamentos de criptografia aplicada e desenvolver scripts utilitários em Python e Bash.

- [ ] **Dias 8 e 9: Estrutura Windows e Gestão de Permissões**
  - **Teoria:** Processos do Windows (LSASS, svchost, explorer), registro do sistema (HKLM, HKCU), logs de eventos (*Event Viewer*) e modelos de controle de acesso (SID, DACL, SACL, UAC).
  - **Prática:** Explorar o registro via `regedit` / PowerShell, auditar serviços ativos (`Get-Service`) e monitorar processos suspeitos via Sysinternals Process Explorer.
  - **Entrega:** Guia de inspeção rápida de artefatos do Windows.

- [ ] **Dias 10 e 11: Criptografia Aplicada e TLS**
  - **Teoria:** Algoritmos de Hash (MD5, SHA-256) e colisões; criptografia simétrica (AES) vs assimétrica (RSA, ECC); assinaturas digitais, certificados X.509 e fluxo do handshake TLS 1.3.
  - **Prática:** Gerar pares de chaves e certificados autoassinados via `openssl`, cifrar/decifrar arquivos e validar hashes via terminal.
  - **Entrega:** Script ou rotina para verificação de integridade de arquivos por hash.

- [ ] **Dias 12 e 13: Scripts e Automação para Segurança (Bash e Python)**
  - **Teoria:** Como automatizar tarefas repetitivas de análise de logs e checagem de portas/hosts ativos.
  - **Prática:** 
    - *Bash:* Criar um script que filtre acessos `404` ou requisições suspeitas em um arquivo de log do Apache/Nginx.
    - *Python:* Desenvolver um scanner simples de portas (usando a biblioteca nativa `socket`) ou um verificador de status HTTP (`urllib` / `requests`).
  - **Entrega:** 2 scripts utilitários salvos e documentados em repositório.

- [ ] **Dia 14: Revisão Prática e Desafios de Criptografia**
  - **Prática:** Avançar nos níveis intermediários do **OverTheWire Bandit (11 ao 16)** ou resolver 3 desafios da categoria *Cryptography* no **picoCTF**.
  - **Entrega do dia:** Write-up dos desafios concluídos.

---

## 📌 Semana 3 — Segurança de Aplicações Web e OWASP Top 10 (Dias 15 a 21)

**Meta da semana:** Dominar o funcionamento das requisições web e entender como explorar e corrigir as principais falhas do OWASP Top 10.

- [ ] **Dias 15 e 16: Arquitetura Web, Sessões, Cookies e APIs**
  - **Teoria:** Anatomia de requisições e respostas HTTP (métodos GET, POST, PUT, DELETE, headers `Authorization`, `Cookie`, `Set-Cookie`), armazenamento de estado (Sessions vs JWT), REST APIs e CORS.
  - **Prática:** Configurar o **Burp Suite Community** como proxy no navegador; interceptar, inspecionar e alterar requisições no *Burp Repeater*.
  - **Entrega:** Análise detalhada dos cabeçalhos de autenticação de uma aplicação de teste.

- [ ] **Dias 17 e 18: Injeção de SQL (SQL Injection - SQLi)**
  - **Teoria:** Mecanismo de falha em concatenação de queries, tipos de SQLi (In-band/Union-based, Blind, Error-based) e formas de mitigação (*Prepared Statements* / Queries Parametrizadas).
  - **Prática:** Resolver os laboratórios gratuitos de SQL Injection no **PortSwigger Web Security Academy**.
  - **Entrega:** Exploração guiada bem-sucedida e código de correção defensiva.

- [ ] **Dias 19 e 20: Cross-Site Scripting (XSS) e Quebras de Autenticação**
  - **Teoria:** Diferença entre XSS Refletido, Armazenado (Stored) e baseado em DOM; impactos (roubo de cookies/sessões, defacement); falhas de autenticação (força bruta, senhas fracas, bypass de controle de acesso).
  - **Prática:** Resolver os laboratórios de XSS no PortSwigger e testar interceptação de requisições de login.
  - **Entrega:** Write-up demonstrando como sanitizar inputs para evitar execução indevida de JavaScript.

- [ ] **Dia 21: Mapeamento OWASP Top 10:2025 & Consolidação Web**
  - **Revisão:** Estudar os 10 riscos mais críticos do OWASP Top 10:2025 (Broken Access Control, Cryptographic Failures, Injection, etc.).
  - **Entrega do dia:** Matriz de mitigação: para cada vulnerabilidade estudada na semana, documentar como o desenvolvedor deve corrigi-la no código-fonte.

---

## 📌 Semana 4 — Exploração Ofensiva, Defesa e Decisão de Carreira (Dias 22 a 30)

**Meta da semana:** Vivenciar a rotina de Red Team (varredura e enumeração) e Blue Team (análise de logs e tráfego), consolidando o aprendizado em um CTF final.

- [ ] **Dias 22 a 24: Enumeração e Varredura (Mentalidade Red Team)**
  - **Teoria:** Ciclo de testes de invasão (Reconhecimento, Varredura, Enumeração, Exploração, Pós-exploração). Tipos de scans do Nmap (`-sS`, `-sV`, `-sC`, `-O`).
  - **Prática:** Executar varreduras controladas em laboratórios do **Hack The Box Academy** ou máquinas locais isoladas; identificar banners e versões desatualizadas de serviços.
  - **Entrega:** Relatório de reconhecimento simulado listando serviços e vulnerabilidades potenciais.

- [ ] **Dias 25 a 27: Investigação de Incidentes e Logs (Mentalidade Blue Team)**
  - **Teoria:** Como identificar anomalias em tráfego de rede (Wireshark) e em logs de autenticação; introdução aos conceitos de SIEM, SOC e regras de detecção.
  - **Prática:** Resolver desafios de análise defensiva na plataforma **CyberDefenders** ou dissecar capturas `.pcap` com tráfego malicioso no Wireshark.
  - **Entrega:** Linha do tempo de um incidente investigado com base nos logs e pacotes.

- [ ] **Dias 28 e 29: Laboratório Integrado e CTF Aberto**
  - **Prática:** Participar de uma maratona prática no **picoCTF** ou em salas integradas do **TryHackMe**, aplicando conhecimentos de Linux, Redes, Criptografia e Web.
  - **Entrega:** Write-up completo de 2 a 3 máquinas/desafios resolvidos de ponta a ponta.

- [ ] **Dia 30: Balanço Final, Retrospectiva e Escolha de Carreira**
  - **Atividade:** Revisar todos os registros, entregáveis e notas produzidos ao longo dos 30 dias.
  - **Decisão:** Avaliar com qual das três trilhas seu perfil de Ciência da Computação teve maior afinidade:
    - *Opção A:* **AppSec** (Segurança de Código, SAST/DAST, proteção de pipelines CI/CD).
    - *Opção B:* **Red Team / Pentest** (Descoberta de falhas, engenharia reversa e intrusão).
    - *Opção C:* **Blue Team / SOC** (Detecção de ameaças, resposta a incidentes e forense digital).
  - **Entrega Final:** Plano de ação traçado para os 60 dias seguintes na área escolhida.
