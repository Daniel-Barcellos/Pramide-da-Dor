## 🌐 1. O que são IP Addresses (Endereços IP)?

Um endereço **IP (Internet Protocol)** é como um “endereço de casa” usado para identificar um dispositivo na internet ou em uma rede local.

**Na cibersegurança, os IPs maliciosos geralmente estão associados a:**
- Servidores C2 (Command and Control): usados por malware para receber comandos.
- Servidores de exfiltração de dados: onde informações roubadas são enviadas.
- Serviços de phishing, botnets, proxies, etc.

>🧠 Exemplo:
`192.168.100.50`
>>(obs: esse exemplo é IP privado, mas em ataques reais geralmente são IPs públicos)
---
## 🔐 2. Uso de IPs em defesa

Quando um analista identifica um IP malicioso:
- **✅ Pode ser bloqueado no firewall, IDS/IPS ou DNS.**
- **✅ Pode ser monitorado para detectar novos acessos.**
- **✅ Pode ser usado para correlacionar eventos em logs (quem se conectou a esse IP?).**
Essa resposta **imediata** é uma grande vantagem.
---

## 😈 3. Por que o IP é fraco como defesa isolada?
Um atacante pode **trocar de IP facilmente**. Ele pode:
- Usar **VPNs ou proxies** (serviços pagos ou gratuitos).
- Contratar **infraestrutura em nuvem** (ex: AWS, DigitalOcean, etc.).
- Utilizar **redes zumbis (botnets)** com IPs variados e rotativos.
- Registrar **domínios com IPs dinâmicos**, trocando o servidor por trás com frequência.
Essas técnicas tornam a **detecção baseada apenas em IP muito frágil** e fácil de evadir.
---
| **Características**                | **Explicação**                                                                 |
|-----------------------------------|--------------------------------------------------------------------------------|
| ✅ Útil para                       | Resposta rápida (bloqueio imediato), rastreamento de conexões maliciosas.     |
| ❌ Não confiável para              | Detecção duradoura — IPs podem mudar rapidamente.                              |
| 🛠️ Dificuldade para o atacante mudar | Fácil — troca por outro IP com VPN, proxy ou novo servidor.                   |
