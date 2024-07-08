#realizacao do caminho com comandos e acoes

k3d cluster create meucluster --servers 3 --agents 3 -p "30000:30000@loadbalancer"



docker build -t 94rnerick/desafiodevops:v1 -f src/Review-Filmes.Web/Dockerfile src/

docker push 94rnerick/desafiodevops:v1

docker pull 94rnerick/desafiodevops:v1

#criar o arquivo deployment.yaml de acordo com o deploy e service

kubectl apply -f deployment.yaml

acessar localhost:30000

Editar o arquivo _Layout.cshtml e salvar

docker build -t 94rnerick/desafiodevops:v2 -f src/Review-Filmes.Web/Dockerfile src/

docker push 94rnerick/desafiodevops:v2

docker pull 94rnerick/desafiodevops:v2

Editar o arquivo deployment.yaml na pasta src linha 56 image para nova imagem

kubectl apply -f deployment.yaml && watch 'kubectl get pod' 
#para observar a troca de versao 
