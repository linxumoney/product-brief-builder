# Product Brief Builder：AI 产品需求、PRD 与 MVP 决策简报 Skill

产品文档最常见的问题不是写得少，而是写了很多背景，却没有说明这次到底要决定什么、哪些是假设、什么不做。

`product-brief-builder` 是一个面向产品经理、创业者和项目负责人的开源 AI 产品需求与 PRD Agent Skill。它把散乱想法压缩成决策型产品简报，明确用户问题、证据、MVP 范围、验收条件、风险和未决问题。适用于 Codex、Claude Code、Cursor 和 OpenCode 等支持 `SKILL.md` 的工具。

## 默认产出

- 本次要做的决策
- 用户问题与现有证据
- 成功信号和失败信号
- 最小范围与明确不做项
- 关键用户流程和验收条件
- 假设、风险与未决问题

## 使用示例

```text
用 $product-brief-builder 把这个想法整理成产品简报：
我们想给知识库增加 AI 自动分类，但还没确定是否需要人工确认。
```

## 安装

```bash
cp -R skills/product-brief-builder ~/.codex/skills/
```

安装后调用 `$product-brief-builder`。

## 为什么不是又一个 PRD 模板

它不强迫所有项目填写同样的八个章节，也不把未知内容自动补齐。证据不足就标成假设；没有达成共识就列为未决问题。

## 适用场景

- 把一句功能想法整理成产品需求文档或产品简报
- 确定 MVP 第一版做什么、明确不做什么
- 从会议记录、用户反馈和调研中提炼需求
- 为需求评审补齐状态、权限、错误流程和验收标准
- 精简冗长 PRD，突出真正需要团队决定的问题

## 常见问题

### 它生成完整 PRD 还是一页简报？

默认生成可扫描的决策简报。复杂项目可以扩展附录，但主文档始终围绕一个核心决策。

### 证据不完整怎么办？

不会自动补写。已知事实、未经验证的假设和未决问题会分开列出，并给出下一步验证动作。

### 能直接交给研发吗？

当核心流程、关键状态和验收条件已经明确时可以用于评审；技术方案、安全和合规仍需对应专业人员确认。

## 方法参考

本项目独立实现。产品需求结构的问题域参考了 [phuryn/pm-skills](https://github.com/phuryn/pm-skills)，该项目采用 MIT License。本项目没有复制其 PRD 模板、章节结构、示例或文字。

## License

MIT License。

## 商业授权

个人学习、研究、测试和非商业使用可以。商业使用请先联系 **linxu.money@gmail.com** 获得授权，详见 [COMMERCIAL-LICENSING.md](COMMERCIAL-LICENSING.md)。

