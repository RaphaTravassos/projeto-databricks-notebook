## DIO | Projeto: Controle e Versionamento de Código no Notebook da Azure 

![CrossingFinishLineNinoSchurterGIF](https://github.com/user-attachments/assets/7299acce-c3cb-435b-b0d7-b6ec901328c5)

## 🌏 Visão Geral

Processo de provisionamento, configuração e uso do Azure Databricks para análise de dados com Spark, com ênfase no controle de versão dentro dos notebooks.

## Objetivo do projeto: 
✅ Criar Cluster no Databricks.

✅ Criar Notebook no Dabricks.

✅ Importar arquivo CSV/dados através de URL, utilizando o panda.

✅ Criar filtro para análisar o arquivo.


## 🪤 Tecnologias Utilizadas

*  Azure Databricks
*  Jupyter Notebook
*  Python
*  Apache Spark (PySpark)

## 📚 Etapas do Projeto

## 1. Usar o Spark to Analyze data

Para efetuar o download do arquivo csv, através da ***'URL: https://raw.githubusercontent.com/MicrosoftLearning/mslearn-databricks/main/data/products.csv'***.

![image](https://github.com/user-attachments/assets/a5dc6b22-5f11-4b9b-87f0-0f3a6ca306ee)
![image](https://github.com/user-attachments/assets/278c2b9a-8a14-4478-8107-ab0c0e83b693)

---

## 2. Importar o arquivo utilizando Panda.

Este processo consiste em baixar o arquivo csv, para manipulação de dados e transformação dos dados.

![image](https://github.com/user-attachments/assets/a4d87bc0-8cee-419e-9f5b-28e2b7d07395)
![image](https://github.com/user-attachments/assets/51cf3fa2-61f2-42e9-8034-46b50a2d7df1)
![image](https://github.com/user-attachments/assets/f4af12f3-cc8c-4a26-86f6-5bbfdacfd143)

---

***Código de importação:***

import pandas as pd

url = 'https://raw.githubusercontent.com/MicrosoftLearning/mslearn-databricks/main/data/products.csv'

df = od,read_csv(url)

display(df)

***Dados gerados no Databricks após a importação do arquivo CSV.***

![image](https://github.com/user-attachments/assets/876f8f63-5ba4-4c67-ba05-76bf13fee852)

---

## 3. Modelagem e filtro dos dados.

Mostramos como é fácil aplicar filtros direto no Databricks para visualizar só uma categoria específica ou escolher quais colunas queremos analisar, tornando a exploração dos dados muito mais prática

![image](https://github.com/user-attachments/assets/e9728724-4be1-40c0-a878-f9c31a90a065)
![image](https://github.com/user-attachments/assets/8835e6dc-0391-4af6-96af-1a526f3b0f96)

---

***Código para fazer filtros:***
df_filtered = df[df['Category'] == 'Road Bikes']
display(df_filtered)
imagem abaixo mostra o filtro feito por Categoria para ‘Road Bikes e Touring Bikes’

----

## 4. Adicionando texto dentro do Notebook

No próprio notebook, podemos adicionar textos explicativos para deixar mais claro o que está sendo feito em cada etapa do processo. Para isso, basta posicionar o mouse dentro do notebook até aparecerem as opções 'Create' (que permite adicionar novos blocos de código) e 'Text'(onde podemos inserir comentários ou descrições). Assim, conseguimos documentar melhor cada passo, como mostrado nos exemplos abaixo.

![image](https://github.com/user-attachments/assets/91362497-192a-44d0-bf15-c4b745a941a0)
![image](https://github.com/user-attachments/assets/b852f46d-270e-4219-ae36-6391d8a6217c)
![image](https://github.com/user-attachments/assets/6e9e1f7b-446d-42f1-a021-c3e1853b91f2)

## 5. Exportação do arquivo Notebook

Exportado em formato `.ipynb` para importação futura e versionamento via GitHub.

![image](https://github.com/user-attachments/assets/751f54ea-580a-4690-a702-0af330aec707)
![image](https://github.com/user-attachments/assets/941bd12d-4711-4d52-b9b8-63133b7e6a3e)
![image](https://github.com/user-attachments/assets/72e36d8d-efeb-4848-94e2-3ef03f1a8649)


## 6. Importação de arquivo notebook Databricks

Importar arquivos para análise.

![image](https://github.com/user-attachments/assets/7c8f5b3f-8cfb-4499-b3b9-613b08ae4cf5)


## 💡 Insights

- O Azure Databricks oferece integração com recursos do Azure e é ideal para análise de dados.
- A criação e configuração de clusters pode ser feita de forma intuitiva via interface web.
- O controle de versões dos notebooks facilita o rastreio de alterações.
- O Spark permite lidar com grandes volumes de dados.
- 
## Possibilidades Futuras

- Integração com o GitHub diretamente nos notebooks Databricks.
- Automatização de pipelines.
- Uso de Delta Lake.
- Aplicação de modelos de Machine Learning.

## 💼 Autor

Raphael Travassos  - Projeto prático DIO para portfólio 🚀
