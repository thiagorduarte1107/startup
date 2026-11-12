# Central de Operações da Empresa (AGY Operations Hub)

Este diretório contém a esteira operacional completa, os contratos, os scripts de vendas e os playbooks de execução da nossa empresa de desenvolvimento, sustentação e IA.

---

## Estrutura Operacional

```
operacoes/
├── 01_juridico/
│   ├── CONTRATO_SUSTENTACAO_E_SLA.md (.docx)   # Minuta jurídica com Damage Cap e SLA blindado
│   ├── ACORDO_CONFIDENCIALIDADE_NDA.md (.docx) # Acordo de sigilo e proteção de código/dados
│   └── ACORDO_DE_SOCIOS.md (.docx)             # Acordo dos 4 sócios (Vesting, Voto de Minerva do Diego, Deadlock)
├── 02_comercial_marketing/
│   ├── PROPOSTA_COMERCIAL_EXECUTIVA.md (.docx) # Proposta oficial com pacotes de R$ 3,8k a R$ 8,5k
│   └── SCRIPTS_PROSPECCAO_OUTBOUND.md          # Scripts de WhatsApp, LinkedIn e abordagem de agências
├── 03_social_media/
│   └── PLAYBOOK_LINKEDIN_AUTORIDADE.md         # Estratégia editorial e templates de posts técnicos
├── 04_rh/
│   └── AVALIACAO_TECNICA_DEV.md                # Desafio prático para estagiários/suporte (Java/Angular/SQL)
├── 05_administracao/
│   ├── MATRIZ_SEVERIDADE_E_SLA.md              # Protocolo de atendimento P1/P2/P3 e gestão de chamados
│   └── PLANEJAMENTO_TRIBUTARIO_E_FINANCEIRO.md (.docx) # Manual CFO: Simples Nacional a 6%, Fator R e Reservas
└── openbot_integracao/                 # Integração e Robôs Especialistas para o OpenBot
    ├── README.md                       # Guia de implantação e fluxo de orquestração
    └── agentes/                        # Perfis prontos: Comercial, Jurídico, SLA, FinOps, Marketing, RH
```

---

## Como Operar Esta Estrutura no Antigravity (AGY)

1. **Para Fechar um Novo Cliente:**
   * Preencha a [PROPOSTA_COMERCIAL_EXECUTIVA.md](02_comercial_marketing/PROPOSTA_COMERCIAL_EXECUTIVA.md) e exporte para PDF.
   * Ao aceitar, gere o [CONTRATO_SUSTENTACAO_E_SLA.md](01_juridico/CONTRATO_SUSTENTACAO_E_SLA.md) assinado via ClickSign/ZapSign/Gov.br.
2. **Para Prospectar Novos Clientes no DF e Brasil:**
   * Utilize os templates em [SCRIPTS_PROSPECCAO_OUTBOUND.md](02_comercial_marketing/SCRIPTS_PROSPECCAO_OUTBOUND.md).
3. **Para Gerar Autoridade Orgânica:**
   * Aplique os modelos de [PLAYBOOK_LINKEDIN_AUTORIDADE.md](03_social_media/PLAYBOOK_LINKEDIN_AUTORIDADE.md).
4. **Para Atender e Controlar Chamados Técnicos:**
   * Siga o protocolo rigoroso de [MATRIZ_SEVERIDADE_E_SLA.md](05_administracao/MATRIZ_SEVERIDADE_E_SLA.md).
