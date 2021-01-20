# kubernetes-resources
 One place for all the resource manifests


## nginx-example.yaml

This file will create a running nginx website within a new namespace name nginx-example. The resources that will be created are:

1) Namespace name - nginx-example
2) PV/PVC name - nginx-logs (5Gi)
3) Deployment name - nginx-deploy
4) Service with LB type - nginx-svc

Commands to use to setup and explore more:

 - Create a file, say with filename: "nginx-example.yaml" and copy/save the file content in the newly created file.
 - kubectl create -f filename.yaml 
 - kubectl get ns nginx-example
 - kubectl get deploy -n nginx-example
 - kubectl get svc -n nginx-example
 - kubectl get pv -n nginx-example
 - kubectl get pods -n nginx-example
 - kubectl exec -it nginx-deploy-76bf4df5b-ksn5v -n nginx-example /bin/bash 

### In the last command - "nginx-deploy-76bf4df5b-ksn5v" is the pod-name. Once you run the command, you'll exec into the pod container where the volume is mounted. The mount path is "/var/log/nginx" (persistent storage). You can exit the container via "exit" command.
  
