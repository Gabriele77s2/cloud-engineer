# Kubernetes

1. **Kubernetes (K8s)**: An open-source container orchestration platform used to automate the deployment, scaling, and management of containerized applications.

2. **Container**: A lightweight, standalone, and executable package that includes everything needed to run a piece of software, including code, runtime, system tools, and libraries.

3. **Pod**: The smallest deployable unit in Kubernetes, representing a single instance of a running process in a cluster, often containing one or more containers.

4. **Node**: A physical or virtual machine within a Kubernetes cluster where containers are deployed and managed.

5. **Cluster**: A set of nodes that work together, managed by Kubernetes, to run containerized applications.

6. **Master Node**: The control plane of a Kubernetes cluster, responsible for managing and coordinating all activities within the cluster.

7. **Worker Node**: Nodes within a Kubernetes cluster that run the containers and workloads.

8. **Deployment**: A Kubernetes resource that defines how to deploy and manage a set of identical pods, ensuring high availability and scalability.

9. **Service**: A Kubernetes resource that provides a stable, network endpoint to access one or more pods, enabling load balancing and service discovery.

10. **Namespace**: A way to logically divide a Kubernetes cluster into multiple virtual clusters, providing isolation, organization, and resource management.

11. **Container Orchestration**: The automated arrangement, coordination, and management of containers in a distributed environment, like Kubernetes does.

12. **ReplicaSet**: A Kubernetes resource that ensures a specified number of pod replicas are running at all times, helping with scalability and fault tolerance.

13. **Ingress**: A Kubernetes resource that manages external access to services, typically acting as a HTTP/HTTPS router or load balancer.

14. **ConfigMap**: A Kubernetes resource used to store configuration data separately from application code, allowing for configuration changes without code modifications.

15. **Secret**: A Kubernetes resource for securely storing sensitive information, such as passwords, API keys, and tokens.

16. **Persistent Volume (PV)**: A storage abstraction in Kubernetes that represents a piece of networked storage in the cluster, used by pods to persist data.

17. **Persistent Volume Claim (PVC)**: A request for storage by a user, specifying the desired storage characteristics, which is bound to a PV by Kubernetes.

18. **Helm**: A package manager for Kubernetes that simplifies the deployment and management of applications using pre-defined charts.

19. **Kubectl**: The command-line tool used to interact with and manage Kubernetes clusters.

20. **Container Registry**: A repository for storing and distributing container images, often used in conjunction with Kubernetes for application deployment.

21. **DaemonSet**: A Kubernetes resource that ensures that a specific pod runs on all or selected nodes in a cluster, typically used for system-level tasks like logging or monitoring.

22. **StatefulSet**: A Kubernetes resource designed to manage stateful applications, providing stable network identities and ordered, graceful scaling.

23. **Horizontal Pod Autoscaler (HPA)**: A Kubernetes resource that automatically adjusts the number of pod replicas in a deployment or replica set based on CPU or custom metrics.

24. **Vertical Pod Autoscaler (VPA)**: A Kubernetes component that adjusts resource requests for containers to optimize resource utilization.

25. **Custom Resource Definition (CRD)**: An extension mechanism in Kubernetes that allows you to define custom resources and their behavior.

26. **Operator**: A pattern for packaging, deploying, and managing applications as Kubernetes extensions, often implemented using custom resources and controllers.

27. **Kubelet**: The component on each worker node that communicates with the Kubernetes control plane and manages containers on the node.

28. **Etcd**: A distributed key-value store used as the backing store for all cluster data in a Kubernetes cluster.

29. **CNI (Container Network Interface)**: A specification and library for configuring network interfaces in Linux containers, allowing for different networking solutions in Kubernetes.

30. **CRUD (Create, Read, Update, Delete)**: The basic operations performed on Kubernetes resources to manage their lifecycle.

31. **RBAC (Role-Based Access Control)**: A Kubernetes feature that defines and enforces permissions and access control for users and services within the cluster.

32. **CSI (Container Storage Interface)**: A standard for exposing arbitrary block and file storage systems to containerized workloads in Kubernetes.

33. **NodeSelector**: A field in a pod's configuration that allows you to constrain which nodes your pod is eligible to be scheduled based on labels assigned to nodes.

34. **Taints and Tolerations**: Mechanisms used in Kubernetes to influence the scheduling of pods onto nodes, helping to separate workloads and control resource allocation.

35. **Kubernetes Dashboard**: A web-based user interface for managing and monitoring Kubernetes clusters.

36. **Kube-proxy**: A network proxy that runs on each node in a Kubernetes cluster, maintaining network rules on nodes and performing connection forwarding.

37. **CronJob**: A Kubernetes resource that creates jobs on a schedule, enabling the automated execution of tasks at specified intervals.

38. **Kubeconfig**: A configuration file used by `kubectl` and other Kubernetes tools to specify the cluster, user, and context information for cluster access.

