# Integração OpenBot ↔ Empresa Empreender

Este diretório contém a integração completa da nossa empresa com a plataforma **OpenBot**, permitindo que a Torre de Controle (`Pai de todos`) orquestre tanto as demandas técnicas de desenvolvimento de software quanto as operações de negócio da empresa.

---

## 🤖 Os 6 Robôs Especialistas da Empresa

| Tag de Roteamento | Nome do Agente no OpenBot | Papel / Especialidade | Base de Conhecimento | Modelo Sugerido |
| :---: | :--- | :--- | :--- | :---: |
| `[COMERCIAL]` | `Operativo-Comercial` | SDR, Prospecção B2B Outbound, quebra de objeções e Propostas Comerciais Executivas (R$ 3.800 a R$ 8.500) | `operacoes/02_comercial_marketing/` | SWE-2 High / gemini-3.8-flash |
| `[JURIDICO]` | `Operativo-Juridico` | Minutas contratuais de sustentação com Damage Cap, NDAs com conformidade LGPD e Acordo de Sócios | `operacoes/01_juridico/` | SWE-2 High / gemini-3.8-flash |
| `[SLA]` | `Operativo-SLA` | Triagem de incidentes (P1 a P4), cronometragem de SLA, bloqueio de horas excedentes e aditivos | `operacoes/05_administracao/MATRIZ_SEVERIDADE_E_SLA.md` | SWE-2 High / gemini-3.8-flash |
| `[FINANCEIRO]` | `Operativo-FinOps` | CFO Operacional, monitoramento contínuo do Fator R (>=28% para 6% no Simples), cascata de fluxo e provisões | `operacoes/05_administracao/PLANEJAMENTO_TRIBUTARIO_E_FINANCEIRO.md` | SWE-2 High / gemini-3.8-flash |
| `[MARKETING]` | `Operativo-Marketing` | Conteúdo de autoridade técnica B2B no LinkedIn (framework Dev-to-Founder) para atração de CTOs e decisores | `operacoes/03_social_media/PLAYBOOK_LINKEDIN_AUTORIDADE.md` | SWE-2 High / gemini-3.8-flash |
| `[RH]` | `Operativo-TechScreen` | Triagem e correção do desafio técnico real (Java/Spring, Angular, SQL) com rubrica de 0 a 100 e AI slop check | `operacoes/04_rh/AVALIACAO_TECNICA_DEV.md` | SWE-2 High / gemini-3.8-flash |

---

## ⚡ Como Adicionar os Robôs no OpenBot (Passo a Passo)

Para cada um dos 6 robôs no OpenBot (menu lateral → **Novo Agente**):

1. **Nome:** O nome da tabela acima (ex: `Operativo-Comercial`).
2. **Modelo:** `SWE-2 High (Free)` (ou o modelo ativo de fallback).
3. **Descrição:** Abra o arquivo `.md` correspondente na pasta `agentes/` e copie todo o bloco de código para o campo de descrição.
4. **Workspace:** Defina a pasta raiz do repositório da empresa (`E:\empresa empreender`).
5. **Context Pack:** Certifique-se de que o arquivo `C:\Users\Thiago Duarte\OpenBot\Shared\context-packs\empresa-empreender.md` está ativo (já configurado).

---

## 🔄 Fluxo de Orquestração com o OpenBot

```
             Mensagem do Usuário / Sócio
                         │
                         ▼
             [Pai de todos / Torre]
                         │
        ┌────────────────┼────────────────┐
        │ [COMERCIAL]    │ [JURIDICO]     │ [SLA] / [FINANCEIRO] / [MARKETING] / [RH]
        ▼                ▼                ▼
Operativo-Comercial  Operativo-Juridico  Operativo Especialista
        │                │                │
        └────────────────┼────────────────┘
                         ▼
                 [Especialista-QA]
       (Auditoria de evidências / números)
                         │
                         ▼
                    [O Cético]
       (Validação de premissas e riscos)
                         │
                         ▼
                  [Canal Entregas]
     (Artefato pronto para aprovação dos Sócios - N1)
```

---

## 🛡️ Matriz de Autonomia Integrada (N0 a N4)

- **N0 (VEDADO):** Movimentações financeiras, envio não supervisionado de propostas/contratos, prometer prazos inexequíveis ou baixar preços abaixo do piso contratual.
- **N1 (SÓ O DONO EXECUTA):** Envio final de minutas contratuais para assinatura digital (ZapSign/ClickSign), envio de propostas a clientes, publicação no LinkedIn e aprovação de candidatos.
- **N2 (APROVA EM LOTE):** Cadências de mensagens de vendas, pautas semanais de marketing e relatórios mensais de consumo de horas de suporte.
- **N3/N4 (AUTÔNOMO):** Redação de propostas, cruzamento de dados, conferência de cálculos do Fator R, classificação de chamados por SLA e avaliação de código do desafio técnico.
