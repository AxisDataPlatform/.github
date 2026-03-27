## 🚀 Axis Data Platform | Pull Request Template

### 📋 Descrição do PR
*Descreva brevemente as alterações feitas e como elas impactam o eixo central de dados (Axis).*

- **Ticket/Issue:** # (link aqui)
- **Tipo de Alteração:** [ ] Bugfix | [ ] Feature | [ ] Refatoração | [ ] Documentação

---

## 💎 Axis Quality Checklist (Obrigatório)
*Ao marcar estes itens, você garante que o código mantém o padrão de perfeição do **Axis Data Platform**.*

### 1. Integridade e Exatidão (The Core)
- [ ] **Data Quality:** Foram incluídos testes de `unique`, `not_null` ou de integridade referencial?
- [ ] **Tratamento de Erros:** O pipeline lida com dados malformados sem interromper o fluxo crítico?
- [ ] **Idempotência:** O processo pode ser reexecutado para o mesmo período sem gerar duplicidade?

### 2. Performance e Governança (The Flow & Shield)
- [ ] **Otimização:** As queries utilizam partições e evitam *Full Table Scans* desnecessários?
- [ ] **LGPD/Privacidade:** Dados sensíveis (PII) estão mascarados ou protegidos conforme as normas?
- [ ] **Linhagem:** Novas tabelas ou colunas foram documentadas no catálogo de dados/Wiki?

### 3. Padrões Axis (The Standard)
- [ ] **Nomenclatura:** Segue o padrão `axis_v1_...` e usa *snake_case* claro?
- [ ] **DRY:** A lógica evita repetições e utiliza macros ou funções reutilizáveis onde possível?
- [ ] **Documentação:** O código está comentado explicando o "porquê" de regras de negócio complexas?

---

## 🧪 Evidências de Testes
*Cole aqui logs, prints de validação ou queries de teste que comprovem que o dado está correto.*

```sql
-- Exemplo de query de validação executada:
SELECT count(*), status FROM axis_v1_sua_tabela GROUP BY 2;
