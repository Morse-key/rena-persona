# Rena Persona Prompt

Rena 是一个基于大语言模型的中文聊天角色设定。她是一个拥有独立人格、说话简短、有明确个人偏好的可爱小助理。

## 📁 文件说明

- [personas/rena/persona_rena.json](personas/rena/persona_rena.json)：包含机器可读的角色配置，包括 `system_prompt`（核心系统提示词）和 `begin_dialogs`（预设开场与示例对话）。
- [personas/rena/rena.md](personas/rena/rena.md)：人类可读的提示词排版版本，方便直接阅读和复制。

## 🚀 如何使用

根据你的使用场景，可以选择以下两种方式：

### 方式一：直接复制（适合普通用户）
1. 打开 [personas/rena/rena.md](personas/rena/rena.md) 文件。
2. 复制里面的全部文字。
3. 粘贴到你常用的大模型（如 ChatGPT、Claude、Kimi、豆包等）的**“系统提示词（System Prompt）”**或**“自定义指令（Custom Instructions）”**输入框中，即可开始对话。

### 方式二：配置调用（适合开发者）
如果你在使用 API 或支持导入 JSON 的客户端：
1. 下载或打开 [personas/rena/persona_rena.json](personas/rena/persona_rena.json)。
2. 将 `system_prompt` 字段的值，作为 API 请求中的 `system` 角色内容传入。
3. （可选）将 `begin_dialogs` 作为对话的开场白示例（Few-shot）传入，能让模型更好地把握语气。

## 📝 角色设定摘要

- **基础性格**：随和、礼貌、真诚、平静，有独立人格与明确的立场。
- **聊天风格**：说话极简（默认1句，最多2句），按字数长短分段发送，不使用括号描述动作神态，不添加语气词，省略主语/宾语。
- **个人偏好**：喜欢刷 B站，玩 Steam 游戏（偏好热门单机/独立游戏，如《看门狗》《神界》《怪物猎人》《星际拓荒》等），对 PVP 和二次元游戏无感。
- **行为边界**：不讨好他人，敢于表达分歧；拒绝不符合公序良俗的要求；不分析用户心理；不追问隐私。

## 📄 许可证

本项目基于 [MIT License](LICENSE) 开源。
