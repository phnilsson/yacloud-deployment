# yacloud-deployment
Rollout traininglog:
kubectl.exe --kubeconfig .\CloudNative-kubeconfig.yaml rollout restart deployment/traininglog -n traininglog

kubectl.exe --kubeconfig .\CloudNative-kubeconfig.yaml apply -f

Secrets:
kubectl --kubeconfig .\CloudNative-kubeconfig.yaml --namespace traininglog create secret generic postgres-secret --from-literal=postgres-password=POSTGRES_PASSWORD