# 云原生架构 (Cloud Native)

## 1. 微服务治理的两大派系
*   **侵入式 (SDK 模式)**：如 Spring Cloud。
    *   *优点*：性能好（无额外代理）、与语言深度集成、成熟度高。
    *   *缺点*：绑定特定语言、SDK 升级困难（需重新发布业务逻辑）。
*   **非侵入式 (Service Mesh 模式)**：如 Istio + Envoy。
    *   *关键概念*：**Sidecar (边车模式)**、**Control Plane (控制面)** vs **Data Plane (数据面)**。
    *   *优点*：多语言支持、透明管理、解耦。
    *   *缺点*：网络延迟、资源消耗、运维复杂。

## 2. Serverless (无服务器)
*   **FaaS (函数即服务)**：代码片段，事件触发（如 AWS Lambda）。
*   **BaaS (后端即服务)**：如云数据库、云存储。
*   *特点*：全托管、按需扩缩容、**冷启动问题 (Cold Start)**。

## 3. 容器化
*   **K8s (Kubernetes)**：容器编排的标准。
*   *核心对象*：Pod, Service, Ingress, ConfigMap, Deployment.
