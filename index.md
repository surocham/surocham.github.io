# Portfólio <a name="inicio"></a>

## Sobre mim

Profissional em transição para a área de dados, com experiência prática em análise, organização e interpretação de dados voltados à tomada de decisão. Ao longo da minha trajetória como desenvolvedora mobile, desenvolvi uma visão analítica apurada, trabalhando diretamente com dados de uso de aplicações, métricas de performance e ciclos de entrega orientados a resultado.

Domino ferramentas como **SQL, Power BI, Python e Excel** para extração, tratamento e visualização de dados. Tenho facilidade para comunicar insights a públicos técnicos e não técnicos, habilidade desenvolvida em projetos com clientes e times multidisciplinares ao longo da minha experiência como desenvolvedora.

Contribuí para entregas que resultaram em redução de aproximadamente 20% em erros recorrentes em aplicações mobile, além de apoiar mais de 10 funcionalidades entregues dentro do prazo e escopo definidos pelo time de produto.

Busco oportunidades como Analista de Dados onde possa aplicar minha capacidade analítica, meu conhecimento técnico em dados e minha experiência com metodologias ágeis para gerar valor real ao negócio.

Analitica de Dados | Data Analytics | Business Intelligence | BI | ETL | Tratamento de Dados | Limpeza de Dados | Data Cleaning | Visualizacao de Dados | Data Visualization | Dashboard | KPI | Metricas | Tomada de Decisao Baseada em Dados | Data-Driven | Storytelling com Dados | Analise Exploratoria | EDA | Pandas | NumPy | Power Query | DAX | SQL Server | PostgreSQL | MySQL | Relatorio Gerencial | Insights | Analista de Dados Junior | Junior Data Analyst | Transicao de Carreira em Dados | Scrum | Kanban | Metodologias Ageis

---

## Projetos<a name="projetos"></a>

### Pipeline ETL com Airflow e Docker

![image](/assets/airflow.jpg)

**Contexto e Problema:**

Em um cenário de estudo prático de orquestração de dados, eu precisava construir um pipeline ETL que extraísse a tabela customers de um banco PostgreSQL (fonte – source_db), armazenasse localmente e carregasse os dados em outro banco PostgreSQL (destino – `target_db`). O desafio era garantir que o processo fosse automatizado, agendado e monitorado, utilizando tecnologias modernas como Apache Airflow e Docker. Além disso, era necessário tratar problemas comuns de rede entre containers, compatibilidade de versões do Airflow e persistência de arquivos temporários.

**Objetivos:**

O objetivo principal era desenvolver uma DAG no Apache Airflow com quatro tarefas encadeadas:

1. Extrair os dados do `source_db` e salvá‑los em CSV.

2. Validar a existência e integridade do arquivo CSV.

3. Carregar o conteúdo do CSV no `target_db`.

4. Validar a carga comparando a contagem de registros entre o CSV e a tabela de destino.

Requisitos adicionais:

- O pipeline deveria rodar dentro de containers Docker, com os bancos em redes isoladas.

- O código deveria ser versionado, documentado e reproduzível.

Ao final, o `target_db` deveria conter exatamente os mesmos 91 clientes existentes no `source_db`.


**Resultado:**
Resultados técnicos

Pipeline ETL funcional e agendado diariamente, sem intervenção manual.

Migração bem‑sucedida de 91 registros da tabela customers do source_db para o target_db.

Validação automática garantiu integridade dos dados (100% de correspondência entre CSV e destino).

Código disponível em repositório público, com README.md detalhado e documentação dos erros e soluções.

Aprendizados e competências desenvolvidas

Orquestração de pipelines com Apache Airflow (DAGs, operadores, sensores).

Comunicação entre containers Docker em redes personalizadas.

Tratamento de problemas reais de ambiente: credenciais, caminhos de arquivo, compatibilidade de versões.

Boas práticas de segurança (uso de Connections do Airflow – mencionado no README).

Documentação de portfólio com método STAR, facilitando a comunicação com recrutadores.

#### Para acessar o projeto basta clicar: 

