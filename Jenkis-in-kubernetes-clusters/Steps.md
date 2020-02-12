How to setup the jenkins inkubernetes clusters example steps

1. Run jenkin docker image
> docker build -t myjenkins .
2. Create persistent volume claim
> kubectl apply -f <claim file>
3. Deployment myjenkins image
> kubectl apply -f <deployment file>