# INSTRUMENTO PARTICULAR DE PRESTAÇÃO DE SERVIÇOS DE SUSTENTAÇÃO, MANUTENÇÃO DE SOFTWARE E ACORDO DE NÍVEL DE SERVIÇO (SLA)

Pelo presente instrumento particular, de um lado:

**CONTRATANTE:**
* **Razão Social / Nome:** [NOME DA EMPRESA CLIENTE]
* **CNPJ / CPF:** [00.000.000/0000-00]
* **Endereço:** [Endereço completo, Cidade - UF, CEP]
* **Representante Legal:** [Nome completo do representante], [Nacionalidade], [Estado Civil], portador do RG nº [0000000] e CPF nº [000.000.000-00], doravante denominada simplesmente **CONTRATANTE**;

E, de outro lado:

**CONTRATADA:**
* **Razão Social:** **[RAZÃO SOCIAL DA CONTRATADA - Em Processo de Constituição]**
* **Nome Fantasia:** [NOME FANTASIA DA EMPRESA]
* **CNPJ:** **[00.000.000/0001-00 - Em Constituição]**
* **Sede:** Brasília - DF
* **Representada por:** [Nome do Sócio Administrador], doravante denominada simplesmente **CONTRATADA**;

Ambas doravante denominadas conjuntamente como **PARTES** e individualmente como **PARTE**.

Têm entre si, justo e contratado, o presente Contrato, mediante as seguintes cláusulas e condições:

---

### CLÁUSULA PRIMEIRA – DO OBJETO
1.1. O presente Contrato tem por objeto a prestação contínua de serviços técnicos especializados de **Sustentação, Manutenção Preventiva, Corretiva e Evolutiva** dos sistemas, bancos de dados e aplicações de propriedade ou posse da **CONTRATANTE**, conforme detalhado no **Anexo I (Escopo e Plano Contratado)**.  
1.2. Os serviços compreendem:
* **Manutenção Preventiva:** Monitoramento de estabilidade, verificações de integridade de banco de dados, atualização de dependências e aplicação de patches de segurança.
* **Manutenção Corretiva:** Diagnóstico e correção de falhas de código (*bugs*), travamentos, lentidões e erros de execução em ambiente de produção.
* **Manutenção Evolutiva:** Pequenas melhorias, otimizações de consultas (queries), alterações de regras de negócio e novas rotinas delimitadas pelo banco de horas mensal contratado.

---

### CLÁUSULA SEGUNDA – DO BANCO DE HORAS E REGIME DE ATENDIMENTO
2.1. A **CONTRATADA** disponibilizará mensalmente à **CONTRATANTE** um banco de **[X horas, ex: 30 horas]** técnicas especializadas.  
2.2. **Não Cumulatividade:** As horas contratadas e não utilizadas dentro do mês de vigência **não serão acumuladas** para os meses subsequentes, remunerando a reserva técnica e disponibilidade contínua da equipe da **CONTRATADA**.  
2.3. **Horas Excedentes:** Caso a **CONTRATANTE** necessite de volume superior ao banco de horas pactuado, as horas adicionais serão faturadas pelo valor de **R$ [180,00] (cento e oitenta reais)** por hora técnica, mediante aprovação prévia e por escrito (inclusive por e-mail ou WhatsApp oficial) da **CONTRATANTE**.  
2.4. O atendimento regular será realizado em dias úteis, das **08:30 às 18:30 (horário de Brasília)**.

---

### CLÁUSULA TERCEIRA – DO ACORDO DE NÍVEL DE SERVIÇO (SLA)
3.1. A **CONTRATADA** compromete-se a cumprir os seguintes tempos máximos de **Primeira Resposta** e **Início de Atuação**, contados a partir da abertura formal do chamado:

| Severidade | Definição do Incidente | Tempo de Resposta | Início de Atuação |
| :--- | :--- | :---: | :---: |
| **P1 - Crítica** | Sistema totalmente fora do ar, indisponibilidade de faturamento ou perda iminente de dados. | **Até 2 horas** | Imediato |
| **P2 - Alta** | Falha grave que prejudica operações essenciais, sem alternativa de contorno imediata. | **Até 4 horas** | Até 6 horas |
| **P3 - Média** | Falha em funcionalidade parcial, lentidão pontual ou demanda com alternativa de contorno. | **Até 8 horas** | Até 24 horas |
| **P4 - Baixa / Evolutiva** | Dúvidas, pequenos ajustes cosméticos ou melhorias de rotina. | **Até 12 horas** | Agendada no backlog |

3.2. Os chamados de emergência de Severidade P1 fora do horário comercial (noites ou fins de semana) deverão ser acionados via canal de sobreaviso, com valor-hora especial de **R$ 250,00 (duzentos e cinquenta reais)**.  
3.3. **Penalidade Exclusiva por Descumprimento de SLA:** Eventual descumprimento injustificado dos prazos estipulados para chamados de Severidade P1 conferirá à CONTRATANTE exclusivamente o direito a um desconto financeiro de 5% (cinco por cento) sobre a mensalidade vincenda do mês subsequente por ocorrência, limitado ao teto máximo de 10% (dez por cento) do valor mensal. O descumprimento pontual de SLA não ensejará rescisão automática nem constituirá fundamento para pleito de perdas e danos ou indenizações materiais.

---

