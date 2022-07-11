https://console.cloud.google.com/gcr/images/google-samples/GLOBAL

https://console.cloud.google.com/gcr/images/google-containers/GLOBAL

https://itnext.io/kubernetes-kind-cheat-shee-2605da77984

https://theithollow.com/2019/02/05/kubernetes-service-publishing/

https://medium.com/@pczarkowski/kubernetes-tip-run-an-interactive-pod-d701766a12


kubectl run -i --tty --rm debug --image=busybox --restart=Never -- sh
 

docker run -d — restart=always -p 127.0.0.1:5000:5000 — name cncf-cheat-sheet-registry registry:2

kubectl run -i --tty --rm debug2 --image=busybox --restart=Never -- sh

https://mauilion.dev/posts/kind-pvc-localdata/

kind delete cluster kind-kind-multi

kubectl exec --stdin --tty shell-demo -- /bin/bash

 kind create cluster --config clustermultinodo.yaml 


 10-241-2-2.default.pod.cluster.local


  kubectl exec --stdin --tty foo -c bar -- /bin/bash
 kubectl scale deployment web-server --replicas 3
 

  docker run -d -p 5001:5001  -e REGISTRY_HTTP_ADDR=0.0.0.0:5001 --restart=always --name kind-registry registry:2

   docker push localhost:5001/hello-app:1.0
docker tag gcr.io/google-samples/hello-app:1.0 localhost:5001/hello-app:1.0

kind load docker-image curso-kind-node:0.0.2 --name multi


https://console.cloud.google.com/gcr/images/kubeflow-images-public/GLOBAL"# curso-kind" 