[![View on GitHub](https://img.shields.io/badge/GitHub-Ver_no_GitHub-darkgreen?logo=GitHub)](https://github.com/surocham/desafio_pratico_fundamentos_DE)

---

### Pipeline de web scraping utilizando Selenium WebDriver para extrair e estruturar dados públicos

**Contexto:**

No início de 2025, participei de um desafio técnico promovido pela He4rt Developers, uma comunidade muito forte na área de tecnologia. O desafio consistia em construir um web scraper utilizando Selenium WebDriver para extrair dados públicos do Portal da Transparência de uma prefeitura brasileira. A ideia era simular um cenário real de trabalho em engenharia de dados: antes de qualquer análise, é preciso coletar, estruturar e tratar os dados brutos, que muitas vezes não estão em formatos amigáveis.

Eu nunca havia trabalhado com Selenium antes, e o desafio era grande: em poucos dias, precisava aprender a automatizar a navegação em um site governamental, extrair uma tabela dinâmica e ainda entregar um dataset limpo e documentado. O projeto seria avaliado não só pela funcionalidade, mas também pela organização, boas práticas e uso de ferramentas como Docker.

**Objetivos:**

Meu objetivo principal era entregar um scraper funcional que extraísse dados de um portal de transparência municipal, estruturasse esses dados em um dataset tabular (CSV) e o deixasse pronto para análises futuras. Os requisitos técnicos do desafio eram:

- Usar Selenium WebDriver obrigatoriamente (linguagem livre, escolhi Python).

- Extrair dados de pelo menos uma tabela do portal (com múltiplas linhas e colunas).

- Realizar limpeza e transformação dos dados, padronizando formatos e tratando valores inconsistentes.

- Salvar o resultado final em um arquivo CSV ou similar.

- Opcional (bônus): usar Docker para executar o scraper, implementar scroll/paginação para carregar todos os dados, e estruturar o código seguindo o padrão ETL.

- Por fim, publicar tudo no GitHub com um README detalhado.

Minha escolha foi extrair a folha de pagamento IPREM - 2025 da Prefeitura de São Paulo, uma tabela com informações como nome do servidor, cargo, lotação, remunerações etc. A tabela era dinâmica (SlickGrid) e estava dentro de um iframe com carregamento lento.

**Resultados:**
Entregáveis técnicos

- Um scraper funcional que extrai a folha de pagamento IPREM de 2025 da Prefeitura de São Paulo.

- Um dataset estruturado em CSV com 12 colunas e dezenas de registros (exemplo: MARIA LENALDA DOS SANTOS SILVA, cargo CHEFE DE EQUIPE I, total de remuneração R$ 20.615,89).

- Código 100% Python, modularizado em funções separadas (extract, transform, load).

- Uso de Docker para execução do Selenium, garantindo reprodutibilidade.

- Documentação completa no README.md, incluindo capturas de tela do ambiente, da execução e da identificação de elementos via XPath.

- Versionamento no GitHub com 8 commits.

**Validação dos dados**

Apliquei limpeza consistente: padronização de strings, conversão de tipos, tratamento de datas, remoção de duplicatas e de registros inconsistentes. A coluna total_remuneracao foi calculada automaticamente.

**Aprendizados e competências desenvolvidas**

- Web scraping com Selenium: domínio de seletores CSS, iframes, scroll dinâmico, esperas explícitas.

- Docker para automação: uso de imagens prontas como selenium/standalone-chrome, mapeamento de portas.

- Tratamento de dados com Pandas: limpeza avançada, padronização, conversão de tipos, cálculos derivados.

- Resolução de problemas complexos: identificação de elementos com IA, scroll progressivo, controle de duplicatas.

- Documentação de portfólio: aprendi a importância de documentar também as dificuldades, não apenas o código final.

- Autodidatismo: fui capaz de aprender uma tecnologia do zero em três dias, combinando múltiplas fontes.

#### Para acessar o projeto basta clicar em: 
[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-darkgreen?logo=GitHub)](https://github.com/surocham/Desafio_He4rt_Data)

---

Entre em contato comigo por meio de:

[<img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">](https://www.linkedin.com/in/surocham/)
[<img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=black" alt="Gmail">](mailto:suamirochati@gmail.com)

© 2026 Suami Evelin Rocha de Medeiros.
