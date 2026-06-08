# C — Mapa de Atores

**Jornada:** Atendimento ao Seguro-Desemprego pela URA da Caixa
**Propósito:** Auxiliar a Caixa a tornar a URA efetiva para solução dos problemas do cidadão com eficiência e sem desperdício de tempo.
**Foco:** Cidadão com baixa experiência digital

---

## Diagrama de Atores (Onion)

```mermaid
flowchart TB
    subgraph Centro["Centro — Cidadão"]
        C["Cidadão<br/>(baixa experiência digital)"]
    end

    subgraph Op["Camada 1 — Operação Direta"]
        A1["URA da Caixa<br/>(automação)"]
        A2["Atendentes humanos BPO"]
        A3["Rede SINE"]
        A4["Central 158 (MTE)"]
        A5["Amigos/familiares<br/>tech-savvy"]
    end

    subgraph Gestao["Camada 2 — Gestão e Dados"]
        G1["Caixa Econômica Federal"]
        G2["MTE & CODEFAT"]
        G3["Dataprev"]
    end

    subgraph Regulacao["Camada 3 — Regulação e Controle"]
        R1["TCU"]
        R2["ANPD"]
        R3["SGD / MGI"]
    end

    subgraph Intermed["Camada 4 — Intermediários"]
        I1["Advogados trabalhistas"]
        I2["Sindicatos"]
    end

    C --> A1
    C --> A2
    C --> A3
    C --> A4
    C --> A5
    A1 --> A2
    A2 --> G1
    A1 --> G1
    A3 -.->|recurso admin.| G2
    A4 -.-> G2
    G1 --> G3
    G3 --> G1
    G2 --> G3
    R3 -.->|diretrizes EGD| G1
    R2 -.->|fiscalização LGPD| G1
    R1 -.->|auditoria| G1
    G1 -->|contrata| I2
    I1 -.->|judicialização| G2
```

---

## Tabela de Atores

### Matriz Poder × Interesse (Mendelow)

| # | Ator | Camada | Poder | Interesse | Classificação |
|---|------|--------|-------|-----------|---------------|
| 1 | Cidadão (baixa experiência digital) | Centro | Baixo | Alto | Manter informado |
| 2 | URA da Caixa (automação) | Operação | — | — | Canal focal |
| 3 | Atendentes humanos BPO | Operação | Baixo | Alto | Manter informado |
| 4 | Rede SINE | Operação | Baixo | Alto | Manter informado |
| 5 | Central 158 (MTE) | Operação | Baixo | Médio | Manter informado |
| 6 | Amigos/familiares tech-savvy | Operação | Baixo | Médio | Manter informado |
| 7 | Caixa Econômica Federal | Gestão | Alto | Médio | Gerenciar de perto |
| 8 | MTE & CODEFAT | Gestão | Alto | Alto | Gerenciar de perto |
| 9 | Dataprev | Gestão | Alto | Médio | Gerenciar de perto |
| 10 | SGD / MGI | Regulação | Alto | Baixo | Manter satisfeito |
| 11 | ANPD | Regulação | Médio | Baixo | Monitorar |
| 12 | TCU | Regulação | Médio | Baixo | Monitorar |
| 13 | Advogados trabalhistas | Intermediários | Baixo | Alto | Manter informado |
| 14 | Sindicatos | Intermediários | Médio | Médio | Monitorar |

---

## Incentivos e Resistências (Atores-Chave)

| Ator | Manutenção (o que ganha hoje) | Resistência (o que perderia) | Alavanca (o que ganharia) |
|------|------------------------------|-----------------------------|---------------------------|
| **Cidadão** | Sofre a fricção, desiste do benefício | Nenhuma | Serviço resolutivo sem desperdício de tempo |
| **Caixa** | Contrato de BPO gera receita corrente | Investimento em redesign técnico | Redução de reclamações no BC/TCU; imagem positiva |
| **MTE/CODEFAT** | URA inefetiva reduz desistências → menos dispêndio do FAT | Perda da "barreira fiscal" oculta | Crédito político por entrega digna; redução de judicialização |
| **Dataprev** | Consultas manuais justificam orçamento | Custo de migrar para interoperabilidade síncrona | Reputação como backbone tecnológico do governo |
| **Empresas de BPO** | Remuneração por volume de ligações → recontato é receita | Contratos menores se URA resolver na 1ª chamada | Estabilidade contratual com métricas de qualidade |
| **Atendentes BPO** | Sofrem com URA mal desenhada (re-digitação, sem contexto) | Nenhuma — são vítimas do design | Serem fonte de inteligência para melhoria da URA |
| **SGD/MGI** | Risco reputacional nos rankings | Nenhuma relevante | Serviço alinhado à EGD = vitrine de governo digital |

---

## Hipóteses de Fricção e Failure Demand

1. **Barreira fiscal (MTE/CODEFAT):** A fricção da URA opera como filtro não declarado — cidadãos que desistem reduzem o dispêndio do FAT sem necessidade de negativa explícita.
2. **Volume vs. resolução (Caixa + BPO):** Contratos pagos por chamada atendida, não por problema resolvido. O incentivo econômico é oposto à efetividade.
3. **Interoperabilidade em lote (Dataprev):** Consultas por batelada em vez de síncronas geram retrabalho e informação desatualizada na URA.

### Métricas Recomendadas

| Dimensão | Métrica | Alvo sugerido |
|----------|---------|---------------|
| Qualidade/Resolução | First Contact Resolution (FCR) | > 70% |
| Volume/Composição | Proporção Value Demand / Failure Demand | Value > 60% |
| Acesso/Inclusão | Drop-off rate por etapa da URA | < 10% por nó |
| Custo | Custo por problema resolvido (não por chamada) | Redução anual |
