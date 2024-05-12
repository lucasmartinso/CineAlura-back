# CineAlura-back

# API de Recomendação de Filmes e Séries e Consulta de Cinemas

Esta é uma API simples construída em Flask para recomendar filmes e séries com base em categorias/gêneros fornecidos pelo usuário e para consultar informações sobre cinemas com base na cidade e no CEP.

## Métodos

### 1. Recomendação de Filmes e Séries

Para obter recomendações de filmes e séries, você pode usar o endpoint `/api/filmes` com o método `GET`. Basta fornecer a categoria ou gênero do filme/série desejado como parâmetro na solicitação.

Exemplo de solicitação: "Ação" || "Aventura" || ...  -> informar gênero/tipo(input) 

A resposta será uma lista de filmes e séries recomendados na categoria especificada, juntamente com suas informações, como título, sinopse, disponibilidade em plataformas de streaming, avaliação dos usuários do Google e classificação do IMDb.

### 2. Consulta de Cinemas

Para consultar informações sobre cinemas em uma determinada cidade com base no CEP, você pode usar o endpoint `/api/cinemas` com o método `GET`. Basta fornecer a cidade e o CEP desejados como parâmetros na solicitação.

Exemplo de solicitação: CIDADE -> informar nome(input) e CEP -> informar conjunto de dígitos(input) 


A resposta será uma lista de cinemas na cidade especificada, juntamente com suas informações, como nome, distância aproximada em quilômetros e endereço.

## Execução

Para executar a API localmente, certifique-se de ter o Python, Flask e google-generativeai(e sua respectiva API KEY) instalados em seu ambiente. Em seguida, você pode iniciar o servidor Flask executando o seguinte comando:
```yml
python main.py
```


Isso iniciará o servidor na porta padrão 5000. Você pode acessar os endpoints da API usando um cliente HTTP ou um navegador da web.




