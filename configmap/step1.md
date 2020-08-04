## Como criar e usar um ConfigMap

Nosso primeiro exercicio será criar um ConfigMap apartir de um Arquivo. 

`kubectl create configmap foursys-config --from-file=application.properties`{{execute}}

Com o ConfigMap criado, você pode visualizar de duas maneiras:

`kubectl describe configmaps foursys-config`

Ou em formato YAML

`kubectl get configmaps foursys-config  -o yaml`

