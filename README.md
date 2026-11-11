<h1 align="center">Fellype Lima da Silva</h1>

<p align="center">
  <strong>Data Engineer</strong><br>
  Pipelines ELT · modelagem em camadas · confiabilidade e qualidade de dados
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/fellype-lima-5a5aa7269/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:fellypelima333@gmail.com">
    <img src="https://img.shields.io/badge/Email-24292F?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
</p>

---

## Sobre

Engenheiro de Dados Júnior na **OUD Tecnologia** e bacharelando em Engenharia de Software na **UNIVAG** — 8º semestre, conclusão em dezembro de 2026.

Trabalho na camada que sustenta o dado: ingestão idempotente, modelagem em camadas, transformação versionada em SQL, testes de qualidade como portão de publicação e orquestração. O que eu entrego sobe em container, passa por CI e tem caminho de volta.

---

## Princípios que aplico

| Princípio | Como aparece nos projetos |
|---|---|
| **Idempotência** | manifesto de arquivos com SHA-256 — rodar de novo não duplica nem recarrega dado |
| **Qualidade como portão** | a camada final só é publicada se as fontes obrigatórias e todos os testes do dbt passarem |
| **Publicação atômica + rollback** | troca de schema em transação única; a versão anterior fica preservada |
| **Linhagem e auditoria** | cada linha carrega arquivo e lote de origem; trilha de execuções e publicações em `ops` |
| **Contrato antes de código** | fontes, colunas essenciais, filtros e regras de exportação declarados em YAML |
| **Separação de privilégios** | roles distintas para ingestão, transformação e leitura |
| **CI que exercita o pipeline** | lint de Python e SQL, testes unitários e de integração em PostgreSQL real, build da imagem |

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

## Stack

**Linguagens** &nbsp;
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white"/>

**Transformação e orquestração** &nbsp;
<img src="https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white"/>
<img src="https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white"/>
<img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white"/>

**Armazenamento** &nbsp;
<img src="https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/SQL%20Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white"/>
<img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white"/>

**Backend** &nbsp;
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white"/>

**Infraestrutura e qualidade** &nbsp;
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
<img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white"/>
<img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white"/>
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>

---

## Aprofundando agora

Processamento distribuído com Spark, lakehouse e formatos de tabela, observabilidade de pipelines, modelagem dimensional avançada e segurança de dados.

---

<p align="center">
  <a href="https://www.linkedin.com/in/fellype-lima-5a5aa7269/">LinkedIn</a> ·
  <a href="mailto:fellypelima333@gmail.com">fellypelima333@gmail.com</a> ·
  Várzea Grande · Cuiabá, MT
</p>
<h1 align="center">Olá, eu sou Fellype Lima da Silva</h1>

<p align="center">
  Engenheiro de Dados Júnior na OUD Tecnologia<br>
  Bacharelando em Engenharia de Software - UNIVAG<br>
  Python, SQL, ETL/ELT, pipelines e modelagem de dados
</p>

<p align="center">
  <a href="https://github.com/FellypeLimadaSilva">
    <img src="https://komarev.com/ghpvc/?username=FellypeLimadaSilva&color=0e75b6&style=flat" alt="Profile views"/>
  </a>
  <a href="https://www.linkedin.com/in/fellype-lima-5a5aa7269/">
    <img src="https://img.shields.io/badge/LinkedIn-Fellype%20Lima-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
</p>

---

## Sobre mim

Atuo como Engenheiro de Dados Júnior, com foco na construção, organização e análise de soluções orientadas a dados.

Tenho experiência com Python, SQL, SQL Server e Git/GitHub, aplicando esses conhecimentos em manipulação de dados, consultas, tratamento de informações, estruturação de bases e apoio à tomada de decisão.

Atualmente venho aprofundando minha atuação em Engenharia de Dados, especialmente em desenvolvimento de pipelines, processos de ETL/ELT, modelagem de dados, qualidade de dados e organização de bases para uso analítico.

---

## Atuação atual

**Engenheiro de Dados Júnior - OUD Tecnologia**

Atuação com dados em ambiente profissional, utilizando Python, SQL e ferramentas de análise para apoiar processos de tratamento, transformação, consulta e visualização de informações.

Principais frentes:

- Manipulação e transformação de dados com Python
- Criação e otimização de consultas SQL
- Apoio em processos de ETL/ELT
- Organização e estruturação de bases de dados
- Desenvolvimento de relatórios e dashboards
- Análise de dados para suporte à tomada de decisão

---

## Tecnologias e ferramentas

<p align="center">
  <img src="https://skillicons.dev/icons?i=python" title="Python"/>
  <img src="https://skillicons.dev/icons?i=postgres" title="PostgreSQL"/>
  <img src="https://skillicons.dev/icons?i=mysql" title="MySQL"/>
  <img src="https://skillicons.dev/icons?i=sqlite" title="SQLite"/>
  <img src="https://skillicons.dev/icons?i=fastapi" title="FastAPI"/>
  <img src="https://skillicons.dev/icons?i=git" title="Git"/>
  <img src="https://skillicons.dev/icons?i=github" title="GitHub"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white" title="SQL Server"/>
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" title="PostgreSQL"/>
  <img src="https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white" title="dbt"/>
  <img src="https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white" title="Databricks"/>
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" title="Apache Spark"/>
  <img src="https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white" title="Apache Airflow"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" title="Docker"/>
</p>

---

## Engenharia de Dados em evolução

Ferramentas, conceitos e práticas que venho estudando e aplicando para evoluir na área:

- Pipelines de dados
- ETL/ELT
- Modelagem dimensional
- Data warehouse
- Lakehouse
- Qualidade de dados
- dbt
- Databricks
- PySpark
- Orquestração de pipelines

---

## Projetos em destaque

- [projeto-bi-academia-jiu-jitsu](https://github.com/FellypeLimadaSilva/projeto-bi-academia-jiu-jitsu): projeto de Business Intelligence com modelagem dimensional, ETL e dashboards em Power BI.
- [Data-Warehouse](https://github.com/FellypeLimadaSilva/Data-Warehouse): pipeline de dados para monitoramento de commodities usando Python, PostgreSQL, dbt e Streamlit.
- [fastapi-pedidos-api](https://github.com/FellypeLimadaSilva/fastapi-pedidos-api): API REST para autenticação JWT e gerenciamento de pedidos utilizando FastAPI, SQLAlchemy e SQLite.

---

## Contato

<p align="center">
  <a href="https://www.linkedin.com/in/fellype-lima-5a5aa7269/" title="LinkedIn">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  
  <a href="mailto:fellypelima333@gmail.com" title="Enviar Email">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  
  <a href="https://www.instagram.com/fellype1222/" title="Instagram">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/>
  </a>
</p>

