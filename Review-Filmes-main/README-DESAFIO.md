# devops4devs-02
docker push 94rnerick/desafiodevops:v3

docker pull 94rnerick/desafiodevops:v3

#criar o arquivo deployment.yaml de acordo com o deploy e service

kubectl apply -f deployment.yaml

acessar localhost:30000

Editar o arquivo _Layout.cshtml e salvar

docker build -t 94rnerick/desafiodevops:v4 -f src/Review-Filmes.Web/Dockerfile src/

docker push 94rnerick/desafiodevops:v4

docker pull 94rnerick/desafiodevops:v4

Editar o arquivo deployment.yaml na pasta src linha 56 image para nova imagem

kubectl apply -f deployment.yaml && watch 'kubectl get pod' 
#para observar a troca de versao 
