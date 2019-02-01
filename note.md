## Fri. 1 Feb 2019

### Kubernetes

#### Techs

1.  prometeus
2.  grafana
3.  tracing
4.  tracing
5.  logging
6.  Go Kit : https://github.com/go-kit/kit
7.  IsTio ( Proxy ) : https://github.com/istio/istio

https://github.com/up1/microservice-workshop

#### Notes

1. Health Check <br />
   Liveness<br />
   Readiness<br />
2. Deploy<br />
   Config Map<br />

## Thu. 31 Jan 2019

### Kubernetes

Learn Kubernetes With P' Pui At KBTG
https://github.com/up1/course-kubernetes-in-practice

#### Techs

1.  https://www.fluentd.org/

#### Notes

1. Get anythings by comma. For example: <br />
   kubectl get deployment,rs,pods
2. Firewall: <br />
   gcloud compute firewall-rules create <firewallname> --allow tcp:<portNumber>
3. Revisioning: <br />
   kubectl rollout undo deployment/hello --to-revision=1
4. Scaling <br >
   kubectl scale deployment hello --replicas=5
   NodePort => Can access via all node in cluster to desire port.
5. Deployment strategy <br >
   5.1 Terminate <br />
   5.2 Ramp (kubernetes)
   5.3 BlueGreen
   5.4 Canary ( ไม่ route มา service ใหม่ทั้งหมด)
   5.5 A/B Testing
   5.6 Shadow: deploy along side, use same request without production impact
6. HPA Horizontal Scale Auto

- Metrics-Server >> time series database collect memory and cpu usage info.
- Caution: Only scale on pod.

7. Inspect all system services

- kube get pod --namespace kube-system
