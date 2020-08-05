
Com o ConfigMap criado, vamos rodar nosso aplicação Doom que renderiza a intensidade e a direção da chama de acordo com o parametro do ConfigMap.
Desta vez o ConfigMap será usado para montar o arquivo em um pasta acessível para a aplicação.

Execute o comando abaixo para visualizar o Yaml da aplicação:

`cat doom.yaml`{{execute}}

Aplicando o YAML:

`kubectl apply -f doom.yaml`{{execute}}

Vamos checar se o Pod foi criado corretamente:

`kubectl get pods`{{execute}}

Com o Pod criado, vamos para o próximo passo...