
Nosso primeiro exercicio será criar um ConfigMap usando linha de comando. 

Como?

KUBECTL - A ferramenta de comandos do Kubernetes

CREATE - A ação

CONFIGMAP - O tipo do objeto

foursys-config - O nome do objeto

--from-literal - Parametro que usamos para informar o conteudo do ConfigMap, nesse caso vamos passar message='Seu Nome'


Clique no comando para copiar:

`kubectl create configmap foursys-config --from-literal=message='Seu Nome Aqui'`{{copy}}

Agora clique no terminal e pressione as teclas shift + insert, isso fará o comando ser colado no terminal. 
Agora apague o "SeuNomeAqui" e escreva seu nome no lugar

Caso preferir, clique no comando abaixo para copiar e executar direto no terminal:
 
`kubectl create configmap foursys-config --from-literal=message='Seu Nome Aqui'`{{execute}}

Com o ConfigMap criado, você pode visualizar de duas maneiras:

`kubectl describe configmaps foursys-config`{{execute}}

Ou em formato YAML

`kubectl get configmaps foursys-config  -o yaml`{{execute}}

Se quiser deletar e criar um novo, basta executar o comando abaixo e repetir os passos anteriores:

`kubectl delete configmaps foursys-config`{{execute}}

Lembrando que você pode acessar os comandos executados pressionando a tecla de seta para cima no terminal.