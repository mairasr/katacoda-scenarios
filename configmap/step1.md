
Nosso primeiro exercicio será criar um ConfigMap usando linha de comando. 

Como?

KUBECTL - A ferramente de comando do kubernetes

CREATE - A ação

CONFIGMAP - O tipo do objeto

foursys-config - O nome do objeto

--from-literal - Parametro que usamos para informar o conteudo do ConfigMap, nesse caso vamos passar message='Seu Nome'


Clique no comando para copiar:

`kubectl create configmap foursys-config --from-literal=message=SeuNomeAqui`{{copy}}

Agora clique no terminal e pressione as teclas shift + insert, isso faz com que o comando seja colado no terminal. Agora apague o "SeuNomeAqui" e esqueva seu nome no lugar

Caso preferir, clique no comando abaixo para copiar e executar direto no terminal:
 
`kubectl create configmap foursys-config --from-literal=message='Seu Nome Aqui'`{{execute}}

Com o ConfigMap criado, você pode visualizar de duas maneiras:

`kubectl describe configmaps foursys-config`{{execute}}

Ou em formato YAML

`kubectl get configmaps foursys-config  -o yaml`{{execute}}

Se quiser deletar e criar um novo, basta executar o comando abaixo e repetir os passos anteriores, lembrando que você pode acessar os comandos executados pressionando a tecla de seta para cima no terminal:

`kubectl delete configmaps foursys-config`{{execute}}

