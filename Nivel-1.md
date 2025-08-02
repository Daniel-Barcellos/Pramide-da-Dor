# 🔽Hash Values

Um **valor de hash** é uma sequência de caracteres gerada a partir de **um algoritmo matemático** que processa os dados de entrada
(por exemplo, um arquivo). Esse valor serve como uma impressão digital única daquele arquivo.

>> 🧠Exemplo
- Arquivo: Malware.exe
- Algoritmo Usado: SHA-256
- Hash Gerado: aef1239e1c3b09c5f6a0b2d3e4f9a1b8c0d1e2f3...
Se **qualquer byte de arquivo mudar**, o hash muda por completo.
---

## 🧩Para que Serve em Cibersegurança?

| Locais | Porque                              |
|-------|------------------------------------------|
| **Análise Forense**   | Quando um analista encontra um malware ou um arquivo suspeito, ele pode calcular o hash e comparar com bancos de dados públicos como VirusTotal, MISP ou outras plataformas de Threat Intelligence. |
| **Integridade**  | Pode ser usado para verificar se um arquivo foi alterado (ex: verificar se um log do sistema foi adulterado). |

---

## 😈Por que é fraco contra variantes de malware?

Os hashes são extremamente **sensíveis** a mudanças. Isso significa que se um malware for **levemente modificado**, o hash muda completamente. Isso é um problema.

**👇 Exemplos de como um atacante pode modificar um malware e gerar um novo hash:**
- **Recompilar o código**
- **Ofuscar o código-fonte.**
- **Inserir bytes irrelevantes.**
- **Alterar o nome das váriaveis ou strings.**
Mesmo que o comportamento malicioso permaneça **exatamente o mesmo**, o hash será **diferente**, enganando sistemas que confiam apenas no hash para identificar ameaças.


