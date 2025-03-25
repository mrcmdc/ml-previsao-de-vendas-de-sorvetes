# ml-previsao-de-vendas-de-sorvetes

## Cenário
Imagine que você é proprietário de uma sorveteria chamada Gelato Mágico, localizada em uma cidade litorânea. Você percebe que a quantidade de sorvetes vendidos diariamente tem uma forte correlação com a temperatura ambiente. No entanto, sem um planejamento adequado, você pode acabar produzindo mais sorvetes do que o necessário e ter prejuízos com desperdícios ou, ao contrário, produzir menos e perder vendas.

Para solucionar esse problema, você decide usar Machine Learning para prever quantos sorvetes serão vendidos com base na temperatura. Com esse modelo, será possível antecipar a demanda e planejar a produção de maneira eficiente.

Agora é a sua hora de brilhar e construir um perfil de destaque na DIO! Explore todos os conceitos explorados até aqui e replique (ou melhore, porque não?) este projeto prático. Para isso, crie seu próprio repositório e aumente ainda mais seu portfólio de projetos no GitHub, o qual pode fazer toda diferença em suas entrevistas técnicas 😎

## Objetivo
O objetivo deste projeto é desenvolver um modelo de regressão preditiva que permita: 

- Treinar um modelo de Machine Learning para prever as vendas de sorvete com base na temperatura do dia.
- Registrar e gerenciar o modelo usando o MLflow.
- Implementar o modelo para previsões em tempo real em um ambiente de cloud computing.
- Criar um pipeline estruturado para treinar e testar o modelo, garantindo reprodutibilidade.

## Lab

Crie um workspace no Azure Machine Learning com as configurações abaixo e em seguida clique no botão "Review + create":