39. **CSI Driver**: A component that implements the CSI specification and allows Kubernetes to interact with different storage systems.

40. **PodSecurityPolicy (PSP)**: A resource that controls the security context and policies for pods, restricting what they can do and which resources they can access.

41. **Kube-proxy**: A network proxy that runs on each node in a Kubernetes cluster, maintaining network rules on nodes and performing connection forwarding.

42. **Kube-scheduler**: A component of the Kubernetes control plane that assigns pods to nodes based on resource requirements, affinity, and other policies.

43. **Service Mesh**: A dedicated infrastructure layer for managing communication between microservices within a Kubernetes cluster, often implemented using tools like Istio or Linkerd.

44. **Kubelet Configuration**: Settings and parameters that can be configured for the Kubelet on each node, influencing its behavior and resource management.

45. **Kubernetes Events**: Logs and records of all notable events that occur in a Kubernetes cluster, providing insight into cluster activities and issues.

46. **Kubernetes State Metrics**: Metrics and data exposed by the Kubernetes API server, providing information about the state and health of the cluster.

47. **Containerd**: An industry-standard core container runtime used by Kubernetes for running containers.

48. **CRI-O**: A lightweight, open container runtime designed to work specifically with Kubernetes, serving as an alternative to Docker.

49. **Kubeadm**: A tool for bootstrapping and managing Kubernetes clusters, making it easier to set up and maintain a cluster.

50. **Multi-Tenancy**: A Kubernetes cluster configuration where multiple teams or applications share the same cluster resources while maintaining isolation and security.

51. **Network Policy**: A Kubernetes resource that allows fine-grained control over the communication between pods, implementing network-level security policies.

## Kubernetes Commands

1. **Cluster Info**: 
   - `kubectl cluster-info`: Displays the address and status of the Kubernetes cluster.
   - `kubectl config get-contexts`: Lists available contexts (cluster configurations) and shows the currently selected one.

2. **Pods**:
   - `kubectl get pods`: Lists all pods in the current namespace.
   - `kubectl describe pod <pod-name>`: Provides detailed information about a specific pod.
   - `kubectl logs <pod-name>`: Displays logs from a specific pod.
   - `kubectl exec -it <pod-name> -- <command>`: Executes a command inside a running pod.

3. **Services**:
   - `kubectl get services`: Lists all services in the current namespace.
   - `kubectl describe service <service-name>`: Provides detailed information about a specific service.

4. **Deployments**:
   - `kubectl get deployments`: Lists all deployments in the current namespace.
   - `kubectl describe deployment <deployment-name>`: Provides detailed information about a specific deployment.
   - `kubectl rollout status deployment/<deployment-name>`: Checks the status of a deployment rollout.
   - `kubectl rollout undo deployment/<deployment-name>`: Rolls back a deployment to a previous version.

5. **Nodes**:
   - `kubectl get nodes`: Lists all nodes in the cluster.
   - `kubectl describe node <node-name>`: Provides detailed information about a specific node.

6. **Configurations**:
   - `kubectl get configmaps`: Lists all ConfigMaps.
   - `kubectl get secrets`: Lists all secrets.
   - `kubectl get namespaces`: Lists all namespaces.
   - `kubectl get svc <service-name> -o yaml`: Retrieves the YAML configuration for a service.
   
7. **Scaling**:
   - `kubectl scale deployment/<deployment-name> --replicas=<number>`: Scales the number of replicas in a deployment.
   - `kubectl autoscale deployment/<deployment-name> --min=<min-pods> --max=<max-pods> --cpu-percent=<cpu-percent>`: Sets up Horizontal Pod Autoscaling (HPA).

8. **Deleting Resources**:
   - `kubectl delete pod <pod-name>`: Deletes a specific pod.
   - `kubectl delete service <service-name>`: Deletes a specific service.
   - `kubectl delete deployment <deployment-name>`: Deletes a specific deployment.
   - `kubectl delete namespace <namespace-name>`: Deletes a specific namespace and all its resources.

9. **Namespace Operations**:
   - `kubectl create namespace <namespace-name>`: Creates a new namespace.
   - `kubectl config set-context --current --namespace=<namespace-name>`: Sets the current namespace for `kubectl` commands.
   - `kubectl config view --minify --flatten`: Lists all objects in all namespaces.

10. **Applying Manifests**:
    - `kubectl apply -f <filename.yaml>`: Deploys or updates resources defined in a YAML or JSON file.
    - `kubectl apply -k <directory>`: Applies resources defined in Kustomize format.
   
11. **Port Forwarding**:
    - `kubectl port-forward <pod-name> <local-port>:<pod-port>`: Forwards local traffic to a pod.

12. **Context and Configuration**:
    - `kubectl config use-context <context-name>`: Sets the current context (cluster and user).
    - `kubectl config set-context <context-name> --cluster=<cluster-name> --user=<user-name> --namespace=<namespace>`: Creates a new context.
