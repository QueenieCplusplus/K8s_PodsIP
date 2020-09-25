# K8s_PodsIP
to deploy seamless Service from Front-end and Back-end Replica Pods


容器在同一 Pod 則存取共同 IP，並利用容器不同的 port 做繫結 bind() 溝通彼此。
而 pod 而言，會配置一獨立的 IP，不與其他 Pod 的 IP 重複，即便是在同一 node 上（可能是虛擬機）。








