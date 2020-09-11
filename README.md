<br> yum install git </br>
<br> git clone https://github.com/vipin-k/kubernetes-ingress.git </br>
<br> cd kubernetes-ingress/ </br>
<br> cd deployments/ </br>
<br> kubectl apply -f common/ns-and-sa.yaml </br>
<br> kubectl apply -f common/default-server-secret.yaml </br>
<br> kubectl apply -f common/nginx-config.yaml </br>
<br> kubectl apply -f common/custom-resource-definitions.yaml </br>
<br> kubectl apply -f rbac/rbac.yaml </br>
<br> kubectl apply -f daemon-set/nginx-ingress.yaml </br>
<br> kubectl get pods -n nginx-ingress </br>
<br> kubectl logs nginx-ingress-ck662 -n nginx-ingress </br>
