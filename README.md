# Teste Android

Esse é um simples app que usa a NewsAPI (https://newsapi.org)

Ele usa a arquitetura MVVM, Retrofit, Koin (para injeção de dependência) e RxAndroid.


## Desafios

O App precisa de várias melhorias, mas no momento estamos com um problema sério onde nem conseguimos abrir o app. A primeira coisa a fazer é corrigir os erros para o app funcionar corretamente.
Nossa chave do NewsAPI expirou, é preciso gerar uma nova chave e trocar ela (no arquivo Constants.kt) para o app funcionar corretamente, para gerar a nova chave (gere a individual, que não tem custos) e também ter informações sobre o funcionamento da API visite: https://newsapi.org

Além do app funcionar corretamente temos alguns desafios extras, não são todos obrigatórios mas tudo que for feito será avaliado.

Os próximos desafios são:
 - O App usa a arquitetura MVVM, mas a nova parte que lista as notícias não está muito legal. Precisamos rever a arquitetura dessa parte e deixar no padrão do projeto (a parte que lista os Sources).
 - A listagem de notícias não está paginada e traz apenas as primeiras notícias. Precisamos paginar ela para trazer todas as informações disponíveis.
 - Alguns testes estão quebrando, verificar a sessão de testes abaixo para saber como executar os testes e corrigir o que for necessário.
 - A nova parte de notícias está sem cobertura de testes unitários e UI. Criar os testes para melhorar a cobertura.
 - Você é livre para fazer outras melhorias que ache necessário.

Faça um pequeno resumo de quais desafios e melhorias foram feitos.

Qualquer dúvida entre em contato.


## Testes

Para executar os testes unitários com cobertura:

    ./gradlew jacocoTestDebugUnitTestReport


Para executar os testes instrumentados:

    ./gradlew connectedDebugAndroidTest
    
Todos os dados dos testes estão mockados.