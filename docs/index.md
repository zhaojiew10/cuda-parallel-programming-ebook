---
title: "CUDA 并行编程"
---

# CUDA 并行编程

依据 **Mastering Parallel Programming with CUDA Platform** 重构的中文书面教程。原 83 讲按知识关联合并为 **4 个部分、26 章**，通过连贯论述、代码和配图组织内容。

[开始阅读：第 1 章](chapters/ch01.md){ .md-button .md-button--primary }  [阅读与实践指南](guide.md){ .md-button }  [术语表](glossary.md){ .md-button }

## 推荐阅读路径

- **系统入门**：按第 1 → 26 章顺序学习。
- **执行与性能优化**：阅读第 8—12 章，再学习第 13—19 章的内存与片上通信。
- **异步并发**：阅读第 20—21 章；基础事件计时位于第 7 章。
- **数值、扫描与压缩**：阅读第 22—24 章。
- **图像处理扩展**：阅读第 25—26 章。

## 全书目录

### 第一部分 · CUDA 入门与程序骨架（第 1—7 章）

从并行问题分析走到可验证、可计时、可查询设备限制的向量加法程序，形成第一个完整的 CUDA 工程闭环。

- [第 1 章 并行计算与 CUDA 入门](chapters/ch01.md)
- [第 2 章 配置环境并运行第一个 CUDA 程序](chapters/ch02.md)
- [第 3 章 用网格和线程块定位数据](chapters/ch03.md)
- [第 4 章 全局索引与边界检查](chapters/ch04.md)
- [第 5 章 完成一次向量加法](chapters/ch05.md)
- [第 6 章 验证结果并处理 CUDA 错误](chapters/ch06.md)
- [第 7 章 计时并查询设备能力](chapters/ch07.md)

### 第二部分 · 理解 GPU 执行与归约优化（第 8—12 章）

用同一条归约主线连接 SM、Warp、占用率、性能分析、展开优化和动态并行，建立从硬件执行到公平性能对比的认识。

- [第 8 章 理解 SM、Warp 与线程执行](chapters/ch08.md)
- [第 9 章 Warp 分化与占用率](chapters/ch09.md)
- [第 10 章 实现并行归约](chapters/ch10.md)
- [第 11 章 优化归约：展开与 Shuffle](chapters/ch11.md)
- [第 12 章 在设备端启动核函数](chapters/ch12.md)

### 第三部分 · 优化内存访问与片上通信（第 13—19 章）

从主机—设备数据路径进入 Warp 地址分析，再用矩阵转置、共享内存、常量广播和 Warp Shuffle 讨论数据重用与通信。

- [第 13 章 管理主机与设备之间的数据](chapters/ch13.md)
- [第 14 章 让全局内存访问更连续](chapters/ch14.md)
- [第 15 章 实现并优化矩阵转置](chapters/ch15.md)
- [第 16 章 理解共享内存与 Bank 冲突](chapters/ch16.md)
- [第 17 章 用共享内存完成块内归约](chapters/ch17.md)
- [第 18 章 用共享内存优化矩阵转置](chapters/ch18.md)
- [第 19 章 用 Shuffle 完成分层归约](chapters/ch19.md)

### 第四部分 · 综合并行实践（第 20—26 章）

把前面建立的执行、内存和同步知识用于完整任务：先组织异步流水线，再处理数值与扫描，最后进入图像处理和 OpenCV 环境。

- [第 20 章 用 CUDA 流重叠传输与计算](chapters/ch20.md)
- [第 21 章 用事件管理异步依赖](chapters/ch21.md)
- [第 22 章 处理浮点误差与并发更新](chapters/ch22.md)
- [第 23 章 实现块内并行扫描](chapters/ch23.md)
- [第 24 章 扩展到跨块扫描与流压缩](chapters/ch24.md)
- [第 25 章 用 CUDA 处理图像像素](chapters/ch25.md)
- [第 26 章 理解图像并配置 OpenCV 环境](chapters/ch26.md)

## 配套页面

- [阅读与实践指南](guide.md)：了解本书结构、实践方法和校对原则。
- [CUDA 术语表](glossary.md)：统一常见术语的中英文表达。
