Descrição dos Contextos Limitados (Bounded Contexts)

1. Scraping Context
   Responsabilidade: Extrair dados das páginas web.

Componentes:

Entidades:
ScrapingTask: Representa uma tarefa de scraping, incluindo a URL da página e o estado da tarefa.
ScrapedData: Representa os dados extraídos de uma página web.
Serviços de Domínio:
ScraperService: Responsável por realizar a tarefa de scraping e extrair dados.
Casos de Uso:
ScrapePage: Caso de uso para realizar scraping de uma página específica.
Interfaces:
ScrapeController: Controlador para lidar com solicitações de scraping.
ScraperGateway: Gateway para comunicação com o serviço de scraping.
Infraestrutura:
ScraperInfrastructure: Implementações de infraestrutura específicas para scraping. 2. Event Management Context
Responsabilidade: Gerenciar e armazenar eventos.

Componentes:

Entidades:
Event: Representa um evento ocorrido no sistema, como a conclusão de uma tarefa de scraping.
Serviços de Domínio:
EventStoreService: Responsável por armazenar eventos no Event Store.
EventPublisherService: Responsável por publicar eventos no Kafka.
Casos de Uso:
StoreEvent: Caso de uso para armazenar eventos no sistema.
Interfaces:
EventController: Controlador para lidar com eventos.
EventGateway: Gateway para comunicação com o Event Store.
Infraestrutura:
EventInfrastructure: Implementações de infraestrutura específicas para gerenciamento de eventos. 3. Data Processing Context
Responsabilidade: Processar e indexar dados extraídos.

Componentes:

Entidades:
ProcessedData: Representa os dados que foram processados e estão prontos para serem indexados.
Serviços de Domínio:
DataProcessorService: Responsável por processar os dados extraídos.
IndexService: Responsável por indexar os dados no Elasticsearch.
Casos de Uso:
ProcessData: Caso de uso para processar dados extraídos.
Interfaces:
DataProcessingController: Controlador para lidar com o processamento de dados.
DataProcessingGateway: Gateway para comunicação com o serviço de processamento de dados.
Infraestrutura:
DataProcessingInfrastructure: Implementações de infraestrutura específicas para processamento de dados. 4. Query Context
Responsabilidade: Consultar e recuperar dados.

Componentes:

Entidades:
Query: Representa uma consulta realizada pelo usuário.
QueryResult: Representa o resultado de uma consulta.
Serviços de Domínio:
QueryService: Responsável por executar consultas no Elasticsearch.
Casos de Uso:
ExecuteQuery: Caso de uso para executar consultas.
Interfaces:
QueryController: Controlador para lidar com consultas.
QueryGateway: Gateway para comunicação com o serviço de consultas.
Infraestrutura:
QueryInfrastructure: Implementações de infraestrutura específicas para consultas.
