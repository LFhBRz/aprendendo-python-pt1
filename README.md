# Projeto Python: EntregaJá CG, agora com pandas

Mesmo problema do projeto de Power BI (dados fictícios de um app de delivery, mar a ago/2026), agora resolvido em Python.
Por que refazer: mostra que você domina o raciocínio, não só uma ferramenta, e permite fazer o que ficou pendente (recompra).

## Regras
- A análise é sua. A IA só para tirar dúvida DEPOIS de tentar, e declare no README o que usou.
- Escreva o raciocínio em células de texto (markdown) antes de cada bloco de código.
- Um commit por sessão.

## Fases (todas no notebook analise_entregaja.ipynb)
1. Conhecer os dados: tamanho, tipos, nulos, duplicados.
2. Auditoria e limpeza: crie um DataFrame pedidos_limpo e documente cada decisão.
3. Perguntas de negócio: cancelamento (onde e quando), tempo de entrega (o que influencia), clima, recompra e cupom.
4. Visualização: 4 gráficos com título, eixos e legenda legíveis.
5. Conclusões: 3 recomendações com número.
6. Comparação: seus resultados em Python batem com os do Power BI? Se não, descubra por quê.

## Cartão de funções (nomes, sem receita)
| Para quê | Procure por |
|---|---|
| Ler e inspecionar | read_csv, info, describe, shape, head, dtypes |
| Qualidade | isna, duplicated, drop_duplicates, value_counts, nunique |
| Texto | str.strip, str.title, str.lower, replace |
| Datas | to_datetime (parâmetros dayfirst, format, errors) |
| Filtrar e ordenar | loc, query, sort_values, isin, between |
| Resumir | groupby, agg, size, pivot_table, mean, median |
| Juntar tabelas | merge (how, left_on, right_on) |
| Criar colunas | assign, np.where, pd.cut, dt.month, dt.dayofweek |
| Pistas de recompra | groupby + min/max por cliente, diff entre datas, merge consigo mesmo |
| Gráficos | plot, seaborn (barplot, lineplot, boxplot, heatmap) |

## Entrega
Notebook executado de cima a baixo, pedidos_limpo.csv, README com descobertas e as seções de erros e transparência (use o modelo do projeto anterior).
