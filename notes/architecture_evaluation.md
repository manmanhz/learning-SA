# 核心术语：架构评估 (必考)

## 1. 质量属性 (Quality Attributes)
*   **可用性 (Availability)**：关注故障恢复。关键词：心跳、冗余、故障切换。
*   **性能 (Performance)**：关注响应时间、吞吐量。关键词：缓存、负载均衡、并发、响应时间。
*   **安全性 (Security)**：关注授权、加密、审计、完整性。
*   **可修改性 (Modifiability)**：关注维护成本。关键词：解耦、封装、通用化。

## 2. 评估三兄弟
*   **敏感点 (Sensitivity Point)**：针对**一个**属性。某个特性的改变对该属性影响极大。
*   **权衡点 (Trade-off Point)**：针对**两个或多个**属性。由于 A 的改变，导致 B 变差。
*   **风险点 (Risk)**：架构中潜在的、未确定的隐患。

## 3. 架构评估方法
*   **ATAM (Architecture Trade-off Analysis Method)**：架构权衡分析法。
*   **SAAM (Software Architecture Analysis Method)**：主要评估可修改性。
