1 - processo de build da imagem
docker build -t xenxem/review-filmes:v1 -f src/Review-Filmes.Web/Dockerfile src/

2 - subida da imagem para meu docker hub
docker push xenxem/review-filmes:v1

3 - aplicação do manifesto para criação do cluster com os objetos
kubectl apply -f k8s/deployment.yml

4 - listagem dos elementos
kubectl get pod

5 - acesso da aplicação em localhost porta 30000

6 - escolha de um pod qualquer para exclusão para testar a resiliência
reviewfilmes-54789cf48f-wwqr5

7 - listagem com kubectl get pod para verificar

8 - alteração do header para v2 em shared/\_Layout.cshtml

9 - geração da imagem para v2
docker build -t xenxem/review-filmes:v2 -f src/Review-Filmes.Web/Dockerfile src/

10 - push da imagem para o meu docker hub
docker push xenxem/review-filmes:v2

12 - aplicação do manifesto
kubectl apply -f k8s/deployment.yml
