<p align="center">
  <img src="https://img.shields.io/badge/CANN-OpenSoftware%202.0-blue" />
  <img src="https://img.shields.io/badge/Electrical%20Engineering%20SIG-CANN%20Community-orange" />
  <img src="https://img.shields.io/badge/license-Apache%202.0-green" />
  <img src="https://img.shields.io/badge/status-active-brightgreen" />
</p>

> **elec-ops-simulation** 是 CANN 社区 Electrical Engineering SIG（电力行业兴趣小组）旗下的电力仿真求解算子库，
> 聚焦于计算电网在稳态运行条件下各节点的电压、相角，以及各支路（线路、变压器）的功率分布的仿真核心需求，面向华为昇腾（Ascend）硬件平台进行深度优化。

---

## 项目背景

电力系统仿真求解是保障电网安全稳定运行的关键技术支撑。在新型电力系统构建背景下，传统仿真工具在处理高比例新能源接入、多变量耦合交互、动态响应分析等复杂场景时，面临"**建模难、求解慢、精度低**"的技术挑战。

本仓库通过在昇腾 CANN 平台上提供专用优化算子，使电力 AI 仿真模型具备以下能力：

- **多物理场耦合实时仿真**：内嵌电网物理约束，实现电磁-热力-机械多场耦合的实时动态求解
- **新能源动态特性建模**：精准刻画风光储系统的非线性响应特性与随机波动规律
- **多时间尺度协同仿真**：支持从秒级暂态到年周期稳态的跨时间尺度联合仿真分析




## 核心算子列表

| 算子名称                    | 场景     | 描述               | 状态     |
| ----------------------- | ------ | ---------------- | ------ |
| `accumulate_nv2`             | 数学计算算子 | 对大规模张量加分运算做了性能优化 | ✅ 已发布  |

---

## 🤝 参与贡献

欢迎所有对电力 AI 和昇腾开发感兴趣的开发者参与共建！贡献方式：

1. 提交 Issue 反馈问题或建议
2. Fork 本仓库并提交 Pull Request
3. 参与 Electrical Engineering SIG 定期研讨会
4. 完善文档与示例

贡献规范请参考 [`CONTRIBUTING.md`]()。

---

## 👥 维护团队

**Maintainers**

|姓名|GitCode ID|单位|
|---|---|---|
|梁寿愚|@jason2025|南方电网人工智能研究中心|
|陆璐|@Lulu_scut|华南理工大学|
|陈辰|@xchencehn|杭州天宽科技|
|张玉橙|@Splendid2025|昇腾产品线|
|田野|@tianye525|AI算力基础设施|

**Committers**

|姓名|GitCode ID|单位|
|---|---|---|
|余涛|@yutao_scut|华南理工大学电力学院|
|刘迪|@weixin_34344963|清华大学电机系|
|江豪|@yhyyyl|华南理工大学 / 南方电网联培|
|陈昀|@edconeone|华南理工大学|
|莫程翔|@Andrewmo1|华为公司|
|李博|@gcw_FHrfwZBn|华为公司|

---

## 📄 许可证

本项目基于 [Apache License 2.0]() 开源。
