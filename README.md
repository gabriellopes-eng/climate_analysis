# Climate Analysis — Análise Climática e Potencial Solar (1984–2014)

Projeto de análise climática com foco em **radiação solar** e em **potencial solar climático**, usando dados agregados para os municípios: **Esperança, Queimadas, Lagoa Seca, Solânea e Arara**.

## Dados

- Fonte: planilha Excel em `climate_analysis/data/raw/Dados climáticos de 1984 a 2014 - Formatado.xlsx`
- Aba usada nos notebooks: `dados`
- Variável-alvo (etapa preditiva): `W/m² - Radiação`

> Como a base não possui geração fotovoltaica (kWh), a **radiação solar mensal média (W/m²)** é usada como *proxy* do potencial solar climático.

## Notebooks (ordem sugerida)

1. `climate_analysis/notebooks/01_exploratory_analysis.ipynb` — análise exploratória
2. `climate_analysis/notebooks/02_tendencia_climatica.ipynb` — tendências climáticas
3. `climate_analysis/notebooks/03_sazonalidade.ipynb` — sazonalidade
4. `climate_analysis/notebooks/04_correlacao_regressao.ipynb` — correlação e regressão
5. `climate_analysis/notebooks/05_modelagem_potencial_fotovoltaico.ipynb` — modelagem do potencial
6. `climate_analysis/notebooks/06_indices_climaticos_solar.ipynb` — índices climáticos/solares
7. `climate_analysis/notebooks/07_extremos_climaticos.ipynb` — extremos climáticos
8. `climate_analysis/notebooks/08_modelagem_preditiva.ipynb` — previsão mensal (ARIMA/SARIMA vs Random Forest/Gradient Boosting)

## Requisitos

Instalação para executar os notebooks:

```bash
pip install -r requirements.txt
```

## Como executar (Windows / VS Code)

1. Criar e ativar ambiente virtual:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Instalar dependências:

```powershell
pip install -r requirements.txt
```

3. Abrir e executar os notebooks:

- Abra um notebook em `climate_analysis/notebooks/`
- Selecione o kernel do Python do `.venv`
- Execute as células na ordem (idealmente “Run All”)

## Estrutura do projeto

- `climate_analysis/notebooks/` — notebooks do trabalho
- `climate_analysis/data/raw/` — dados brutos (Excel)
- `climate_analysis/docs/` — documentação (quando aplicável)
