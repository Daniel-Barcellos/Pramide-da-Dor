# 🧱 Pirâmide da Dor

> 📌 **O que é?**

A **Pirâmide da Dor** é um conceito da **cibersegurança** desenvolvido por *David Bianco* que descreve o **nível de dificuldade** que um adversário enfrenta ao ter seus métodos detectados e neutralizados.  
Ela mostra como **certos indicadores de comprometimento (IoCs)** são mais fáceis ou mais difíceis de mudar.

🔺 **Quanto mais alto na pirâmide**, mais **dor** para o atacante e **mais efetiva é sua detecção**.

---

## 🧠 Estrutura da Pirâmide

A pirâmide é dividida em **6 níveis**, do mais fácil de mudar (base) ao mais difícil (topo):

---

### 🔽 **Nível 1: Hashes**  
🧩 *Identificadores únicos de arquivos maliciosos (ex: MD5, SHA1).*  
🔧 Fácil para o atacante mudar com reempacotamento ou recompilação.

---

### 🌐 **Nível 2: Endereços IP**  
📍 *Endereços usados pelos atacantes para se comunicar com suas vítimas.*  
🔁 Podem ser trocados rapidamente com uso de VPNs, proxies ou botnets.

---

### 🌍 **Nível 3: Domínios**  
🔗 *Domínios registrados para comando e controle (C2).*  
📜 Um pouco mais custoso de mudar, pois envolve registro e propagação DNS.

---

### 🕸️ **Nível 4: Artefatos de Rede**  
📡 *Padrões específicos no tráfego (ex: payloads, URLs, user-agents).*  
🔍 Exigem mais conhecimento para modificar e manter a funcionalidade.

---

### 🛠️ **Nível 5: Ferramentas**  
🧰 *Softwares usados pelo atacante (ex: Mimikatz, Cobalt Strike).*  
🔐 Substituí-las ou personalizá-las consome mais tempo e conhecimento.

---

### 🔺 **Nível 6: TTPs – Táticas, Técnicas e Procedimentos**  
🧠 *Modo de operação do atacante, sua “assinatura” de comportamento.*  
💥 Mais difícil de mudar. Se detectado, prejudica seriamente sua operação.

---

## 📌 Resumo

| Sigla | Significado                              |
|-------|------------------------------------------|
| IoC   | 🕵️‍♂️ Indicador de Comprometimento         |
| TTPs  | ⚔️ Táticas, Técnicas e Procedimentos       |

