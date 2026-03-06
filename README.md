conteudo_readme = """Análise de Dados: Titanic Dataset
Desafio extra do curso treinamento Carreira Tech - Trilha Análise de Dados -
Introdução ao Data Science de dados do histórico.

O objetivo:
 * importação dos dados;
 * compreensão do conjunto de informações;
 * preparação e tratamento dos dados;
 * verificação e tratamento de valores nulos e duplicados;
 * ajustes de tipagem;
 * organização das colunas
 * agrupamento dos dados
 * visualização gráfica

Para essa atvidade foi utilizado o histórico de passageiros do Titanic, por meio
do arquivo com os dados do titanic.

-----------------------------------
Tecnologias utilizadas:
Python 3.12
Pandas para a manipulação e análise de dados
Seaborn/Matplotlib para a visualização de dados estatísticos

---------------------------------------

Detalhamento das etapas:

1. Importação e compreensão:

Os dados foram carregados a partir de um arquivo .CSV (titanic_dataset.csv).
Para uma visualização incial, foi utilizado o comando df.head() e df.info()
para visualizar os tipos de variáveis e valores nulos e campos vazios.


2. Tratamento e limpeza dos dados:

Verificação de dados Dduplicados com o comando df.duplicated() e a exclusãp com
df.drop_duplicates().

Tratamento de Nnlos:

Dados nulos no campo 'Age': os campo nulos foram substituidos pela média das
idades.

Coluna 'Cabin' com campos em branco: os campos em branco foram preenchidos com
a palavra "Desconhecida".

Dados numls no campo 'Embarked': Como havia apenas dois registros nulos, foi
realizada a remoção das linhas, pois o impacto no total de dados é mínimo.

3. Ajustes dos tipos e organização:

A coluna Age foi convertida de decimal  para inteiro, usando astype(int).

A ordenação dos dados pela coluna 'Sex' para facilitar a visualização de grupos
específicos.

---------------------------------------

Análise Eeploratória:

Agrupamento: o método groupby(['Sex'])['Survived'].sum() para consolidar o total
de sobreviventes por gênero.

A análise de agrupamento e a visualização gráfica mostram uma taxa de
sobrevivência significativamente maior entre o sexo feminino.

Visualização gráfica:

Foi gerado um gráfico de barras utilizando a biblioteca seaborn para representar
relação entre o sexo e o número de sobreviventes.

# Representação visual da sobrevivência por sexo
sns.barplot(data=df_por_sexo, x='sex', y='survived')
plt.show()

----------------------------------------
Como Executar o Projeto
Certifique-se de ter o Python e as bibliotecas Pandas, Seaborn e Matplotlib
instaladas.
Faça o upload do arquivo titanic_dataset.csv.
Execute o script de tratamento para gerar a base limpa e as visualizações.

--------------------------------------------------------------------------------
Projeto desenvolvido como parte do Desafio Extra de Data Analytics."""
