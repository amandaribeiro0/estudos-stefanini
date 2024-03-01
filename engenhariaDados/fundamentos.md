#  Fundamentos da Engenharia de Dados -  Data Science Academy

#### O que é engenharia de dados?
Um conjunto de tecnicas, etapas, conjuntos, processos, procedimentos que permitem que dados brutos se tornem dados utilizaveis(informação).
A engenharia de dados ajuda a tornar os dados mais úteis e acessíveis para os consumidores de dados.

#### O que é Pipeline de Dados?
Um pipeline de dados é um meio de mover dados de um locas (a origem) para o destino (um Data Warehouse ou Data Lake por exemplo).
Ao longo do caminho os dados são transformados e otimizados

Um pipeline de dados é uma série de etapas de processamento de dados.

- <b > Componentes de um pipeline </b>
      - Origem
      - Processamento 
      - Destino
  
Os pipelines de dados modernos tornam a extração de informações dos dados coletados rápida e eficiente.

- <b> Principais características: </b>
      - Processamento de dados contínuo e extensível
      - A elasticidade e agilidade da nuvem
      - Recursos isolados  e independentes para processamento de dados
      - Acesso democratizado a dados e gerenciamento de autoatendimento
      - Alta disponibilidade e recuperação de desastres
  
- <b> Composição de uma pipeline </b>
    - Origem: A maior parte das pipwlines puxa dados brutos de múltiplas fontes;
    - Destino: Os dados podem ser direcionados para um storage, ou diretamente para uma aplicação;
    - Transformação: Operações que modificam os dados, incluindo padronização, ordenação, duplicação, validação ou verificação. Todas as transformações necessárias para deixar os dados "limpos" e prontos para análise;
    - Dataflow: Movimento dos dados da origem até o destino, incluindo as transformações que serão aplicadas sobre eles e silos de dados pelos quais vão passar. Uma das abordagens possíveis para esse fluxo é a ETL;
              ETL: extract, transform, load.
    - Processamento: Apesar de ser relacionado com o Dataflow, o processamento pode variar de acordo com o volume de dados e a velocidade com que se pretende processar os mesmos;
    - Storage: Compartimentos quais os dados serão armazenados ao longo da pipeline. O tipo de storage depende de alguns fatores como volume de dados, tipos de dados, frequência de query, etc;
    - Workflow: Se refere ao sequenciamento de dependências dos processos. Gerenciar o agendamento, execução, distribuição e outras relações durante a pipeline. Entra no workflow os conceitos de upstream e downstream jobs;
    - Monitoramento: Pipelines precisam ser monitoradas de perto para garantir a integridade dos dados.


#### ETL 
Extração, Transformação e Carga. 
É um processo utilizado para transferir dados de diferentes fontes, convertê-los em um formato adequado e carregá-los em um sistema de destino. O objetido do ETL é fornecer dados de qualidade prontos para análise.

Cada etapa de ETL:

- <b> Extração </b>
Essa etapa envolve a obtenção de dados de diversas fontes. Essa etapa pode ser complexa pois os dados podem estar armazenados em diferentes sistemas, com estruturas diferentes e até mesmo em formatos não estruturados.

- <b> Transformação </b>
Após os dados serem extraídos, é preciso transformalos em um formato e estrutura consistentes. Isso pode incluir a limpeza dos dados,  a padrozinação de valores a normalização dos dados, aplicação de regra de negócio e etc. A etapa da transformação garante que os dados estejam coerentes e prontos para uma análise.

- <b> Carga </b>
Etapa final do processo de ETL, é a carga dos dados transformados em um sistema de destino. Pode ser realizada de maneira incremental, ou de maneira completa. Pode envolver a criação de estruturas necessárias para a análise de dados.