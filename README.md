<p align="center">
  <img src="assets/hero.png" alt="游城 youcheng · 移动端前端 · AI 应用" width="100%">
</p>

# 你好，我是 youcheng10d

在读学生，做移动端前端与 AI 应用。
正在把“今天吃啥”这件小得不能再小的事，做成一个真的有人在用的产品；也在研究一件事：AI 怎样才能记住一个人，而不是每次从零开始。

## 现在在做

### 吃嘛 · What to Eat

面向大学生的食堂菜品推荐 Web 应用。说一句偏好（“减肥、预算 15 元、不想吃辣”），它从真实菜品库里挑出一道菜，并告诉你去哪个食堂、哪个档口。

| 项目 | 现状 |
| --- | --- |
| 菜品库 | 2382 道，65 个档口，2 个食堂 |
| 形态 | 静态前端 + 无服务器 AI 代理；Pro / Flash 双版本 |
| AI 边界 | 只做理解，不做挑选；热量由本地成分表逐项计算，可展开复核 |
| 交付 | 在线 Pages + 单文件离线版；7 个测试脚本，含变异测试 |
| 参赛 | 第二十届全国大学生软件创新大赛 · 传智杯 AI 创新应用挑战赛 |

- 在线体验：[youcheng10d.github.io/what-to-eat](https://youcheng10d.github.io/what-to-eat/)（手机打开效果最佳）
- 仓库：[youcheng10d/what-to-eat](https://github.com/youcheng10d/what-to-eat)
- 开发日志（8 篇）：[01](https://github.com/youcheng10d/what-to-eat/blob/main/docs/blog/blog-01-v0.1.md)、[02](https://github.com/youcheng10d/what-to-eat/blob/main/docs/blog/blog-02-v1.0.md)、[03](https://github.com/youcheng10d/what-to-eat/blob/main/docs/blog/blog-03-v1.2.md)、[04](https://github.com/youcheng10d/what-to-eat/blob/main/docs/blog/blog-04-v2.0.md)、[05](https://github.com/youcheng10d/what-to-eat/blob/main/docs/blog/blog-05-v2.1.md)、[06](https://github.com/youcheng10d/what-to-eat/blob/main/docs/blog/blog-06-v2.1.2.md)、[07](https://github.com/youcheng10d/what-to-eat/blob/main/docs/blog/blog-07-wenli.md)、[08](https://github.com/youcheng10d/what-to-eat/blob/main/docs/blog/blog-08-v2.3.2.md)

### 可审计的记忆系统

两轮工程实验，比较抽取式记忆、篇级索引与行级检索，结论是：**主路必须是“原文 + 追加账本 + 行级检索”**，索引只负责定位，回答必须回原文并给行号。

- 抽取式记忆（EverOS、Mem0）输在细节、归因与更正；
- 结构化旁路只能做“大概在哪一条”，不能替代原文；
- 12 个失败模式里，隐式冲突、口语改写、隐私写入仍未解决。

实验报告与失败记录都在本地仓库 `memory-lab/docs/`，不把没验证的结论写成结论。

### 纯代码视频管线

用 HTML/Canvas 写场景，Playwright 逐帧渲染，FFmpeg 编码；分镜、时长、验收先写成 `SPEC.md`，脚本只消费规范。

- 吃嘛实机演示 6:24.7：手机录屏 + 旁白 + 字幕 + 大字证据卡；
- 宣传片 8s / 32s / 36s：纯代码逐帧，不调用视频生成模型；
- 音色：edge-tts 出标准中文，RVC 换音色，本人试听通过才算交付。

## 技术栈

- 前端：HTML / CSS / 原生 JavaScript，移动端优先，无框架
- AI：Cloudflare Worker 代理，文本 / 营养 / 视觉三类模型，密钥只在服务端
- 数据：PowerShell 采集与清洗，OCR 录入，构建期生成静态 JSON
- 测试：Node.js 裸脚本，冒烟 / 回归 / 集成 / 金文件 / 变异 / 版本隔离
- 视频：Playwright 逐帧、FFmpeg、edge-tts、RVC
- 工具：Reqable 抓包（含 MCP 接入）、GitHub Actions、uv

## 怎么做

AI 全程参与，但把重点放在三件事上：意图对齐、架构可控、全链路可复现。

- **先对齐意图再写代码**：项目从一句 Prompt 开始，输入与输出在那句里就定死
- **关键决策留档**：每个版本的取舍都写进开发日志，包括判断错的地方
- **每次改动都跑测试**：变异测试要求注入缺陷全部被杀死，做不到就不算通过
- **本人验收才算交付**：AI 自测指标只作参考，成品必须自己试用 / 试听通过

## 产品观

每个决策都不靠拍脑袋。

口味档案、档口滑窗、单卡与三卡，来自一份学生问卷；v2.1 的三层防线，来自同学实测时说的三个差评；v2.3 的口味槽位，来自一次“勾了酸甜，推出来一份 2 元的番茄”。

发现问题的那一版，永远比修好它的那一版更值得写。

## 在学

- 数据库与数据结构：把反馈学习从 localStorage 挪到服务端
- 可审计记忆：让“哪条旧结论被推翻、为什么”可查
- 视频工程：把分镜、字幕、音频、验收收进同一份规范

## 联系

- GitHub：[@youcheng10d](https://github.com/youcheng10d)
- 项目问题与建议：[what-to-eat/issues](https://github.com/youcheng10d/what-to-eat/issues)

---

<p align="center"><sub>With the wind, with your heart.</sub></p>
