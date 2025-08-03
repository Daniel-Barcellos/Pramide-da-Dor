# 🌐 O que são Domain Names?
São **nomes registrados que apontam para servidores na internet**. Atacantes usam domínios para:
- **Hospedar sites falsos (phishing)**
- **Servir malware**
- **Controlar servidores C2**
Enganar usuários com **typosquatting** (ex: micorsoft-update.com em vez de microsoft.com).
---

>🧠 Exemplo prático
>>**Domínio malicioso:** micorsoft-update.com
>>**Objetivo:** Enganar vítimas que acham que estão acessando o site oficial da Microsoft.

| **Características**                  | **Explicação**                                                                 |
|-------------------------------------|--------------------------------------------------------------------------------|
| ✅ Útil para                        | Detectar padrões suspeitos (ex: typosquatting, domínios estranhos, etc).       |
| ❌ Não confiável para               | Detecção duradoura — domínios podem ser facilmente trocados ou descartados.    |
| ⚠️ Dificuldade para o atacante mudar | Moderada — exige novo registro, possível custo e tempo de configuração.        |
---

## 🔍 Por que domínios são úteis na detecção?

**Permitem análise comportamental:** você pode ver se há padrões repetitivos em domínios usados.
**Permitem detecção com regras:** como uso de algoritmos DGA (Domain Generation Algorithm), nomes muito longos, ou parecidos com marcas (typosquatting).

---

## 😈 Limitações dos domínios como IoCs
- Domínios podem ser descartáveis (registrados e usados por poucas horas).
- Existem serviços de domínios temporários e dynamic DNS, que permitem mudança rápida.
- O atacante pode registrar milhares de domínios com pequenas variações (ex: micros0ft.com, micorsoft.co, m1crosoft.org, etc.).
