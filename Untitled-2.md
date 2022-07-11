Name:               multi-worker
Roles:              <none>
Labels:             beta.kubernetes.io/arch=amd64
                    beta.kubernetes.io/os=linux
                    kubernetes.io/arch=amd64
                    kubernetes.io/hostname=multi-worker
                    kubernetes.io/os=linux
Annotations:        kubeadm.alpha.kubernetes.io/cri-socket: unix:///run/containerd/containerd.sock
                    node.alpha.kubernetes.io/ttl: 0
                    volumes.kubernetes.io/controller-managed-attach-detach: true
CreationTimestamp:  Sun, 03 Jul 2022 13:41:06 +0200
Taints:             <none>
Unschedulable:      false
Lease:
  HolderIdentity:  multi-worker
  AcquireTime:     <unset>
  RenewTime:       Sun, 03 Jul 2022 14:27:05 +0200
Conditions:
  Type             Status  LastHeartbeatTime                 LastTransitionTime                Reason                       Message
  ----             ------  -----------------                 ------------------                ------                       -------
  MemoryPressure   False   Sun, 03 Jul 2022 14:24:57 +0200   Sun, 03 Jul 2022 13:41:06 +0200   KubeletHasSufficientMemory   kubelet has sufficient memory available
  DiskPressure     False   Sun, 03 Jul 2022 14:24:57 +0200   Sun, 03 Jul 2022 13:41:06 +0200   KubeletHasNoDiskPressure     kubelet has no disk pressure
  PIDPressure      False   Sun, 03 Jul 2022 14:24:57 +0200   Sun, 03 Jul 2022 13:41:06 +0200   KubeletHasSufficientPID      kubelet has sufficient PID available
  Ready            True    Sun, 03 Jul 2022 14:24:57 +0200   Sun, 03 Jul 2022 13:41:17 +0200   KubeletReady                 kubelet is posting ready status
Addresses:
  InternalIP:  172.22.0.3
  Hostname:    multi-worker
Capacity:
  cpu:                12
  ephemeral-storage:  263174212Ki
  hugepages-1Gi:      0
  hugepages-2Mi:      0
  memory:             78915220Ki
  pods:               110
Allocatable:
  cpu:                12
  ephemeral-storage:  263174212Ki
  hugepages-1Gi:      0
  hugepages-2Mi:      0
  memory:             78915220Ki
  pods:               110
System Info:
  Machine ID:                 a9beb71f02a648cca78ae73e0f89d8b4
  System UUID:                a9beb71f02a648cca78ae73e0f89d8b4
  Boot ID:                    df92d5e2-c4e9-49a1-b562-a5b138db9df5
  Kernel Version:             5.10.16.3-microsoft-standard-WSL2
  OS Image:                   Ubuntu 21.10
  Operating System:           linux
  Architecture:               amd64
  Container Runtime Version:  containerd://1.6.4
  Kubelet Version:            v1.24.0
  Kube-Proxy Version:         v1.24.0
PodCIDR:                      10.241.1.0/24
PodCIDRs:                     10.241.1.0/24
ProviderID:                   kind://docker/multi/multi-worker
Non-terminated Pods:          (5 in total)
  Namespace                   Name                CPU Requests  CPU Limits  Memory Requests  Memory Limits  Age
  ---------                   ----                ------------  ----------  ---------------  -------------  ---
  default                     debug2              0 (0%)        0 (0%)      0 (0%)           0 (0%)         45m
  default                     hello               0 (0%)        0 (0%)      0 (0%)           0 (0%)         13m
  default                     p1                  0 (0%)        0 (0%)      0 (0%)           0 (0%)         45m
  kube-system                 kindnet-8kkbm       100m (0%)     100m (0%)   50Mi (0%)        50Mi (0%)      46m
  kube-system                 kube-proxy-nh2bl    0 (0%)        0 (0%)      0 (0%)           0 (0%)         46m
Allocated resources:
  (Total limits may be over 100 percent, i.e., overcommitted.)
  Resource           Requests   Limits
  --------           --------   ------
  cpu                100m (0%)  100m (0%)
  memory             50Mi (0%)  50Mi (0%)
  ephemeral-storage  0 (0%)     0 (0%)
  hugepages-1Gi      0 (0%)     0 (0%)
  hugepages-2Mi      0 (0%)     0 (0%)
Events:
  Type    Reason                   Age                From             Message
  ----    ------                   ----               ----             -------
  Normal  Starting                 45m                kube-proxy
  Normal  Starting                 46m                kubelet          Starting kubelet.
  Normal  NodeHasSufficientMemory  46m (x2 over 46m)  kubelet          Node multi-worker status is now: NodeHasSufficientMemory 
  Normal  NodeHasNoDiskPressure    46m (x2 over 46m)  kubelet          Node multi-worker status is now: NodeHasNoDiskPressure   
  Normal  NodeHasSufficientPID     46m (x2 over 46m)  kubelet          Node multi-worker status is now: NodeHasSufficientPID    
  Normal  NodeAllocatableEnforced  46m                kubelet          Updated Node Allocatable limit across pods
  Normal  RegisteredNode           46m                node-controller  Node multi-worker event: Registered Node multi-worker in 
Controller
  Normal  NodeReady                45m                kubelet          Node multi-worker status is now: NodeReady