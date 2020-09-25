# K8s_PodsIP
to deploy seamless Service from Front-end and Back-end Replica Pods


容器在同一 Pod 則存取共同 IP，並利用容器不同的 port 做繫結 bind() 溝通彼此。
而 pod 而言，會配置一獨立的 IP，不與其他 Pod 的 IP 重複，即便是在同一 node 上（可能是虛擬機）。
再者，經過 RC 的副本處理後，pod 不只是一個人，而是成千上萬的 pod 共同擁有同一服務 Service，對於前端來說，
透過 Label Selector 存取 pod，倘若叢集中某一 pod 死亡，也有其他 pod 補上服務的位子，可以說相當的便利與穩定。

# 虛擬化後端

對外服務的 Master Node 則使用 pod 的 IP 結合容器的 port 行成可以對外服務的虛擬後端端點 EndPoint。

# IP 配置方式

  (to be continued...)








