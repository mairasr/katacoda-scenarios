

Outra forma de criar o ConfigMap é basear-se em um arquivo, como o .properties que você provavelmente já utiliza.

Neste exemplo iremos usar o arquivo application.properties para criar o nosso ConfigMap

`cat application.properties`{{execute}}

`kubectl create configmap doom-config --from-file=application.properties`{{execute}}

Use uma das opções abaixo para conferir o seu ConfigMap.

Describe:

`kubectl describe configmaps doom-config`{{execute}}

YAML:

`kubectl get configmaps doom-config  -o yaml`{{execute}}
