
Agora vamos utilizar o ConfigMap criado.

No exemplo, estamos atribuindo o valor guardado no ConfigMap a uma variavel de ambiente do Pod.
Execute o comando abaixo para visualizar:

`cat pod.yaml`{{execute}}

Para executar este Pod, aplique o YAML:

`kubectl apply -f pod.yaml`{{execute}}

Com o comando abaixo podemos verificar que o nosso Pod foi criado com sucesso:

`kubectl get pods`{{execute}}

E com este comando vemos o resultado no log:

`kubectl logs configmap-demo`{{execute}}
