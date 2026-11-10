# Previsão do Pico Diário de Carga – Subsistema Sul

Projeto Final da disciplina de **Ciência de Dados** – UTFPR Campo Mourão
Prof. Dr. Eduardo Pena

## Integrantes

- Lucas dos Santos Vaz – RA 2020955

## Problema

Prever a **carga máxima diária** do subsistema **Sul** do Sistema Interligado Nacional
com um dia de antecedência, investigando a influência do clima e dos feriados no pico
de demanda.

## Dados

| Fonte | Uso | Link |
|---|---|---|
| ONS – Curva de Carga Horária | Série principal (pico diário calculado a partir da carga horária) | https://dados.ons.org.br/dataset/curva-carga |
| ONS – Demanda Máxima Diária por Subsistema | Conferência do pico calculado (2024+) | https://dados.ons.org.br/dataset/demanda_maxima_di |
| Open-Meteo / INMET | Variáveis climáticas | https://open-meteo.com/ |
| Biblioteca `holidays` | Feriados nacionais e estaduais (PR, SC, RS) | https://pypi.org/project/holidays/ |

## Estrutura do repositório

```
├── data/
│   ├── raw/          # arquivos originais baixados (não versionados)
│   └── processed/    # base final em Parquet
├── docs/             # proposta, relatório e slides
├── notebooks/        # notebooks de cada etapa
├── src/              # scripts de download e preparação
└── requirements.txt
```

## Como reproduzir

```bash
python -m venv .venv
.venv\Scripts\activate        # Windows  (Linux/Mac: source .venv/bin/activate)
pip install -r requirements.txt
```

As instruções de execução do pipeline serão adicionadas nas próximas etapas.

## Entregas

- [x] Etapa 1 – Proposta (`docs/`)
- [ ] Etapa 2 – Preparação e integração dos dados
- [ ] Etapa 3 – Análise exploratória e consultas SQL
- [ ] Etapa 4 – Modelagem e experimentos
- [ ] Etapa 5 – Relatório e apresentação
