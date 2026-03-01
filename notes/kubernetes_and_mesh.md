# Kubernetes 与 Service Mesh 深度解析

## 1. Kubernetes (K8s) 核心概念
*   **Pod**：K8s 的最小调度单位。
    *   *特性*：Pod 内的容器**共享网络命名空间** (同一 IP, 通过 localhost 通信) 和 **存储卷**。
*   **Service**：定义一组 Pod 的逻辑集合，提供负载均衡。
*   **Ingress**：集群流量的入口 (L7 层代理)。

## 2. Service Mesh (服务网格)
*   **Sidecar (边车模式)**：与业务容器在同一个 Pod 中运行，透明拦截流量。
*   **数据面 (Data Plane)**：由所有 Sidecar 代理组成，负责数据的实际转发、重试、熔断。
*   **控制面 (Control Plane)**：负责全局配置管理、策略下发、服务发现。

## 3. 架构优势 (对应质量属性)
*   **可修改性 (Modifiability)**：基础设施逻辑与业务逻辑解耦，配置变更无需重新编译部署代码。
*   **安全性 (Security)**：自动实现服务间的双向 TLS (mTLS) 加密。
*   **可用性 (Availability)**：集中式的熔断、限流策略，防止雪崩。

## 🚀 考试易错点
*   问：Sidecar 与业务容器怎么通信？ 答：**localhost**。
*   问：Service Mesh 的核心优势？ 答：**跨语言、非侵入式、解耦**。
