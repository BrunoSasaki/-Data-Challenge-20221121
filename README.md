# Data-Challenge-20221121
Resolução do desafio para a vaga de Data Analyst 

Carreguei toda a informação dos dados para fazer análises exploratórias utilizando o método pd.read_csv do pandas e o info() para ver os tipos de dados. 

Para filtrar e manipular dados foi utilizado o Google Colab e Biblioteca Pandas.

1- Top 10 atores/atrizes considerando todos os dados;

Para rankear os Top 10 atores/atrizes considerando todos os dados, você precisa contar o número de vezes que cada ator/atriz aparece nos dados. O método utilizado foi o value_counts() para contar o número de vezes que cada ator/atriz aparece na coluna "cast". Em seguida, ele usa o método head() para obter os 10 atores/atrizes com mais ocorrências. Finalmente, ele imprime os resultados na tela.


2- Top 5 países produtores de conteúdos considerando todos os dados e comparando as duas plataformas;

Para rankear os Top 5 países produtores de conteúdo considerando todos os dados e comparando as duas plataformas, você pode usar a biblioteca pandas do Python para carregar os dados dos dois arquivos CSV em dois objetos DataFrame separados e, em seguida, concatenar os dois dataframes em um único dataframe com todas as informações. Em seguida, você pode usar o método groupby() para agrupar os dados por país e contar o número de ocorrências de cada país. Finalmente, você pode classificar os países em ordem decrescente e imprimir os Top 5.

3- Mês no qual há mais adições de filmes na plataforma Netflix;

Para obter o mês com mais adições de filmes na plataforma Netflix, você pode usar a biblioteca pandas do Python para carregar os dados do arquivo CSV em um objeto DataFrame e, em seguida, extrair a informação de mês da coluna "date added".

4- Quantidade de filmes listados como comédia.

Para obter a quantidade de filmes listados como comédia na plataforma Netflix, você pode usar a biblioteca pandas do Python para carregar os dados do arquivo CSV em um objeto DataFrame e, em seguida, filtrar as linhas que contêm o gênero "Comedy". Utilizei o método str.contains() para filtrar as linhas que contêm a string "Comedy" na coluna "listed_in", que lista os gêneros de cada filme. O argumento na=False é usado para tratar valores faltantes como strings vazias. Em seguida, ele usa o método shape[0] para contar o número de linhas filtradas. Finalmente, ele imprime o resultado na tela.

5- Lista de todos os gêneros de filmes.

Para obter a lista de todos os gêneros de filmes na plataforma Netflix, você pode usar a biblioteca pandas do Python para carregar os dados do arquivo CSV em um objeto DataFrame e, em seguida, extrair os valores únicos da coluna "listed_in". Este código carrega os dados do arquivo CSV "netflix.csv" em um objeto DataFrame chamado df. Em seguida, ele cria um conjunto vazio chamado genres para armazenar os gêneros de filmes únicos. Ele percorre cada string de gêneros na coluna "listed_in" e usa o método split() para separar a string em uma lista de gêneros individuais. Em seguida, ele percorre cada gênero na lista e usa o método strip() para remover espaços em branco adicionais. Ele adiciona cada gênero único ao conjunto genres. Finalmente, ele usa o método sorted() para ordenar a lista de gêneros em ordem alfabética e imprime cada gênero na tela. Observe que, se houver valores faltantes ou com formatos diferentes na coluna "listed_in", o método split() pode gerar erros. Nesse caso, você precisará realizar algum pré-processamento nos dados para tratá-los antes de fazer a separação em uma lista.

6- A frequência de "TV Show" de todos os dados e comparativamente em relação as duas plataformas

Para obter a frequência de "TV Show" de todos os dados na plataforma Netflix e na Amazon Prime Video, você pode usar a biblioteca pandas do Python para carregar os dados dos arquivos CSV em objetos DataFrame e, em seguida, contar o número de ocorrências da string "TV Show" na coluna "type". Este código carrega os dados dos arquivos CSV "netflix.csv" e "amazon.csv" em objetos DataFrame chamados df_netflix e df_amazon, respectivamente. Em seguida, ele usa o método shape[0] para contar o número de linhas que contêm a string "TV Show" na coluna "type" de cada DataFrame. Ele armazena a frequência de "TV Show" na Netflix na variável netflix_tv_shows e a frequência de "TV Show" na Amazon na variável amazon_tv_shows. Finalmente, ele imprime os resultados na tela.
Observe que este código assume que os arquivos CSV têm uma coluna chamada "type" que indica se cada título é um filme ou uma série de TV.

7- A frequência de "Movies" de todos os dados e comparativamente em relação as duas plataformas

Para obter a frequência de "Movies" de todos os dados na plataforma Netflix e na Amazon Prime Video, você pode usar a biblioteca pandas do Python para carregar os dados dos arquivos CSV em objetos DataFrame e, em seguida, contar o número de ocorrências da string "Movie" na coluna "type". Este código carrega os dados dos arquivos CSV "netflix.csv" e "amazon.csv" em objetos DataFrame chamados df_netflix e df_amazon, respectivamente. Em seguida, ele usa o método shape[0] para contar o número de linhas que contêm a string "Movie" na coluna "type" de cada DataFrame. Ele armazena a frequência de "Movie" na Netflix na variável netflix_movies e a frequência de "Movie" na Amazon na variável amazon_movies. Finalmente, ele imprime os resultados na tela.
