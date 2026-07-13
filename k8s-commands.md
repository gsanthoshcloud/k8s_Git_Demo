# Kubernetes quick commands

- Apply all manifests in this folder:
  kubectl apply -f demo-kubernetes-components/
- Delete resources:
  kubectl delete -f demo-kubernetes-components/
- View pods:
  kubectl get pods -n <namespace>
- Describe a pod:
  kubectl describe pod <pod-name> -n <namespace>
- View logs:
  kubectl logs -f <pod-name> -n <namespace>
- Exec into a pod:
  kubectl exec -it <pod-name> -- /bin/sh
- Port-forward (example for mongo-express):
  kubectl port-forward svc/mongo-express 8081:8081
