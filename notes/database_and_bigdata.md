# 数据库与大数据架构

## 1. 理论基石
*   **ACID**：传统关系型数据库 (RDBMS) 的核心。
*   **BASE (Basically Available, Soft state, Eventually consistent)**：分布式系统的核心。
    *   基本可用、软状态、**最终一致性**。
*   **CAP 定理**：分布式系统三选二 (通常选 AP 或 CP)。

## 2. 存储选型策略
*   **读写分离**：解决读压力大。
*   **分库分表 (Sharding)**：解决存储容量和写压力。
*   **NoSQL 补充**：
    *   缓存选 Redis。
    *   复杂对象存 MongoDB。
    *   百亿级日志存 HBase。
    *   关系追踪选 Neo4j。

## 3. 大数据架构演进
*   **数据仓库 (Data Warehouse)**：结构化、ETL、决策支持。
*   **数据湖 (Data Lake)**：原格式存储、海量非结构化、Schema-on-read。
*   **Lambda 架构**：批处理层 + 流处理层 (经典、稳定)。
*   **Kappa 架构**：纯流处理层 (未来趋势、对流处理引擎要求高)。
*   **湖仓一体 (Lakehouse)**：融合了数据湖的灵活性和数仓的严谨性 (最新热点)。
