# Análise de Fraudes Bancárias

Projeto de análise de transações bancárias com foco em detectar padrões suspeitos e transações de risco, utilizando SQL e organização de dados.

## 📌 Objetivo
Analisar um conjunto de transações financeiras com objetivo de:
- Identificar padrões de comportamento suspeito;
- Filtrar transações marcadas como suspeitas;
- Agrupar e entender os clientes com maior número de ocorrências;
- Explorar comportamentos atípicos por país e valores elevados.

## 🧠 Tecnologias
- SQL para consultas e filtragens
- GitHub para versionamento

## 📁 Estrutura de dados
O dataset contém as colunas:
- `id_transacao` — Identificador único da transação  
- `id_cliente` — Identificador do cliente  
- `valor` — Valor da transação  
- `data_transacao` — Data registrada  
- `tipo_transacao` — Tipo (PIX, CARTÃO, etc.)  
- `pais` — País de origem  
- `status` — Aprovada ou Suspeita

## 📊 Exemplo de consulta SQL
```sql
SELECT *
FROM transacoes
WHERE status = 'SUSPEITA';
