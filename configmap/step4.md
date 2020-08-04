
## Criando o ConfigMap usando um Arquivo

Outra forma de criar o ConfigMap é basear-se em um arquivo, como o properties que você provavelmente já utiliza.

No próximo exemplo iremos usar o arquivo application.properties para criar o nosso ConfigMap

`kubectl create configmap application-config --from-file=application.properties`{{execute}}

Use uma das opções abaixo para conferir o seu ConfigMap.

Describe:

`kubectl describe configmaps application-config`{{execute}}

YAML:

`kubectl get configmaps application-config  -o yaml`{{execute}}
