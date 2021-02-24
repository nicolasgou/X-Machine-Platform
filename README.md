# RESUMO
Este repositório tem como objetivo apresentar o estudo de arquitetura sistêmica proposta em projeto de pesquisa de inovação apresentado a FAPESP - Fundação de Amparo à Pesquisa do Estado de São Paulo.
Projeto de pesquisa técnico cientifica intitulado: Prototipação de Plataforma de Software para Análise, Diagnostico e Prognostico de Manutenção de Ativos Industriais Integrada com Modelos de Manutenção Preditiva.
https://bv.fapesp.br/pt/auxilios/106269/modelo-preditivo-para-deteccao-de-falhas-iminentes-em-maquinas-eletricas-industriais/



# Inovação e P&D
FAPESP - Fundação de Amparo à Pesquisa do Estado de São Paulo 
PIPE - Programa Pesquisa Inovativa em Pequenas Empresas

Projeto de Pesquisa: 2º ciclo de 2019 
Título: Modelo Preditivo para Detecção de Falhas Iminentes em Máquinas Elétricas Industriais
Área de Pesquisa: Modelos de Inteligência Artificial (IA) e Aprendizado de Máquina (Machine Learning)

Estruturação de infraestrutura de recursos para pesquisa com aquisição de equipamentos, painéis e bancadas de maquinas e componentes essenciais pra montagem de um Laboratório de Pesquisas em Diagnostico e Prognostico de ativos Industriais, propondo ser uma instalação projetada para suportar o desenvolvimento, maturação e avaliação comparativa (benchmarking) de tecnologias de diagnóstico, prognóstico e decisão para aplicações de gerenciamento dos sistemas de “saúde” de ativos industriais assim como  validação dos modelos preditivos desenvolvidos.

Os Principais objetivos da pesquisa foram a consolidação de experimentos de hardware em loop para coletar dados para equipamentos exercidos em modos nominais e de falha e em diferentes condições de operação;

•Modelagem matemática em ambiente computacional de condições de falhas nos ativos e injeção desses modelos de falhas de forma repetível e padronizada. e performação/geração de data-sets run-to-fail a serem usados no treinamento dos algoritmos;

•Desenvolver bancada (testbed) de hardware em loop e infraestrutura de software de suporte que permite a modelagem matemática e computacional de falhas;

•Pesquisa e formulação  de métricas apropriadas para benchmarking de algoritmos de diagnósticos e prognósticos de falhas;

•Desenvolver e avaliar metodologias de gerenciamento de incertezas que quantifiquem os efeitos das incertezas da solução sistêmica proposta, ambiente e de uso operacional;

•O Desenvolvimento e implementações de técnicas para tomada de decisão com base em informações de saúde;

•Treinamento de modelo classificador para detectar diferentes tipos de falhas, com objetivo de se obter uma visão sobre qual parte do equipamento requer atenção;

![Lab de P D avancadas em sistemas P Indus](https://user-images.githubusercontent.com/45576249/109039573-b3070900-76ab-11eb-88ba-a98ae675c83a.png)

# Arquiteturas
O X-Machine Platform se compõem de componentes de software que são executados tanto em infraestrutura local quanto em nuvem.
O desenvolvimento em tecnologias de nuvem produtivas, híbridas, inteligentes e confiáveis, o X-Machine Platform é a combinação da experiência no mercado industrial com implementação de tecnologias, recursos e serviços computacionais no estado na arte da plataforma cloud Microsoft Azure, como Azure Machine Learning Service, Azure IoT Edge Run-Time System, Iot Hub, digital twin services, data factory, app services entre outro. O que nos permite oferecer uma plataforma adaptável, especializada e segura para a indústrias de processo como um todo.

![arquitetura_2](https://user-images.githubusercontent.com/45576249/109039603-bb5f4400-76ab-11eb-9888-bdc4cc751b5b.png)




# Sample Web Aplication Views
![MPDFIMEI_webapp](https://user-images.githubusercontent.com/45576249/109039638-c619d900-76ab-11eb-9dd9-cbac6f797d92.png)


A coleta de um grande conjunto de dados de sensores representando diferentes condições de operações saudáveis e defeituosa. Assim como a coleta de dados em diferentes ambientes de operação, onde as máquinas que funcionam em lugares diferentes, uma pode falhar mais cedo que a outra devido a essas diferentes condições de operação. Capturar todos esses dados permitiu consolidação de um algoritmo robusto que pudesse detectar melhor falhas.
 
Em alguns casos, você pode não ter dados suficientes representando uma operação saudável e defeituosa. Sendo assim, uma das estratégias foi construir um modelo matemático do ativo e estimar seus parâmetros a partir de dados de sensores. Em seguida, simular este modelo com diferentes estados de falha em diferentes condições operacionais para gerar dados de falha data sets- run-to fail para treinamento dos modelos. 
 
Uma vez que se tenha os dados gerados complementando os dados de telemetria e você pode usar uma combinação de ambos para desenvolvimento do algoritmo/modelo. 

![arcq_X-Machine-MMS](https://user-images.githubusercontent.com/45576249/109039584-b69a9000-76ab-11eb-9b59-6b77ba3e467e.png)

## Funcionalidades Sistemicas
Elaboração dos códigos fontes que atendam a demanda do escopo do projeto de pesquisa das funcionalidades:
•Monitoramento de condição do ativo em tempo real (status) – Desenvolvimento das funcionalidades de leitura de dados em banco de dados relacional e disponibilização das informações para apresentação nos painéis (Dashboards), performarão a geração dos gráficos de degradação do ativo (máquinas elétricas), e indicadores de análise de estado, além da performarem a geração de relatórios para visualização e análise dos usuários.

•Detecção De Falhas Análise e Diagnostico – Desenvolvimento das funcionalidades de detecção de falhas que podem ocorrer nos ativos, a detecção da natureza das falhas e performem recomendações de ações para solução das falhas detectadas;

•PROGNOSTICO DE FALHAS (RLU/TTF) – Desenvolvimento das funcionalidades de interação como os modelos preditivos e o processamento das informações de prognostico dos ativos para 
disponibilização das informações para apresentação através dos painéis interativos com o usuário da solução. Painéis os quais apresentarão a detecção de falhas previstas nos ativos, a natureza da falha prevista, indicadores de Tempo de Vida Útil Remanescente (RLU) ou Tempo até a Falha (TTL) e recomendações de mitigação para a falha prevista.

Consolidação de plataforma (web cloud Microsoft Azure) solução de software modular, tanto nos aspectos de arquitetura back-end quanto front-end do projeto de pesquisa.

•	Implementação de arquiteturas de microserviços de alta escalabilidade em nuvem;
•	Desenvolvimento em linguagem Python3, C#.net, ASP.NET, JavaScript;

Implementação e integração dos recursos e serviços de plataforma computacional em nuvem: Azure Machine Learning Service, Azure IoT Hub , Azure App Service, Azure Function Serverless, Azure Data Base Services e Azure Data Factory Service;


## TODO


## Authors

* **Nicolas Goulart** - *Initial work* - [NicolasGou](https://github.com/nicolasgou)