![image](https://github.com/user-attachments/assets/87b6a6e3-de71-4788-a159-54fd8610ec0c)


Será feita a validação do setup antes da criação de fato do workspace. Estando tudo certo basta clicar no botão "Create":

![image](https://github.com/user-attachments/assets/21806318-51f3-4c39-af58-3afe91349610)


Basta aguardar a implatanção do serviço:

![image](https://github.com/user-attachments/assets/b541c055-6d68-4bc7-b5b8-b9fa0313fe01)


Uma vez conclído agora é ir até os recursos criados clicando no botão "Go to resource" para ter acesso a tela principal do workspace criado:

![image](https://github.com/user-attachments/assets/b74b1341-5a43-4cdb-a713-b70d2ed710e7)
![image](https://github.com/user-attachments/assets/f3ae2a66-e389-4acc-80ae-221a73f2a7d2)


Após clicar no botão "Launch studio" o sistema apresenta o Machine Learning Studio uma plataforma de desenvolvimento visual e colaborativo fornecida pela Microsoft como parte do Azure Machine Learning. Ele permite que usuários criem, treinem e implantem modelos de machine learning sem precisar escrever código manualmente (ou com suporte a código, dependendo da versão):

![image](https://github.com/user-attachments/assets/fc26999f-c1f1-4518-afea-9600f5f77443)


Ao clicar em "Notebooks" é preciso adicionar os arquivos com dados que farão parte do aprendizado:

![image](https://github.com/user-attachments/assets/ee8daa26-44db-453b-af25-d1483b7fb85a)

É possível adicionar arquivos ou até mesmo pastas. No Lab será feita a importação de uma pasta contendo um arquivo com dados relacionados a vendas de sorvetes e temperatura no dia /inputs/ml-sorvetes-temp/dados-sovertes-temp.txt:

![image](https://github.com/user-attachments/assets/10dca56f-924b-4d3b-987d-9ce1e730e15f)


Crie um notebook na pasta importada:

![image](https://github.com/user-attachments/assets/ab37e8e1-5280-4460-bccd-34b8c7f0af75)


Agora é preciso criar uma instância de computador:

![image](https://github.com/user-attachments/assets/237224d9-0468-4d29-ab98-210157492e21)

![image](https://github.com/user-attachments/assets/4f4f5ab0-9d02-44af-846d-a094d4d79e53)

![image](https://github.com/user-attachments/assets/a7fc1be9-5ddc-4d5e-9c7b-2f2d81de73e8)

![image](https://github.com/user-attachments/assets/e51bce03-69d0-4f58-b963-0d242e9f0823)


Para esse lab será utilizado também um cluster de computador:

![image](https://github.com/user-attachments/assets/e4ccaec0-b75c-4a01-a039-854badb5b89c)

![image](https://github.com/user-attachments/assets/b78f42fb-f72b-420e-a756-ce5a00ef9b89)

![image](https://github.com/user-attachments/assets/f6f7cf7e-fbd7-4716-9bb4-5d3e1a7b3c23)


Agora será feita a configuração dos dados:

![image](https://github.com/user-attachments/assets/a94251ba-1e18-48de-9f25-990f2f26be71)


Clicar em Data assets:

![image](https://github.com/user-attachments/assets/7c4c6ff3-ade8-43ca-ad0c-525728731b1f)

![image](https://github.com/user-attachments/assets/e229df1e-ddb2-4b0e-a6ae-107451b51ab4)

![image](https://github.com/user-attachments/assets/0483931c-469c-49c1-ab9c-b69c7a5624f5)

![image](https://github.com/user-attachments/assets/ce41ab15-6400-4acc-ae5d-ccfb8c1cd007)

![image](https://github.com/user-attachments/assets/ea4a4c34-b2d6-4627-aa38-997c1c042e09)

![image](https://github.com/user-attachments/assets/9111ca47-15a8-43e6-b40a-7a4b75ae89a0)

![image](https://github.com/user-attachments/assets/460b6237-0657-44a0-9131-5e0f1dd51e4a)

![image](https://github.com/user-attachments/assets/62f1dc55-783c-4e6f-8fd2-7cf492222a03)


Após clicar no botão "Create" esse será o resultado:

![image](https://github.com/user-attachments/assets/ab3541d6-8bd2-4801-8d68-2e6a2ffbaabd)


Agora o trabalho segue configurando um AutoML:

![image](https://github.com/user-attachments/assets/13fe1a0b-a543-46dd-a327-add7d7daf496)

![image](https://github.com/user-attachments/assets/b24a6574-74da-42b2-b429-3eb6ec682154)

![image](https://github.com/user-attachments/assets/91b682fd-1024-4721-8d97-1c3bbeb65d68)

![image](https://github.com/user-attachments/assets/2c48d7f6-9393-4dbc-b3f8-80b966ff8b77)

![image](https://github.com/user-attachments/assets/c1976d07-ec4c-4593-b07f-08848905b4e3)

![image](https://github.com/user-attachments/assets/b408a49c-f36c-43b3-9f98-5be87971c085)


É possível usar um modelo específico. A seguir é feita a configuração do modelo XGBoostRegressor:

![image](https://github.com/user-attachments/assets/5a4ddbe1-1ed7-4adf-8c16-f20f01f06568)

![image](https://github.com/user-attachments/assets/967b3876-2c6a-462f-b1e9-e94e1eced2f2)

![image](https://github.com/user-attachments/assets/cf2912ac-66ab-4117-ac45-cb51e33ed9c8)

![image](https://github.com/user-attachments/assets/314b6516-300a-4af9-a176-1a21406183e0)

![image](https://github.com/user-attachments/assets/6401afc2-2b6c-4d57-8f4f-cdc6a8136f15)

![image](https://github.com/user-attachments/assets/4d9f3120-353a-4d13-a144-1606b11d530c)



## Criando um Novo Pipeline

Depois de clicar me "Create a new pipeline..." é hora de configurar: 
"

![image](https://github.com/user-attachments/assets/acc612e4-1bf4-485d-a53e-7d6126ce6734)


Arraste o data asset para o frame de desgin:

![image](https://github.com/user-attachments/assets/320c2512-9b7e-4800-982c-963865771b9c)


Adicione um componete:

![image](https://github.com/user-attachments/assets/f3600430-6192-41eb-b674-7f4a2a5facc2)


Selecione os campos:

![image](https://github.com/user-attachments/assets/0cc63d1e-cebc-401b-adf2-ff2f944f3695)


Configure o Split Data:

![image](https://github.com/user-attachments/assets/01b25fc7-ff1a-4dab-8170-f0a0b83584be)


Adicione um train model:

![image](https://github.com/user-attachments/assets/a3dbf1c0-9763-4e68-b3a9-9c053d282f4a)


Adicione e configure um "Linear Regression":

![image](https://github.com/user-attachments/assets/6b48ad27-a7d4-4bcb-9441-5592d3fbf309)


Após clicar em "Configure e Submit" 

![image](https://github.com/user-attachments/assets/e0e85b03-17d6-46b9-9685-7f1017d882f5)


Para verificar em Jobs o pipeline deve aparecer:

![image](https://github.com/user-attachments/assets/cdeea50b-f65b-4b95-8f42-de6ae699b8b7)

















