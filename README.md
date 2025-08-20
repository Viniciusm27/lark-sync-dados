# Dados para sincronização com Lark Base

Este repositório contém arquivos de dados que podem ser sincronizados com o Lark Base e consumidos por outras ferramentas (ex.: Power BI).

## Arquivos
- `dados.csv` — tabela principal em CSV (separador: vírgula, decimal: ponto).
- `dados.json` — mesma tabela em JSON.

## Esquema
Campos:
- `id` (int) — identificador único
- `sku` (string)
- `produto` (string)
- `categoria` (string)
- `quantidade` (int)
- `preco` (number, decimal com ponto)
- `moeda` (string, ex.: BRL)
- `status` (string, ex.: ativo/inativo)
- `updated_at` (string, ISO 8601, ex.: 2025-08-19T16:00:00-03:00)
- `link` (string, URL)
- `tags` (string; separador por ponto-e-vírgula)

## Observações
- Use **ponto** como separador decimal (`29.90`), para evitar conflito com a vírgula do CSV.
- Atualize este arquivo sempre que alterar o esquema.
