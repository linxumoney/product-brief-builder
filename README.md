# Product Brief Builder：把“想做个功能”变成团队能拍板的决策简报

产品文档最常见的问题不是写得少，而是写了很多背景，却没有说明这次到底要决定什么、哪些是假设、什么不做。

`product-brief-builder` 是一个面向产品经理、创业者和项目负责人的开源 Agent Skill。它把散乱想法压缩成一份决策型产品简报，让设计、研发和业务能快速发现分歧。

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

## 方法参考

本项目独立实现。产品需求结构的问题域参考了 [phuryn/pm-skills](https://github.com/phuryn/pm-skills)，该项目采用 MIT License。本项目没有复制其 PRD 模板、章节结构、示例或文字。

## License

MIT License。
