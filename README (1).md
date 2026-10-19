# Árvore, Floresta ou Boosting? — Preditor de Falhas em Redes

Artigo técnico comparando Árvore de Decisão, Random Forest e XGBoost aplicados ao preditor de falha/risco em dispositivos de rede.

**Página publicada:** [COLAR O LINK depois de ativar o GitHub Pages]
**Autor:** Jonathan Ferreira Luna — Grupo 4

## Como reproduzir o experimento

1. Python 3.10+
2. Instalar dependências:
   ```bash
   pip install scikit-learn xgboost pandas
   ```
3. Ter em mãos `log_rede.csv` e `dataset_sintetico.csv` (gerados no projeto principal).
4. Rodar:
   ```bash
   python src/comparacao_modelos.py
   ```
5. O script imprime as métricas de cada modelo e salva `resultados_comparacao_modelos.csv`.

## Estrutura

```
.
├── index.html          # a página publicada
├── README.md
└── src/
    └── comparacao_modelos.py
```

## Dados usados

- `log_rede.csv`: 110 medições reais via ICMP (icmplib), coletadas em outubro de 2026.
- `dataset_sintetico.csv`: 150 registros sintéticos, gerados seguindo as mesmas regras de classificação.
- Nenhum dado real de tráfego de uma rede institucional, empresa ou IP identificável de terceiros foi publicado — apenas medições de ping contra serviços públicos (DNS públicos) e dados sintéticos.

## Licença

[definir, ex.: MIT]
