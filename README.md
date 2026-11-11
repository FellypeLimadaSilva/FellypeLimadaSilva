<h1 align="center">Fellype Lima da Silva</h1>

<p align="center">
  <strong>Data Engineer</strong><br>
  Big Data · Pipelines ELT/ETL · Arquitetura Medalhão · Data Warehouse e Lakehouse<br>
  Confiabilidade, qualidade e governança de dados
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/fellype-lima-5a5aa7269/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:fellypelima333@gmail.com">
    <img src="https://img.shields.io/badge/Email-24292F?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white"/>
  <img src="https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white"/>
  <img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQL%20Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
</p>

---

## Sobre

Engenheiro de Dados na **OUD Tecnologia** e bacharelando em Engenharia de Software na **UNIVAG** — 8º semestre, conclusão em dezembro de 2026.

Atuo na camada que sustenta o dado: ingestão idempotente, processamento distribuído com PySpark, modelagem em camadas, transformação versionada em SQL, testes de qualidade como portão de publicação e orquestração de pipelines. Trabalho com Big Data e com data warehouses em nuvem (BigQuery, Databricks). O que eu entrego sobe em container, passa por CI e tem caminho de volta.

---

## Arquiteturas e padrões

| Arquitetura / padrão | Onde aplico |
|---|---|
| **Medalhão (bronze → silver → gold)** | camadas com responsabilidades separadas: dado cru e rastreável, dado tipado e limpo, dado modelado e publicado |
| **ELT e ETL** | ingestão do dado como veio e transformação versionada em SQL (dbt); ETL quando o processamento exige Python ou Spark |
| **Data Warehouse** | staging → data mart, modelagem dimensional, fatos e dimensões |
| **Lakehouse** | armazenamento em lake com processamento distribuído e governança de tabelas (Databricks) |
| **Processamento distribuído** | transformações em larga escala com PySpark e SQL analítico em BigQuery |
| **Orquestração por DAGs** | dependências, retries, agendamento e observabilidade de execuções (Airflow) |
| **Data quality gates** | testes de fontes, schema, unicidade e integridade que bloqueiam a publicação |
| **Data contracts** | fontes, colunas essenciais, filtros e regras declarados em YAML antes do código |
| **Publicação atômica + rollback** | troca de schema em transação única, com a versão anterior preservada |

---

## Bancos de dados e armazenamento

| Categoria | Tecnologias |
|---|---|
| **Relacionais (OLTP e DW)** | PostgreSQL · SQL Server · MySQL · SQLite |
| **Data warehouse em nuvem** | Google BigQuery · Databricks |
| **Big Data / processamento** | Apache Spark (PySpark) · Pandas |
| **Modelagem** | dimensional (star schema), camadas medalhão, normalização, particionamento e índices |

---

## Princípios de engenharia

| Princípio | Como aparece nos projetos |
|---|---|
| **Idempotência** | manifesto de arquivos com SHA-256 — rodar de novo não duplica nem recarrega dado |
| **Qualidade como portão** | a camada final só é publicada se as fontes obrigatórias e todos os testes do dbt passarem |
| **Linhagem e auditoria** | cada linha carrega arquivo e lote de origem; trilha de execuções e publicações em `ops` |
| **Separação de privilégios** | roles distintas para ingestão, transformação e leitura |
| **CI que exercita o pipeline** | lint de Python e SQL, testes unitários e de integração em PostgreSQL real, build da imagem |
| **Reprodutibilidade** | ambiente inteiro em Docker Compose; infraestrutura versionada junto com o código |

---

## Projetos em destaque

### [`datahack`](https://github.com/FellypeLimadaSilva/datahack) — Rota do Diploma · 1º lugar no DataHack UNIVAG 2026

Plataforma de dados ponta a ponta sobre microdados do INEP e a API do IBGE, em arquitetura medalhão (bronze → silver → gold). A ingestão nunca quebra por tipo: o dado entra como veio e a conversão é medida e testada no dbt. A Gold só é promovida com os portões aprovados, por troca atômica de schema, com `rollback` disponível.

`PostgreSQL 16` · `Python 3.12` · `dbt-core 1.12` · `Airflow 3.3` · `Docker Compose` · `GitHub Actions`

Meu papel: arquitetura ELT, ingestão, modelagem no dbt, DAGs do Airflow, testes de qualidade e publicação da camada Gold.

### [`Data-Warehouse`](https://github.com/FellypeLimadaSilva/Data-Warehouse) — pipeline de commodities

Pipeline de ingestão de séries de preços com carga em PostgreSQL e modelagem em camadas (staging → data mart) no dbt. Separação explícita entre extração, armazenamento e transformação, com credenciais fora do código.

`Python` · `PostgreSQL` · `dbt-core` · `SQLAlchemy` · `Pandas`

### [`fastapi-pedidos-api`](https://github.com/FellypeLimadaSilva/fastapi-pedidos-api) — API REST com autenticação JWT

Serviço REST com autenticação por JWT, camada de persistência em SQLAlchemy e migrações versionadas com Alembic.

`Python` · `FastAPI` · `SQLAlchemy` · `Alembic` · `JWT`

---

## Stack completa

**Linguagens** &nbsp;
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white"/>

**Big Data e processamento** &nbsp;
<img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white"/>
<img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white"/>
<img src="https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>

**Transformação e orquestração** &nbsp;
<img src="https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white"/>
<img src="https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white"/>

**Bancos de dados** &nbsp;
<img src="https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/SQL%20Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white"/>

**Backend** &nbsp;
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white"/>

**Infraestrutura e qualidade** &nbsp;
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
<img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white"/>
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>

---

## Aprofundando agora

Formatos de tabela para lakehouse, observabilidade de pipelines, modelagem dimensional avançada e segurança de dados.

---

<p align="center">
  <a href="https://www.linkedin.com/in/fellype-lima-5a5aa7269/">LinkedIn</a> ·
  <a href="mailto:fellypelima333@gmail.com">fellypelima333@gmail.com</a> ·
  Várzea Grande · Cuiabá, MT
</p>
