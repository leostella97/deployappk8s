# Deploy de uma aplicação Kubernetes

Exemplo básico de um arquivo YAML que descreve todos os recursos necessários para implantar uma aplicação em um cluster Kubernetes.

Para começar, vamos falar sobre o Deployment. Nesse recurso, você precisa especificar o nome da sua aplicação, o número de réplicas que deseja,
a imagem do container que deseja implantar (no caso, foi usado o Ubuntu versão final) e os recursos de CPU e memória necessária para a aplicação. Com essas informações,
o Kubernetes pode criar e gerenciar os pods que executam a aplicação.

Agora, vamos ao Service. Aqui, você precisa fornecer o nome da sua aplicação, selecionar o conjunto de pods que deseja expor (no caso, app: myapp)
e definir a porta que deseja expor (no caso, port: 80). Com isso, o Kubernetes pode criar um ponto de acesso para sua aplicação dentro do cluster.

No exemplo, o tipo de serviço é LoadBalancer, que permite que você acesse sua aplicação de fora do cluster.
Mas é importante lembrar que existem outros tipos de serviços que você pode usar, dependendo do que precisa.
