
Agora vamos deletar esse ConfigMap e recria-lo com YAML para nosso próximo exemplo.

`kubectl delete configmap doom-config`{{execute}}

Vamos olhar a estrutura do YAML antes de aplica-lo?

`cat doom-config.yaml`{{execute}}

Lembrando que os valores esperado para configurar o fogo do Doom são: 

Sentido: 0 - Crescente para a esquerda, 1 - Centralizado, 2 - Crescente para a direita.

Intensidade: de 0 a 36.

Criando o ConfigMap com YAML:

`kubectl apply -f doom-config.yaml`{{execute}}

Use uma das opções abaixo para conferir se o seu ConfigMap foi criado corretamente.

Describe:

`kubectl describe configmaps doom-config`{{execute}}

YAML:

`kubectl get configmaps doom-config  -o yaml`{{execute}}

