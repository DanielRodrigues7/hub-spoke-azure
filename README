
# Azure Hub‑Spoke – Laboratório Completo

Este repositório demonstra a implementação prática da arquitetura **Hub‑Spoke no Microsoft Azure**, validando:

- Comunicação centralizada via Hub
- Isolamento entre VNets Spoke
- Propagação de rotas via peering regional e global
- Testes reais de conectividade entre máquinas
- Rotas efetivas em cada interface

Toda a documentação é baseada em um laboratório real, acompanhado por prints armazenados em **rede hub/**.

---

## 🏗 Arquitetura do Laboratório

O ambiente contém:
- 1 VNet Hub (`vnet-hub`)
- 1 VNet Spoke HML (`vnet-hml`)
- 1 VNet Spoke DEV (`vnet-dev`)
- Máquinas virtuais distribuídas entre os spokes
- Peering Hub ↔ Spoke HML (global)
- Peering Hub ↔ Spoke DEV (regional)

### 📸 Diagrama da Arquitetura
rede hub/teste.drawio.png

---

## ⚙️ Endereçamento das VNets e Subnets

| Componente | VNet | Subnet | Região |
|-----------|------|--------|--------|
| **Hub**        | 10.1.0.0/16 | 10.1.1.0/24 | Brazil South |
| **Spoke HML**  | 10.0.0.0/16 | 10.0.1.0/24 e 10.0.2.0/24 | East US |
| **Spoke DEV**  | 10.2.0.0/16 | 10.2.1.0/24 | Brazil South |

---

## 🖥️ Máquinas Virtuais do Ambiente
rede hub/vms.png

---

## 🔗 Emparelhamentos (Peering)

rede hub/Emparelhamento.png

- **Hub ↔ HML** — Peering Global
- **Hub ↔ DEV** — Peering Regional
- ❌ Não existe peering entre spokes (isolamento intencional)

---

## 🛣️ Rotas Efetivas
rede hub/rotas.png

---

# 🔍 Testes de Comunicação

## 🟥 1. Spoke HML **não** consegue falar com o Spoke DEV
rede hub/dev fala apenas com hub.png

**Resultado esperado:** spokes ficam isolados.

---

## 🟦 2. Spoke HML → Hub (OK)
rede hub/comunicacao .png

---

## 🟩 3. Spoke DEV → Hub (OK)
rede hub/comunicacao .png

---

# 🛡️ Benefícios da Arquitetura Hub‑Spoke

- Isolamento entre workloads
- Comunicação centralizada
- Roteamento simplificado
- Arquitetura recomendada pela Microsoft

---

# 📁 Estrutura do Repositório
```
README.md
rede hub/
   Emparelhamento.png
   comunicacao .png
   dev fala apenas com hub.png
   rotas.png
   teste.drawio.png
   vms.png
```

---

# 📫 Contato
LinkedIn: https://www.linkedin.com/in/daniel-rodrigues-358b41121/
Email: daniel07.rodrigues@hotmail.com
