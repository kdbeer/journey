## Thu. 31 Jan 2019
### Kubernetes

Learn Kubernetes With P' Pui At KBTG
https://github.com/up1/course-kubernetes-in-practice

#### notes

1. Get anythings by comma. For example: <br />
  kubectl get deployment,rs,pods
2. Firewall: <br />
  gcloud compute firewall-rules create <firewallname> --allow tcp:<portNumber>
3. Revisioning: <br />
  kubectl rollout undo deployment/hello --to-revision=1
4. Scaling <br >
  kubectl scale deployment hello --replicas=5
