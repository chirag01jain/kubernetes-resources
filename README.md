# kubernetes-resources
 One place for all the resource manifests


## nginx-example.yaml

This file will create a running nginx website within a new namespace name nginx-example. The resources that will be created are:

1) Namespace name - nginx-example
2) PV/PVC name - nginx-logs (5Gi)
3) Deployment name - nginx-deploy
4) Service with LB type - nginx-svc
