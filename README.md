# Jogos Olímpicos de Verão

**Fonte dos Dados:** [Historical Data from the Olympics](https://basedosdados.org/dataset/62f8cb83-ac37-48be-874b-b94dd92d3e2b?table=567b1ccd-d8c2-4616-bacb-cf5c0e7b8d89)

## Introdução

A base de dados contém informações sobre os Jogos Olímpicos ocorridos entre 1986 e 2022, sendo composta por sete tabelas, conforme relacionado abaixo.

* \_Athlete Bio\_: cada linha representa um atleta suas informações, tais como nome, sexo, data de nascimento, país, entre outras;
* \_Athlete Event Result\_: cada linha apresenta um evento ou esporte olímpico específico, acompanhado pelo atleta participante e os resultados (ranking) alcançados;
* \_Game Medal Tally\_: cada linha corresponde a um país em uma edição dos Jogos Olímpicos, indicando o total de medalhas conquistadas, bem como a quantidade separada por tipo: bronze, prata e ouro
* \_Country\_: lista de países que participaram dos jogos;
* \_Result\_: detalhamento dos resultados de um evento esportivo específico nos Jogos Olímpicos;
* \_Game\_: lista de todas as edições dos jogos olímpicos (inverno e verão).

Nesta análise, optou-se por incluir apenas os jogos olímpicos de verão.

Por meio de dashboard no Power BI, buscou-se apresentar informações gerais como total de atletas participantes, quantidade de medalhas conquistadas, países onde ocorreram mais edições do jogos, assim como uma comparativo entre os gêneros dos atletas, um ranking dos países participantes e dos atletas. 

## Criação das Consultas no BigQuery

Primeiramente, foram realizadas consultas no BigQuery para cada uma das tabelas, selecionando todas as colunas e filtrando apenas as edições dos jogos olímpicos de verão. A visualização das consultas foram salvas, para que posteriormente pudessem ser acessadas no Power BI.

**Athlete Bio**
![image](https://github.com/user-attachments/assets/cb0a04c4-67ea-42bc-9659-ed0751e872c8)

**Athlete Event Result** 
![image](https://github.com/user-attachments/assets/4965c03e-3e99-4e97-bf04-78eeac58f97c)

**Game Medal Tally**
![image](https://github.com/user-attachments/assets/10e083ce-6b5e-4b7f-be43-df77de17f883)

**Country**
![image](https://github.com/user-attachments/assets/ec9add48-dce4-4472-b43c-3a2d5c97a261)

**Result**
![image](https://github.com/user-attachments/assets/35a096ef-ceab-4318-9c54-d7ca0628b8c1)

**Game**
![image](https://github.com/user-attachments/assets/60480757-cb52-413f-b4ee-503b6734d73d)

## Importação dos Dados no Power BI

As tabelas foram carregadas no PowerBI por meio da opção Obter Dados - Google Big Query. Após selecionar as tabelas para importação e selecionar "Transformar Dados", é exibida a opção de Importar (trazer uma cópia dos dados para o Power BI) ou Direct Query (conexão em tempo real com a fonte de dados). Na presente análise, entende-se que não existe necessidade de conexão em tempo real, então optou-se por apenas importar.

![image](https://github.com/user-attachments/assets/912a6769-9c91-4f7c-bee6-bb6fbde778f1)

## Análise

 - **Acesse o Dashboard completo**
[aqui](https://app.powerbi.com/view?r=eyJrIjoiOTk4ZDhiNjQtNmZiOC00MTEyLWFhMmQtZDczYzAzMjY1MTUxIiwidCI6ImIyOTIxMzJhLWQ2YzgtNGMyMi1hZmM4LWFhNmI5NWIwMzM5MSJ9&pageName=c6ec69d3905c501c6eb9)

## Fatos interessantes que descobri com esse dashboard
- Olímpiadas não foram disputadas durante a guerra mundial (acho que primeira)
- Estados Unidos boicotou as olímpiadas de 1980 (Moscow) por razões políticas (presidentes Jimmy Carter)
