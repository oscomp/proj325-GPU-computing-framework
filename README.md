# proj325-GPU-computing-framework
# 面向AI计算的可信GPU计算框架

## 项目描述

目前AI计算应用广泛并且发展迅猛，由于需要处理大量的并发计算，目前的AI框架会调用GPU等加速器来提升AI算力。

然而AI框架运行的敏感数据以及模型本身都会受到攻击并泄露，如攻击者使用提权漏洞获取内核权限并直接读取传递给GPU的数据信息。

为了防止恶意的攻击者，需要构架一套可信GPU计算框架，保证AI计算安全。本项目旨在使用CPU TEE技术，利用软硬件协同手段为GPU构造隔离计算环境，并保证AI计算数据在内核中的安全流通。

## 预期目标

- 扩展CPU TEE安全能力，并应用于GPU中，保证GPU中的数据传输与计算安全；
- 加固AI计算使用的内核模块，防止内核特权攻击；
- 可信GPU模块的安全高效切换，不干扰原有系统的运行；

## 特征

- 熟练掌握CPU TEE软硬件协同技术，并应用于外设接口保护GPU的计算安全
- 重写GPU计算模块，单独构造隔离区间保护GPU的运算数据
- 熟练掌握AI框架，梳理AI计算中的数据流传输过程，保证数据流不被恶意获取
- 熟练端侧的内核开发以及软件安全编写规范

## 已有参考资料

- [optee_os](https://github.com/OP-TEE/optee_os)
- [optee_client](https://github.com/OP-TEE/optee_client)
- [optee_linuxdriver](https://github.com/OP-TEE/optee_linuxdriver)

## 赛题分类

2.3 操作系统内核大类 -->  2.3.7 安全操作系统/可信执行环境

## 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生或研究生
- 允许学生参加大赛的多个不同题目，最终自己选择一个题目参与评奖
- 请遵循“2024全国大学生操作系统比赛”的章程和技术方案要求

## 难度

高等

## License

GPL-3.0 License

## 所属赛道

2024全国大学生操作系统比赛的“OS功能挑战”赛道

## 项目导师

- 姓名：王杰
- 单位：华中科技大学
- github ID：[https://github.com/ongoing-jw](https://github.com/ongoing-jw)
- email：[wangjie_s@hust.edu.cn](mailto:wangjie_s@hust.edu.cn)
