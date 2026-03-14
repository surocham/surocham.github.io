# Portfólio <a name="inicio"></a>

## Sobre mim 
Profissional com experiência em análise de dados. Tenho habilidades em modelagem de dados, construção de pipelines, desenvolvimento de soluções end-to-end e criação de dashboards analíticos.  

Minha experiência em análise de dados no estágio durante a graduação, deu origem à minha trajetória na área. Durante esse período, percebi como a análise de dados pode impactar significativamente a melhoria de processos e potencializar a geração de resultados positivos.   
   
Meu objetivo é apoiar empresas na tomada de decisões, oferecendo soluções baseadas em dados para impulsionar o crescimento e a inovação.    

**Habilidades Técnicas:**    
- Linguagens: Python, SQL e R
- Ferramentas: Airflow, Amazon QuickSight, dbt, Git e Power BI.  
   
---
## Projetos End to End <a name="projetos-end-to-end"></a>

### Pipeline para migração de tabela com Airflow e Docker
![image](/assets/airflow.jpg)

**Contexto:** Documentação completa do processo de construção de um pipeline ETL para migrar a tabela customers do source_db para o target_db usando Apache Airflow orquestrado via Astro CLI.

**Objetivos:** 
O objetivo do projeto é construir um pipeline ETL que:

Extrai a tabela customers do banco source_db
Salva os dados localmente em um arquivo CSV
Carrega os dados no banco target_db
Valida a integridade da carga comparando contagens

**Resultados:**
- Airflow

Parâmetros como days_ago e schedule_interval foram descontinuados — sempre verifique a versão instalada
O Airflow detecta mudanças na pasta dags/ automaticamente em ~30 segundos, sem precisar reiniciar
O painel de Erros de Importação é o primeiro lugar a verificar quando uma DAG não aparece

- Docker

localhost dentro de um container nunca aponta para outros serviços — use o nome do serviço
Serviços em docker-compose diferentes ficam em redes separadas por padrão
Volumes precisam ser mapeados no container correto — mapear no source_db não adianta se quem grava é o Airflow

Boas práticas

Nunca colocar credenciais diretamente no código — usar as Connections do Airflow (Admin > Connections)
Sempre ler o log completo da task que falhou, não apenas a mensagem resumida
Documentar a ordem de inicialização quando há dependências entre serviços

**Ferramentas e Tecnologias Utilizadas:**
- Airflow
- Docker
- Git
- Python
- SQL
- Visual Studio Code  

#### Para acessar o projeto basta clicar em:      [![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/surocham/desafio_pratico_fundamentos_DE)
---
### Pipeline de web scraping utilizando Selenium WebDriver para extrair e estruturar dados públicos


**Contexto:** O projeto simula um cenário real de trabalho em ciência de dados e engenharia de dados: antes de realizar qualquer análise, é necessário coletar, estruturar e tratar os dados brutos.


**Objetivos:**
Cada participante deverá desenvolver um scraper capaz de navegar em um portal de transparência municipal, extrair dados relevantes e organizá-los em uma tabela estruturada pronta para análise.

Os dados coletados serão posteriormente utilizados em uma live técnica, onde serão exploradas técnicas analíticas de ciência de dados sobre a base construída pelos participantes.

**Resultados:**
• Qual portal foi utilizado?

O portal usado foi: IPREM - Folha de Pagamento - 2025 da Prefeitura de São Paulo URL

• Qual município foi analisado?

São Paulo

• Quais dados foram coletados

Folha de pagamento IPREM


**Ferramentas e linguagens utilizadas:**
- Git
- Selenium Web Driver
- Python
- Docker
- Visual Studio Code
  
#### Para acessar o projeto basta clicar em:      [![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/surocham/Desafio_He4rt_Data)
---
### Artigo Análise de Correspondência Simples
![image](https://substackcdn.com/image/fetch/$s_!i_Tf!,w_1456,c_limit,f_webp,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F8d82c6d7-dc0d-4f42-b898-1cf27bc6615c_498x270.gif)

**Contexto:** Um projeto completo de Análise de Correspondência Simples (CA) usando Python, onde exploramos as relações entre as aldeias do mundo Naruto e os estilos de luta dos shinobis.

**Objetivos:**
1	Importação de bibliotecas	Reunir o squad
2	Carregamento dos dados	Ler o relatório da missão
3	Tabela de contingência	Ver quantos shinobis de cada aldeia preferem cada estilo
4	Perfis de linha e coluna	Montar o "perfil de combate" de cada aldeia
5	Teste Qui-Quadrado	Confirmar que a associação não é coincidência
6	Resíduos padronizados	Encontrar os "Rock Lees" dos dados
7	Decomposição SVD	Usar o Sharingan — focar no que importa
8	Mapa de Correspondência	Desenhar o mapa final do mundo dos shinobis
9	Interpretação	Entender quem se pareça com quem

**Resultados:**
A Análise de Correspondência é um mapa que mostra quais categorias se parecem entre si, sem precisar olhar para uma tabela cheia de números!

**Ferramentas e linguagens utilizadas:**
- Git
- Python
- Visual Studio Code

#### Para acessar o projeto basta clicar em:      [![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/surocham/ca_naruto)
---


### Análise Estratégica do Setor Vitivinícola Brasileiro
![image](https://github.com/user-attachments/assets/fabe2652-bbed-42e8-b0a6-7f3e14324880)

**Contexto:** Este projeto foi desenvolvido como parte do Tech Challenge da FIAP - Pós-Graduação em Data Analytics, apresentando uma análise estratégica do setor vitivinícola brasileiro com foco em competitividade internacional e oportunidades de crescimento.

**Objetivos:**
- Analisar a evolução dos preços médios de exportação por país de destino
- Calcular e interpretar a Taxa de Crescimento Anual Composta (CAGR) das exportações
- Determinar a correlação entre produção nacional e volume exportado
- Avaliar a taxa de utilização da capacidade produtiva para exportação
- Propor recomendações estratégicas baseadas em evidências

**Resultados:**
- Analisar a evolução dos preços médios de exportação por país de destino
- Calcular e interpretar a Taxa de Crescimento Anual Composta (CAGR) das exportações
- Determinar a correlação entre produção nacional e volume exportado
- Avaliar a taxa de utilização da capacidade produtiva para exportação
- Propor recomendações estratégicas baseadas em evidências

**Ferramentas e linguagens utilizadas:**
- Git
- Python
- Visual Studio Code

  #### Para acessar o projeto basta clicar em:      [![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/surocham/vinho_brasil_analytics)

---

Entre em contato comigo por meio de:  

[<img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">](https://www.linkedin.com/in/surocham/) 
[<img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">](mailto:suamirochati@gmail.com) 


© 2026 Suami Evelin Rocha de Medeiros. 

