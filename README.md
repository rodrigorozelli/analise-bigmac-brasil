# 🍔 Índice Big Mac vs REER — Brasil 2000-2026

O índice Big Mac ajustado pelo PIB teria servido como alerta de sobrevalorização
cambial do real? Este notebook compara a série do Big Mac (The Economist) com o
REER amplo do BIS para o Brasil.

## Conclusão principal
Em jul/2011 o Big Mac ajustado do Brasil atingiu **+1,47** (real ~147% acima do
que o PIB/cap justificava). O REER confirma o pico no mesmo período.
Correlações: **Big Mac raw × REER = +0,94** · **Big Mac ajustado × REER = +0,91**.
Ex-post, o real desvalorizou ~60% até 2015-16 — a correção que o esticamento exigia.

## O que os gráficos mostram
- `brasil_bigmac_vs_reer_v2.png`: Big Mac (raw/ajustado) vs REER suavizado, com
  crises sombreadas. Mesmo sinal, mesmo timing.
- `latam_3_epocas.png`: valuation ajustado na América Latina em 2003 / 2011 / 2026.
  Brasil: barato (crise) → caro (boom, +1,47) → barato (hoje).

## Metodologia & fontes
- Big Mac: github.com/TheEconomist/big-mac-data (índices raw e GDP-adjusted)
- REER: BIS via FRED (RBBRBIS, índice 2020=100, mensal)
- Literatura: UNCTAD 2011, OCDE 2011, Oreiro 2014 (~48% sobreval.), Soo 2015

## Ressalvas
Correlação em níveis pode ser inflada por tendência comum (o rigor exigiria
primeiras diferenças). n=1 (Brasil) não valida poder preditivo geral — requer
teste em painel. Sinal ≠ timing (real ficou esticado até ~2013).

Feito com Python (pandas, matplotlib) no Colab. Meu primeiro projeto de ciência
de dados — clonado, estudado, executado e estendido a partir de um repo público.
