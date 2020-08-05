
Agora vamos utilizar o ConfigMap criado.

No exemplo, estamos atribuindo o valor guardado no ConfigMap a uma variavel de ambiente do Pod.
Execute o comando abaixo para visualizar:
`cat pod.yaml`{{execute}}

Para executar este Pod, aplique o YAML:

`kubectl apply -f pod.yaml`{{execute}}