### CLÁUSULA QUARTA – DOS VALORES E CONDIÇÕES DE PAGAMENTO
4.1. Pela prestação dos serviços objeto deste contrato, a **CONTRATANTE** pagará à **CONTRATADA** o valor fixo mensal de **R$ [X.XXX,00] ([Valor por extenso])**.  
4.2. O pagamento será efetuado até o dia **[05 ou 10]** de cada mês subsequente ao vencido, mediante emissão prévia de Nota Fiscal de Serviços Eletrônica (NFS-e) e boleto bancário ou chave PIX emitida pela **CONTRATADA**.  
4.3. Em caso de inadimplemento, incidirá multa moratória de 2% (dois por cento) sobre o valor em atraso, acrescida de juros de mora de 1% (um por cento) ao mês e correção monetária pelo IPCA/IBGE.  
4.4. O atraso superior a 15 (quinze) dias facultará à **CONTRATADA** suspender a execução dos serviços de suporte até a regularização do débito.

---

### CLÁUSULA QUINTA – DA PROPRIEDADE INTELECTUAL
5.1. Todo o código-fonte, scripts de aplicação, documentações e customizações desenvolvidos especificamente para atender às regras de negócio da **CONTRATANTE** em decorrência deste contrato pertencerão exclusivamente à **CONTRATANTE** após a respectiva quitação financeira.  
5.2. A **CONTRATADA** resguarda a titularidade exclusiva sobre suas ferramentas pré-existentes, bibliotecas proprietárias, frameworks internos, métodos de engenharia, prompts de Inteligência Artificial e rotinas-base desenvolvidos de forma independente, outorgando à **CONTRATANTE** apenas uma licença de uso perpétua, irrevogável e não-exclusiva para a operação de seus sistemas.

---

### CLÁUSULA SEXTA – DA PROTEÇÃO DE DADOS (LGPD) E CONFIDENCIALIDADE
6.1. As **PARTES** comprometem-se a cumprir integralmente a Lei nº 13.709/2018 (Lei Geral de Proteção de Dados - LGPD).  
6.2. A **CONTRATADA** atuará na condição de **Operadora de Dados Pessoais**, tratando apenas as informações estritamente necessárias para a manutenção e suporte dos sistemas da **CONTRATANTE** (Controladora).  
6.3. Ambas as partes obrigam-se a manter absoluto sigilo sobre códigos-fontes, segredos de negócio, dados financeiros e credenciais de acesso, sob pena de indenização por perdas e danos.

---

### CLÁUSULA SÉTIMA – DA VIGÊNCIA E RESCISÃO
7.1. O presente contrato tem vigência de **[12 (doze) meses]**, iniciando em **[DATA DE INÍCIO]** e renovando-se automaticamente por períodos iguais caso nenhuma das partes se manifeste em contrário.  
7.2. Qualquer das partes poderá rescindir o presente contrato imotivadamente mediante aviso prévio por escrito com antecedência mínima de **30 (trinta) dias**, sem incidência de multa após decorridos os primeiros 90 (noventa) dias de contrato.  
7.3. O descumprimento reiterado e injustificado de obrigações essenciais ensejará a rescisão motivada, após notificação formal com prazo de 15 (quinze) dias para saneamento da falha.

---

### CLÁUSULA OITAVA – DA LIMITAÇÃO DE RESPONSABILIDADE CIVIL (DAMAGE CAP)
8.1. **Teto Máximo Indenizatório (Damage Cap):** A responsabilidade civil total e cumulativa da **CONTRATADA** perante a **CONTRATANTE** ou quaisquer terceiros por quaisquer danos diretos, perdas, custos, falhas operacionais ou prejuízos decorrentes deste Contrato, independentemente da teoria jurídica aplicada (contratual, extracontratual ou responsabilidade civil), estará **estrita e expressamente limitada à soma do valor correspondente a 3 (três) mensalidades vigentes** efetivamente pagas pela **CONTRATANTE** nos últimos 3 meses anteriores ao evento danoso.  
8.2. **Exclusão de Danos Indiretos e Lucros Cessantes:** Em nenhuma hipótese a **CONTRATADA** responderá perante a **CONTRATANTE** por: lucros cessantes, perda de receitas, perda de faturamento, paralisação de vendas, interrupção de negócios, danos indiretos, incidentais ou punitivos, nem por perda ou corrupção de dados decorrentes de falhas de serviços terceirizados, instabilidade em provedores de nuvem (AWS/GCP/Azure) ou ataques cibernéticos externos imprevisíveis.

---

### CLÁUSULA NONA – DO FORO
9.1. Para dirimir quaisquer litígios oriundos do presente instrumento, as partes elegem o **Foro da Circunscrição Judiciária de Brasília - DF**, com expressa renúncia a qualquer outro, por mais privilegiado que seja.

E, por estarem justas e contratadas, as partes firmam o presente instrumento por meio de assinatura eletrônica nos termos da Lei nº 14.063/2020.

Brasília - DF, [Dia] de [Mês] de [Ano].

_____________________________________________  
**CONTRATANTE:** [NOME DA EMPRESA CLIENTE]  
CNPJ: [00.000.000/0000-00]  

_____________________________________________  
**CONTRATADA:** [RAZÃO SOCIAL DA CONTRATADA]  
CNPJ: [00.000.000/0001-00]  
[Nome do Sócio Administrador] (Administrador)  
