
## Usando o ConfigMap

Agora vamos utilizar o ConfigMap criado.

No exemplo abaixo, estamos atribuindo o valor guardado no ConfigMap a uma variavel de ambiente do Pod.

`apiVersion: v1                   `
`kind: Pod                        `
`metadata:                        `
`  name: command-demo             `
`  labels:                        `
`    purpose: demonstrate-command `
`spec:                            `
`  containers:                    `
`  - name: command-demo-container `
`    image: debian                `
`    command: ["/bin/echo"]       `
`    args: ["$(MESSAGE)"]         `
`    env:                         `
`     - name: MESSAGE             `
`       valueFrom:                `
`         configMapKeyRef:        `
`           name: foursys-config  `
`           key: message          `
`   restartPolicy: OnFailure      `

Para executar este Pod, aplique o YAML:

`kubectl apply -f pod.yaml`{{execute}}
