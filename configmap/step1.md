
## Como criar um ConfigMap

Nosso primeiro exercicio será criar um ConfigMap usando um Arquivo. 

`kubectl create configmap foursys-config --from-file=application.properties`{{execute}}

Com o ConfigMap criado, você pode visualizar de duas maneiras:

`kubectl describe configmaps foursys-config`{{execute}}

Ou em formato YAML

`kubectl get configmaps foursys-config  -o yaml`{{execute}}

