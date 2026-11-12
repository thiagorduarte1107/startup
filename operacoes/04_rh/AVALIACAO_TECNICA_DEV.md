# GUIA DE AVALIAÇÃO TÉCNICA E RECRUTAMENTO DE DESENVOLVEDORES

Este documento padroniza a avaliação prática para futuras contratações de estagiários, desenvolvedores juniores ou apoios técnicos temporários para o suporte da nossa empresa.

---

## 1. Princípio da Avaliação
Não aplicamos testes teóricos de decorar algoritmos (estilo LeetCode). Avaliamos **habilidade de resolver problemas reais de sustentação**:
1. Capacidade de ler e entender código legado de outra pessoa;
2. Conhecimento sólido em SQL e integridade de dados;
3. Noções de arquitetura limpa em Java / Spring Boot e Angular;
4. Uso inteligente e responsável de ferramentas de IA (Copilot/ChatGPT) com senso crítico.

---

## 2. O Desafio Prático: "O Resgate do Sistema Legado"
O candidato recebe um mini-repositório com uma aplicação simples de controle de pedidos contendo propositalmente 3 falhas comuns de sistemas reais.

### Cenário do Desafio:
* **Backend:** Java 17+ com Spring Boot e Spring Data JPA.
* **Frontend:** Angular 16+ com TypeScript.
* **Banco de Dados:** PostgreSQL ou H2 em memória.

### Tarefas que o Candidato Deve Executar (Prazo: 48 horas):

#### Tarefa 1: Otimização de Consulta SQL (Gargalo de Performance)
* **O Problema:** O endpoint `/api/pedidos` realiza uma consulta que dispara o infame problema do *N+1 queries*, travando o banco de dados quando existem mais de 500 pedidos cadastrados.
* **Critério de Avaliação:** O candidato deve refatorar a consulta usando `JOIN FETCH`, `@EntityGraph` ou uma query nativa otimizada, explicando a diferença no log do Hibernate.

#### Tarefa 2: Correção de Concorrência e Transação
* **O Problema:** Dois usuários tentando aprovar o mesmo pedido simultaneamente causam duplicidade de estoque.
* **Critério de Avaliação:** Uso correto de anotações `@Transactional`, *Optimistic Locking* (`@Version`) ou bloqueio pessimista adequado para garantir consistência.

#### Tarefa 3: Pequena Melhoria no Frontend Angular
* **A Demanda:** Adicionar uma coluna de "Status do Pedido" com cores dinâmicas e um filtro reativo por período utilizando RxJS e Signals.
* **Critério de Avaliação:** Componentização limpa, sem vazamento de memória (gerenciamento adequado de subscriptions).

---

## 3. Matriz de Pontuação e Rubrica (Nota 1 a 5)

| Critério | Peso | O que buscamos |
| :--- | :---: | :--- |
| **Clareza do Código e Boas Práticas** | 25% | Nomes significativos, métodos curtos, tratamento adequado de exceções. |
| **Domínio de SQL e Modelagem** | 25% | Compreensão real de índices, chaves estrangeiras e eficiência de joins. |
| **Segurança e Validação** | 20% | Validação de entradas (evitar SQL Injection, validações de DTO). |
| **Comunicação e Raciocínio** | 20% | Clareza ao explicar a solução no README do teste ou na entrevista técnica. |
| **Uso Consciente de IA** | 10% | Permitimos o uso de IA, desde que o candidato saiba explicar cada linha de código entregue. |

---

## 4. Roteiro da Entrevista Técnica (30 minutos com os Sócios)
1. *"Explique como você identificou a causa raiz do problema de performance no desafio."*
2. *"Se o banco de dados desse cliente começasse a atingir 100% de CPU em produção às 10h da manhã, quais seriam os seus três primeiros passos de diagnóstico?"*
3. *"Como você utilizou ferramentas de IA para resolver o teste e quais partes você precisou corrigir manualmente?"*
