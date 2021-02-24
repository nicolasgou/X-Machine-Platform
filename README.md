# RESUMO
Este repositório tem como objetivo apresentar o estudo de arquitetura sistêmica proposta em projeto de pesquisa de inovação apresentado a FAPESP - Fundação de Amparo à Pesquisa do Estado de São Paulo.
Projeto de pesquisa técnico cientifica intitulado: Prototipação de Plataforma de Software para Análise, Diagnostico e Prognostico de Manutenção de Ativos Industriais Integrada com Modelos de Manutenção Preditiva.


# Inovação e P&D
FAPESP - Fundação de Amparo à Pesquisa do Estado de São Paulo 
PIPE - Programa Pesquisa Inovativa em Pequenas Empresas

Projeto de Pesquisa: 2º ciclo de 2019 
Título: Modelo Preditivo para Detecção de Falhas Iminentes em Máquinas Elétricas Industriais
Área de Pesquisa: Modelos de Inteligência Artificial (IA) e Aprendizado de Máquina (Machine Learning)

Estruturação de infraestrutura de recursos para pesquisa com aquisição de equipamentos, painéis e bancadas de maquinas e componentes essenciais pra montagem de um Laboratório de Pesquisas em Diagnostico e Prognostico de ativos Industriais, propondo ser uma instalação projetada para suportar o desenvolvimento, maturação e avaliação comparativa (benchmarking) de tecnologias de diagnóstico, prognóstico e decisão para aplicações de gerenciamento dos sistemas de “saúde” de ativos industriais assim como  validação dos modelos preditivos desenvolvidos.

Os Principais objetivos da pesquisa foi a consolidação de experimentos de hardware em loop para coletar dados para equipamentos exercidos em modos nominais e de falha e em diferentes condições de operação;
•Modelagem matemática em ambiente computacional de condições de falhas nos ativos e injeção desses modelos de falhas de forma repetível e padronizada. e performação/geração de data-sets run-to-fail a serem usados no treinamento dos algoritmos.
•Desenvolver bancada (testbed) de hardware em loop e infraestrutura de software de suporte que permite a modelagem matemática e computacional de falhas
•Pesquisa e formulação  de métricas apropriadas para benchmarking de algoritmos de diagnósticos e prognósticos de falhas.
•Desenvolver e avaliar metodologias de gerenciamento de incertezas que quantifiquem os efeitos das incertezas da solução sistêmica proposta, ambiente e de uso operacional.
•O Desenvolvimento e implementações de técnicas para tomada de decisão com base em informações de saúde.

•Treinamento de modelo classificador para detectar diferentes tipos de falhas, com objetivo de se obter uma visão sobre qual parte do equipamento requer atenção.


# Arquiteturas
O X-Machine Platform se compõem de componentes de software que são executados tanto em infraestrutura local quanto em nuvem.
O desenvolvimento em tecnologias de nuvem produtivas, híbridas, inteligentes e confiáveis, o X-Machine Platform é a combinação da experiência no mercado industrial com implementação de tecnologias, recursos e serviços computacionais no estado na arte da plataforma cloud Microsoft Azure, como Azure Machine Learning Service, Azure IoT Edge Run-Time System, Iot Hub, digital twin services, data factory, app services entre outro. O que nos permite oferecer uma plataforma adaptável, especializada e segura para a indústrias de processo como um todo.





# Sample Web Aplication Views



A coleta de um grande conjunto de dados de sensores representando diferentes condições de operações saudáveis e defeituosa. Assim como a coleta de dados em diferentes ambientes de operação, onde as máquinas que funcionam em lugares diferentes, uma pode falhar mais cedo que a outra devido a essas diferentes condições de operação. Capturar todos esses dados permitiu consolidação de um algoritmo robusto que pudesse detectar melhor falhas.
 
Em alguns casos, você pode não ter dados suficientes representando uma operação saudável e defeituosa. Sendo assim, uma das estratégias foi construir um modelo matemático do ativo e estimar seus parâmetros a partir de dados de sensores. Em seguida, simular este modelo com diferentes estados de falha em diferentes condições operacionais para gerar dados de falha data sets- run-to fail para treinamento dos modelos. 
 
Uma vez que se tenha os dados gerados complementando os dados de telemetria e você pode usar uma combinação de ambos para desenvolvimento do algoritmo/modelo. 



## Tecnologias
Gateway desenvolvido baseado em: Official OPC UA .Net Standard Samples from the OPC Foundation
Sample Servers and Clients, including all required controls, for .NET Framework 4.6.2, .NET Core 2.0 and UWP.

Consolidação de plataforma (web cloud Microsoft Azure) solução de software modular, tanto nos aspectos de arquitetura back-end quanto front-end do projeto de pesquisa.

•	Implementação de arquiteturas de microserviços de alta escalabilidade em nuvem;
•	Desenvolvimento em linguagem Python3, C#.net, ASP.NET, JavaScript;

Implementação e integração dos recursos e serviços de plataforma computacional em nuvem: Azure Machine Learning Service, Azure IoT Hub , Azure App Service, Azure Function Serverless, Azure Data Base Services e Azure Data Factory Service;


## TODO


## Authors

* **Nicolas Goulart** - *Initial work* - [NicolasGou](https://github.com/nicolasgou)
