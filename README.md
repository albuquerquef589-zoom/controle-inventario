# 📦 Controle de Inventário Geral

Planilha em Excel para **inventário geral** com leitura por **coletor de código de barras**, status por cores e dashboard com gráficos para apresentação à gerência.

> ⚠️ Este repositório contém apenas um **modelo com dados fictícios**. Os dados reais da empresa são confidenciais e não são versionados.

## Como funciona

| Aba | Função |
|---|---|
| **Dashboard** | Resumo, gráficos por status, corredor, responsável e dia |
| **Bipagem** | Digita-se a **posição**, bipa-se o **material**, escolhe-se o **responsável** |
| **Data** | Base de posições. Preenche-se **SISTEMA**; **FISICO**, **STATUS** e cores são automáticos |
| **Config** | Lista de responsáveis, motivos e data de início |
| **LEIA-ME** | Passo a passo de uso |

## Status

| Cor | Status | Significado |
|---|---|---|
| 🟢 | OK | Contagem física igual ao sistema |
| 🔴 | DIVERGENTE | Contagem diferente. Exige **motivo** |
| 🔴 | NÃO FEITO | Posição não contada, com **motivo** informado |
| 🟠 | PENDENTE | Ainda não contada |

## Como usar

1. Abra `inventario_modelo.xlsx`.
2. Na aba **Data**, preencha a coluna **SISTEMA**.
3. Na aba **Bipagem**, digite a posição e bipe os materiais com o coletor.
4. Nas divergências, escolha o **motivo** na aba **Data**.
5. Acompanhe tudo no **Dashboard**.

### Data/hora automática (opcional)
Use a macro em [`macro_data_hora.txt`](macro_data_hora.txt) (salvar como `.xlsm`) ou os atalhos `Ctrl+;` e `Ctrl+Shift+;`.

## Tecnologias
Excel (fórmulas `COUNTIFS`, `MAXIFS`, formatação condicional, gráficos) e VBA opcional.

---

<sub>Feito por Fernando Luiz Santos Albuquerque · Cursando Gestão da Tecnologia da Informação · Suporte Técnico</sub>
