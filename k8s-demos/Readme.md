# Kubernetes Workload Components

API Version | Kind | Short Forms| Description
------------|------|------------|-----------
v1 | Namespace | ns | Logical container for all workload kinds, can not be nested.
v1 | ConfigMap | cm | Shared configuration (Environment Variables)
v1 | Secrets | secrets | Base64 Encoded environment, Digital Certs
v1 | Pod | po |Wrapper for containers
apps/v1 | ReplicaSet | rs  | Group of Identical pods
apps/v1 | Deployment | deploy |  Wrapper for ReplicaSet, Manages revision history and provides rollingUpdate
autoscaling/v1 | HorizontalPodAutoscaler | hpa | Horizontal Auto Scaling for ReplicaSet or Deployment or Stateful Sets
v1 | Service | svc | Services (ClusterIP, NodePort or LoadBalancer)
v1 | EndPoint | ep | Individual POD Endpoint for Service (Acts as a back-end)
v1 | PersistentVolume | pv | An abstract link to external storage. All read/write redirected from PV. Only way POD can consume storage.
v1 | PersistentVolumeClaim | pvc | A Request from POD to obtain "PV". Claim can be not used by more than one POD.
