# Prometheus-kubernetes
Integrate Prometheus monitoring in Kubernetes cluster

Clone this repo in your working area and deploy these files using kubctl in your kubernetes cluster as below,

kubectl apply -f -n <namespace> <FILENAME>
  
Once all the files are deployed, verify all the above resource using below commands:
  kubectl get deploy
  kubectl get prometheus
  kubectl get pod
  kubectl get service
  
Access Prometheus UI with below command:
  
  kubectl port-forward svc/prometheus 9090
  
Now open below URL from Your Kubernetes cluster, Master node in Dashboard using Chrome or Mozilla Firefox,
  
URL: http://localhost:9090
