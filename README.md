
# Projeto: Criando e Explorando um Índice de Pesquisa com Azure AI Search

Este README documenta o processo que realizei para configurar e explorar um índice de pesquisa utilizando o **Azure AI Search**. A atividade incluiu a configuração de recursos no Azure, o upload de documentos, a criação de um índice enriquecido com habilidades de IA e consultas no índice para obter insights úteis.

---

## Passos Realizados

### 1. Configuração dos Recursos no Azure
- Acessei o portal do Azure e criei os seguintes recursos:
  - **Azure Cognitive Search**: Para gerenciar o índice de pesquisa.
  - **Azure AI Services**: Para aplicar habilidades cognitivas.
  - **Azure Storage Account**: Para armazenar os documentos que seriam processados.
- Configurei a conta de armazenamento com um contêiner de blob chamado `knowledge-container`, onde os documentos seriam carregados.

### 2. Upload de Documentos
- Fiz o upload dos documentos fornecidos para o contêiner de blob `knowledge-container` na conta de armazenamento criada.
- Confirmei que os documentos estavam disponíveis no contêiner antes de prosseguir para a criação do índice.

### 3. Criação e Configuração do Índice
- No portal do Azure Cognitive Search, configurei um **data source** apontando para o contêiner de blob.
- Configurei uma **skillset** para enriquecer os dados, incluindo:
  - Extração de frases-chave.
  - Detecção de linguagem.
  - Extração de entidades nominais.
- Criei um **indexer** que utilizou as habilidades configuradas para processar os documentos e criar um índice de pesquisa.
- Validei que o índice foi criado com sucesso e estava pronto para consultas.

### 4. Consultando o Índice
- No portal do Azure Cognitive Search, utilizei a ferramenta de **Search Explorer** para realizar consultas no índice.
- Testei diferentes consultas para verificar:
  - Frases-chave extraídas dos documentos.
  - Detecção de idiomas nos textos.
  - Informações enriquecidas a partir das habilidades cognitivas.

---

## Resultados Obtidos
- Configurei com sucesso um índice funcional no Azure Cognitive Search.
- Apliquei habilidades de IA para enriquecer os dados armazenados.
- Realizei consultas no índice que retornaram informações detalhadas, como frases-chave, idiomas detectados e entidades extraídas.

---

## Observações Finais
Todo o processo foi concluído conforme o tutorial. Os resultados atenderam às expectativas, e o índice de pesquisa configurado provou ser eficaz para acessar informações de forma rápida e enriquecida.

Para detalhes adicionais sobre o laboratório, acesse:  
[Explorar um Índice de Pesquisa com Azure AI Search](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)
