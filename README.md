# DevOps4Devs 02

## Aula 01
### O projeto conversão de temperatura se encontra no link abaixo:

[https://github.com/KubeDev/conversao-temperatura](https://github.com/KubeDev/conversao-temperatura)

## Aula 02
### Comando de criação do cluster Kubernetes com o K3D
```bash
k3d cluster create meucluster --servers 3 --agents 3 -p "30000:30000@loadbalancer"
```


## Aula 03

### Link para a AWS:

[https://aws.amazon.com](https://aws.amazon.com)

### Link para instalação do AWS CLI:

[https://aws.amazon.com/pt/cli](https://aws.amazon.com/pt/cli)

### URL do template usado do Cloud Formation:
```
https://s3.us-west-2.amazonaws.com/amazon-eks/cloudformation/2020-10-29/amazon-eks-vpc-private-subnets.yaml
```

# Aula 04

# Aula 05 

### Comando para obter a senha do Grafana
```
kubectl get secret --namespace default grafana -o jsonpath="{.data.admin-password}" | base64 --decode
```