# Machine Learning - Previsão de Aluguel de Bikes (Azure)

Este repositório documenta minha experiência com o curso de **Machine Learning** da DIO, onde utilizei o **Azure Machine Learning** para prever o aluguel de bicicletas em uma empresa, utilizando dados históricos. O modelo foi treinado utilizando **Regression**.

---

## Sobre o Projeto

Neste projeto, utilizei o recurso de **Automated ML** do Azure para prever o aluguel de bicicletas com base em dados históricos de uma empresa. O objetivo é construir um modelo de **regressão** para prever o número de bicicletas que serão alugadas em um determinado período de tempo, utilizando dados de fatores como clima, dia da semana, e outros parâmetros.

---

## Etapas do Processo

1. **Criação do Recurso no Azure**  
   O primeiro passo foi criar o recurso no portal do Azure para utilizar o serviço de **Machine Learning**.
   ![Criar recurso](prints/1.jpg)
   
3. **Criação do Workspace**  
   Dentro do portal do Azure, criei um **Workspace** para organizar e gerenciar todos os recursos e experimentos relacionados ao modelo de Machine Learning.
   ![Criar workspace](prints/2.jpg)
   
4. **Acesso ao Automated ML**  
   No **Workspace**, entrei na seção de **Automated ML** e selecionei a tarefa de **regressão** para a previsão do aluguel de bikes e cliquei em CREATE para adicionar a base de dados historica.
   ![Clicar em automated ML](prints/3.jpg)
   ![Escolher Regressao](prints/5.jpg)
   
5. **Upload de Dados**  
   Para essa etapa, escolhi o **Azure Blob Storage** como a origem dos dados. Carreguei os dados históricos de aluguel de bicicletas no Blob Storage para treinamento do modelo.
   ![Tipo Tabluar](prints/6.jpg)
   ![From local files](prints/7.jpg)
   ![BlobStorage](prints/8.jpg)

6. **Ajuste dos dados**  
   Ajustei as configurações da tabela dos dados:
   ![Ajuste tabela](prints/10.jpg)

7. **Ajuste da tarefa**  
   Ajustei as configurações da tarefa:
   ![Ajuste tarefa](prints/12.jpg)
   ![Ajuste tarefa](prints/13.jpg)
      
8. **Treinamento do Modelo**  
   Após configurar, cliquei em **Create** para iniciar o treinamento do modelo. O **Azure Machine Learning** automaticamente ajustou os parâmetros e começou a treinar o modelo.
![Completado](prints/14.jpg)

9. **Registro do Modelo**  
   Após o treinamento ser concluído, cliquei em **+ Register Model** para registrar o modelo gerado e torná-lo disponível para implantação e ajustei algunmas informacoes.
![Ajuste model](prints/15.jpg)

10. **Acesso ao Modelo em Models**  
   Fui até a seção de **Models** para verificar o modelo registrado.
![Models](prints/16.jpg)

11. **Implantação do Modelo - Real-Time Endpoint**  
   Cliquei em **Deploy**, escolhi a opção de **Real-Time Endpoint** para configurar o modelo para previsões em tempo real. Ajustei as configurações de implantação conforme necessário.
![Deploy](prints/17.jpg)
![Ajuste endpoint](prints/18.jpg)

12. **Visualização do Endpoint**  
    Por fim, fui até **Endpoints**, onde cliquei no item de endpoint recém-criado para visualizar e utilizar o modelo para previsões.
![Endpoint](prints/19.jpg)
![Succeed](prints/20.jpg)

---

## Resultados

O modelo de regressão foi treinado com os dados históricos da empresa, e agora é possível realizar previsões em tempo real sobre o aluguel de bicicletas. O processo foi totalmente automatizado através do **Azure Machine Learning**, desde a criação do workspace até a implantação do modelo como endpoint.

Este projeto demonstrou como usar o **Azure ML** para realizar tarefas de Machine Learning de forma eficiente, mesmo para aqueles que não possuem experiência profunda em tuning de modelos, já que a ferramenta automatiza grande parte do processo.

---

## Tecnologias Utilizadas

- **Microsoft Azure**: Plataforma de computação em nuvem utilizada para hospedar o projeto.
- **Azure Machine Learning**: Serviço de Machine Learning para automação do treinamento e implantação de modelos.
  
---

## Conclusão

Este projeto foi uma excelente oportunidade para aprender sobre o uso de **Machine Learning** no Azure, com foco em **regressão** para previsão de aluguéis de bicicletas. Através da interface de **Automated ML**, consegui configurar e treinar um modelo de forma rápida e eficiente, sem a necessidade de configurações manuais complicadas.

Agora, com o modelo implantado como um **Real-Time Endpoint**, posso realizar previsões instantâneas sobre o aluguel de bicicletas, o que facilita a tomada de decisões para a empresa.
