# agrotrack-k8s

AgroTrack - Farm Microservices

This project runs two Flask microservices (user and crop) on Kubernetes using Minikube.

How to run:
1. Start Minikube and enable ingress
2. Build Docker images using `eval $(minikube docker-env)`
3. Deploy with `kubectl apply -f .`
4. Run `minikube tunnel`
5. Add `127.0.0.1 agrotrack.local` to /etc/hosts

Test:
- http://agrotrack.local/user/
- http://agrotrack.local/crop/
