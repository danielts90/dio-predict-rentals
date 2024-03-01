# dio-predict-rentals

A tarefa foi desenvolvida seguindo o passo a passo 
contido no [Microsoft Learn]( https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)

### 1  - Criação do Workspace na plataforma do Azure
   * Aqui foi explicado como criar um Workspaceno portal do Azure,
     vinculando-o com uma assinatura válida. 

### 2  - Uso do Azure Machine Learning Studio
  * Criação de um novo Automated ML job
  * Configuação do job
  * Importação dos dados de uma fonte na web. [link](https://aka.ms/bike-rentals)
  * Configurações dos parâmetros do job. 

### 3 - Revisão do Modelo
  * Acesso à aba de Overview
  * Seleção do algoritmo
  * Visualização das métricas

### 4 - Deploy do Modelo 
  * Configuração do deploy do modelo como Web Service

### 5 - Teste 
  * Para testes foi usado o Json

    ```json
    {
      "Inputs": {
        "data": [
          {
            "day": 1,
            "mnth": 1,
            "year": 2022,
            "season": 2,
            "holiday": 0,
            "weekday": 1,
            "workingday": 1,
            "weathersit": 2,
            "temp": 0.3,
            "atemp": 0.3,
            "hum": 0.3,
            "windspeed": 0.3
          }
        ]
      },
      "GlobalParameters": 1.0
    }
    ```

    Obtendo como resultado
    ```json
    {
      "Results": [ 342.48779440925205 ]
    }
    ```


