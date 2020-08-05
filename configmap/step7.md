No link abaixo você pode conferir o resultado e observe com atenção a direção e intensidade, pois irá mudar...

Os valores esperado para o sentido são: 0 - Crescente para a esquerda, 1 - Centralizado, 2 - Crescente para a direita
A intensidade pode variar de 0 a 36.

https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com

Caso não consiga acessar ainda, use o comando abaixo para checar se o IP externo foi definido, senão estiver preenchido ainda, aguarde alguns minutos e tente novamente.

`kubectl get services`{{execute}}


Agora vamos aplicar outro Yaml com os parametros de renderização da chama alterados.

`cat doom-config2.yaml`{{execute}}

`kubectl apply -f doom-config2.yaml`{{execute}}

Agora atualize a página, por favor...mudou?

Vamos tentar outro?

`cat doom-config3.yaml`{{execute}}

`kubectl apply -f doom-config3.yaml`{{execute}}

Agora atualize a página, por favor...mudou?
