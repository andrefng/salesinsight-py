# SalesInsight PY

Análise e visualização de dados de vendas com Python.

## Objetivo

Organizar um fluxo de análise que gere ou carregue dados de vendas, inspecione sua estrutura, trate datas inválidas e produza métricas e visualizações.

O projeto permite acompanhar a receita por mês, identificar os produtos com maior receita, comparar categorias e regiões e segmentar clientes pelo gasto acumulado. Os resultados são exportados em CSV, JSON e imagens PNG.

## Contexto

Mini-projeto do Módulo 01 do curso de Desenvolvimento de IA para Análise Preditiva, utilizando conteúdos estudados até a Semana 07.

O desenvolvimento foi realizado individualmente, adotando a organização de branches e funcionalidades prevista para uma squad de até três integrantes.

## Tecnologias utilizadas

- Python: lógica e organização do programa.
- Pandas: leitura, tratamento, transformação e agregação dos dados.
- NumPy: configuração da semente utilizada no gerador.
- Matplotlib e Seaborn: criação e personalização dos gráficos.
- `datetime`, `random`, `os` e `json`: geração de dados, datas, arquivos e exportação.
- VS Code com as extensões Python e Jupyter: desenvolvimento e execução do notebook.
- Git e GitHub: versionamento e publicação do projeto.

## Preparação do ambiente

1. Instale o Python.
2. Instale o VS Code e as extensões Python e Jupyter.
3. No terminal, instale as dependências:

```bash
python -m pip install pandas numpy matplotlib seaborn ipykernel
```

Os módulos `datetime`, `random`, `os` e `json` fazem parte da biblioteca padrão do Python e não precisam de instalação adicional.

## Como executar

1. Abra a pasta `salesinsight-py` no VS Code.
2. Abra o arquivo `salesinsight.ipynb`.
3. Em **Selecionar Kernel**, escolha o ambiente Python em que as dependências foram instaladas.
4. Clique em **Reiniciar Kernel** e depois em **Executar Tudo**.

As primeiras células definem as funções, as configurações e a classe `AnalisadorDeVendas`. A última célula chama `main()` e executa o fluxo completo.

O programa carrega `vendas.csv`. Se o arquivo não existir, gera um dataset sintético com uma semente fixa para permitir a reprodução dos dados.

Durante a execução, são exibidos a inspeção inicial, o relatório de limpeza, as métricas, a segmentação de clientes, os quatro gráficos e a conferência do JSON exportado.

A conclusão é indicada pela mensagem:

```text
RF10 - Fluxo finalizado com sucesso
```

## Arquivos do projeto

```text
salesinsight-py/
├── .gitignore
├── README.md
├── salesinsight.ipynb
├── vendas.csv
└── outputs/
    ├── metricas_por_mes.csv
    ├── segmentacao_clientes.csv
    ├── estatisticas_gerais.json
    └── graficos/
        ├── receita_por_mes.png
        ├── top_produtos.png
        ├── quantidade_vs_receita.png
        └── painel_resumo.png
```

Os arquivos em `outputs` são gerados novamente durante a execução. Arquivos anteriores com os mesmos nomes são substituídos pelos resultados atuais.

## Conceitos aplicados

- Tipos de dados, operadores, condicionais e repetições.
- Listas, tuplas e dicionários.
- Funções com parâmetros, retorno e docstrings.
- Funções lambda e função de ordem superior.
- Classe com atributos e métodos para organizar o fluxo.
- Leitura e escrita de arquivos CSV e JSON.
- Geração e conversão de datas.
- DataFrames, filtros e seleções com Pandas.
- Remoção de espaços nas extremidades dos textos.
- Conversão de tipos e remoção de registros com datas inválidas.
- Operações vetorizadas e classificação condicional com `.loc`.
- Agregações com `groupby`.
- Gráficos de linha, barras e dispersão.
- Painel com subplots, personalização e exportação em PNG.

## Organização com Git e GitHub

O desenvolvimento foi dividido em tarefas, com testes e commits descritivos antes da integração à branch `develop`.

| Branch                       | Finalidade                                             |
|------------------------------|--------------------------------------------------------|
| `main`                       | Versão final validada do projeto.                      |
| `develop`                    | Integração das etapas concluídas.                      |
| `feat/leitura-limpeza`       | Geração, leitura, inspeção e tratamento dos dados.     |
| `feat/analise-metricas`      | Colunas derivadas, métricas e segmentação de clientes. |
| `feat/visualizacoes`         | Gráficos individuais e painel resumo.                  |
| `feat/funcoes-reutilizaveis` | Transformações com função de ordem superior.           |
| `feat/exportacao-resultados` | Exportação em CSV e gravação e leitura de JSON.        |
| `feat/classe-analisador`     | Classe analisadora e integração com a função `main()`. |
| `docs/readme-video`          | Documentação e apresentação do projeto.                |

As mensagens dos commits identificam as mudanças realizadas. As integrações utilizam commits de merge para registrar a conclusão de cada etapa.


## Vídeo de demonstração

Em preparação. O link será acrescentado após a gravação.


