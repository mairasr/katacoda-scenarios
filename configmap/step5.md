
Com o ConfigMap criado, vamos rodar nosso aplicação Doom que renderiza a intensidade e a direção da chama de acordo com o parametro do ConfigMap.
Desta vez o ConfigMap será usado para montar o arquivo em um pasta acessível para a aplicação.

Execute o comando abaixo para visualizar o Yaml da aplicação:

`cat doom.yaml`{{execute}}

Aplicando o YAML:

`kubectl apply -f doom.yaml`{{execute}}

Vamos checar se o Pod foi criado corretamente:

`kubectl get pods`{{execute}}

Com o Pod criado, vamos para o próximo passo...

Para ver o resultado, precisamos que o EXTERNAL IP do serviço esteja preenchido, por isso execute o comando abaixo para rerificar:

`kubectl get services`{{execute}}

Caso esteja <PENDING>, só aguardar e checar novamente com o mesmo comando até que apareça um IP, isso pode levar alguns minutos.
