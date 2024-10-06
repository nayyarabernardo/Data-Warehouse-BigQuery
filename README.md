# Data-Warehouse-BigQuery

## Descrição do Projeto

Este projeto tem como objetivo a criação de um Data Warehouse utilizando o **Google BigQuery**. O Data Warehouse servirá como uma solução centralizada para armazenar e modelar dados que serão consumidos para análises e dashboards. Durante o processo, serão abordadas etapas como a ingestão de dados, processamento, transformação e modelagem dos dados.

O projeto está em andamento e, até o momento, inclui um **notebook** para a ingestão de dados a partir de um bucket do Google Cloud Storage.

## Estrutura Atual

Até agora, o projeto contém os seguintes componentes:

- **Notebooks**:
  - `data_ingestion_notebook.ipynb`: Notebook responsável pela ingestão de dados a partir de um bucket no Google Cloud Storage. Este notebook inclui as etapas de:
    - Carregamento dos arquivos de dados brutos para o BigQuery.
    - Configuração das permissões e credenciais de acesso.
  
### Estrutura de Diretórios

```bash
.
├── notebooks
│   └── data_ingestion_notebook.ipynb   # Notebook de ingestão
├── data                               # Pasta para armazenar arquivos locais temporariamente
├── scripts                            # Scripts para automatização (em breve)
└── README.md                          # Este arquivo
```

## Funcionalidades Futuras

O desenvolvimento do projeto incluirá as seguintes etapas:

- **Automatização do Processo de Ingestão**: Criação de scripts em Python/Bash para automatizar o processo de ingestão dos dados de forma programática e eficiente.
- **Transformação e Modelagem dos Dados**: Aplicação de transformações e criação de tabelas no BigQuery seguindo uma arquitetura medallion (Bronze, Silver, Gold).
- **Validação de Dados**: Implementação de validação e limpeza dos dados para garantir a qualidade no processo de ETL.
- **Dashboards**: Conexão com ferramentas de BI, como Looker Studio, para a visualização dos dados modelados.

## Requisitos

- **Google Cloud SDK**
- **Python 3.x**
- **BigQuery API**

### Configurações Iniciais

1. Clone este repositório:
   ```bash
   git clone https://github.com/nayyarabernardo/Data-Warehouse-BigQuery/.git
   ```

2. Instale as dependências necessárias:
   ```bash
   pip install -r requirements.txt
   ```

3. Configure suas credenciais do Google Cloud:
   ```bash
   gcloud auth application-default login
   ```

4. Execute o notebook de ingestão:
   Abra o Jupyter Notebook e execute o arquivo `data_ingestion_notebook.ipynb`.

## Próximos Passos

- Desenvolvimento de scripts automatizados de ingestão.
- Implementação da camada de transformação e modelagem.
- Atualização contínua do README conforme novas funcionalidades forem adicionadas.
