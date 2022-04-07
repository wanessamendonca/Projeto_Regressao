# Previsão de Custos de Planos de Saúde a Partir de Características dos Clientes 


<img src = 'https://user-images.githubusercontent.com/92948655/162278169-c564dce0-dae4-4fe6-9c37-d43e3c35a16a.jpg' width = '400'>

*fonte da imagem [aqui](https://www.behance.net/collection/7427185/illustration).*


## Contexto e Objetivos do Projeto

Estima-se que no ano de 2019 o número de pessoas com acesso a planos de saúde nos Estados Unidos tenha chegado a uma marca próxima de 300 milhões, o que corresponde à 91,4% da população. Destes, cerca de 50,3% obtiveram acesso ao plano de saúde por meio do trabalho, enquanto 39,5%, dependiam de programas do governo, como Medicare e Medicaid, que cobrissem os custos do plano.

Tendo em vista a dependência que a população americana possui em relação ao custeamento de planos de saúde, uma vez que não há um sistema único de saúde gratuito como no Brasil, faz-se de extrema importância a previsão de valores de encargos de forma precisa e rápida, devido a alta demanda.

**Diante do cenário apresentado, este projeto possui como principal objetivo a previsão de custos individuais de plano de saúde em base anual a partir de características informadas por diferentes clientes, como idade, gênero e se são ou não fumantes, por exemplo. Diferentes algoritmos de regressão serão utilizados para o desenvolvimento das previsões.**

🎲 Os dados foram extraídos da plataforma Kaggle em 22 de março de 2022 e podem ser obtidos por meio deste [link](https://www.kaggle.com/datasets/mirichoi0218/insurance).

📑 Para maiores informações sobre o cenário da dependência da população em relação aos planos de saúde nos Estados Unidos, maiores informações podem ser consultadas [aqui](https://www.statista.com/topics/7807/health-insurance-in-the-us/#dossierContents__outerWrapper).


## Dicionário de Dados



<div style="width: 650px;"></div>
<img src = 'https://user-images.githubusercontent.com/92948655/162276668-dc530406-ce1c-4407-b4d9-2d81ecf00d44.png' width="650">


## Headlines

As principais conclusões obtidas ao final do desenvolvimento do presente projeto foram:

- A base de dados apresenta um certo desbalanceamento no que se refere ao número de clientes fumantes/não-fumantes e ao número de dependentes;


- Foi possível inferir também que a base de dados está bastante concentrada em clientes que pagam abaixo de 14 mil reais por ano em plano de saúde. Existe uma pequena parcela que desembolsa acima de 40 mil dólares;



- Entre os clientes que pagam abaixo e acima de 15 mil dólares, foi possível observar que estes grupos apresentam leves diferenças em relação ao índice de massa corporal e ao número de dependentes. Clientes que pagam menos encargos, tem entre 0 e 1 dependente e IMC em torno de 30 (sobrepeso), enquanto que, clientes cujos gastos são maiores, possuem entre 1 e 2 dependentes e IMC de aproximadamente 32 (obesidade grau I); 



- A depender da fonte dos dados, seria interessante que os casos de clientes que pagam valores mais altos tivessem um número mais expressivo na base, para que os algoritmos pudessem ser ainda mais enriquecidos de tal informação;


- O desempenho das diferentes técnicas de machine-learning utilizadas ao longo do projeto, não tiveram, de forma geral, um bom desempenho, podendo errar em média em até 6 mil dólares quando da previsão dos encargos. Este mau desempenho evidencia uma necessidade de talvez voltarmos para a etapa de coleta dos dados, tornando a base mais diversa ou pesquisando por novas *features*;


- Apesar do desempenho mediano, os algoritmos que melhor previram os encargos foram os menos complexos: regressão linear com dados padronizados e regressão linear com Lasso. O modelo de regressão linear com padronização dos dados conseguiu generalizar de forma eficiente para os dados contidos no conjunto de teste;


- A criação de novas *features* pode chegar a enriquecer o nível de informação dos modelos gerados, com métricas apontando para um ótimo desempenho. Porém, neste ponto cabe dizer que a inclusão de novas variáveis deve sempre observar a minimização do uso de *features* que estão fora do controle da pessoa-alvo do modelo.
