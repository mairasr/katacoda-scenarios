
## Como criar um ConfigMap

Nosso primeiro exercicio será criar um ConfigMap usando linha de comando. 

`kubectl create configmap foursys-config --from-literal=message=TeamFoursys`{{execute}}

Com o ConfigMap criado, você pode visualizar de duas maneiras:

`kubectl describe configmaps foursys-config`{{execute}}

Ou em formato YAML

`kubectl get configmaps foursys-config  -o yaml`{{execute}}

