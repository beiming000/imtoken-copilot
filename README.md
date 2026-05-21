# 🚀 imToken Copilot: 下一代 AI 驱动智能钱包原型

本演示项目为 **imToken 10 周年“AI 共创：构建你心目中的理想钱包”** 活动参赛作品。

我们通过将 **Gemini 大语言模型的高阶自然语言理解力** 与 **imToken 强大的底层核心技术组件 Token Core** 相结合，实现了“只用大白话，即可安全、顺畅、极低成本与多链网络进行交互”的终极无门槛钱包交互体验。

---

## 💡 设计哲学与解决痛点
1. **彻底告别复杂的区块链术语：** 用户无需理解什么是 L1、L2、Gas 费、路由、跨链桥。AI Copilot 智能理解用户大白话意图。
2. **极速多链 L2 路由优化：** 调用 **Token Core** 底层核心引擎，自主寻找最高效、最便宜的传输和跨链路径，最大幅度节省用户损耗。
3. **安全沙盒预执行机制：** 在用户签名广播前，模拟合约运行状态，进行防地址污染核验与反钓鱼拦截。

---

## 🛠️ 技术栈与实现方案
- **前端架构：** HTML5 单文件极限高保真工程 + Tailwind CSS (极简科技美学) + FontAwesome。
- **AI 智能中枢：** 深度集成 **Gemini 3.1 Flash API**，利用其强大的 **Structured Mime Response & JSON Schema** 特性，将完全非结构化的用户文字百分之百精准转化为可执行的 Web3 Transaction Payload。
- **降级保护：** 即使没有输入 API Key，应用内完备的正则句式解析器也能确保良好的交互性，为评委演示保驾护航。

---

## 🤖 核心 AI 提示词 (Prompts)
我们如何使 Gemini 充当 Token Core 格式化转换器：
```javascript
const systemPrompt = "You are imToken's Token Core AI Routing parser. Extract transaction intentions from the user's plain natural language query. Always output structural properties corresponding to the user's intent.";
// 借助 JSON Schema，限定返回属性仅有 action, token, amount, targetChain...
```
