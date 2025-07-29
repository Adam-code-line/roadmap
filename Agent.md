## 什么是 agent ？
简单来说，**agent 是一个能够感知环境、做出决策并解决问题的系统**。著名的例子包括 IBM 的深蓝、AlphaGo 等系统，它们分别在 1997 年和 2016 年击败了当时世界一流的国际象棋和围棋高手。  
当前的 AI Agent，狭义上指的是利用大语言模型（LLMs）作为核心，调用外部工具来解决复杂问题的系统。

LLM驱动的Agent的一般框架图：
![the general structure of agent](https://lilianweng.github.io/posts/2023-06-23-agent/agent-overview.png)

## 概述
在以 LLMs 为核心的 Agent 系统中，LLMs 如同 “大脑”，为整个系统提供决策能力，此外还包含以下几个辅助组件：
- Planning 
	- 子任务分解
	- 反思与完善
- Memory
	- 短期记忆
	- 长期记忆
- Tool use
	- 使用工具类的 API 或者自定义工具。
## Planning
- 子任务分解：
	- [CoT](https://arxiv.org/abs/2201.11903)
	- [ToT](https://arxiv.org/abs/2305.10601)
	- [Plan-and-Solve](https://arxiv.org/abs/2305.04091)
- 反思与完善
	- 经典的 [ReAct](https://arxiv.org/abs/2210.03629)
	- [Reflexion](https://arxiv.org/abs/2303.11366)
	- [Chain of Hindsight](https://arxiv.org/abs/2302.02676)
## Memory
记忆机制主要在获取、存储、检索、概括等方面存在差异。
![](https://lilianweng.github.io/posts/2023-06-23-agent/memory.png)
## Tool use
这一功能主要用于扩展 LLMs 的能力范围，以解决相应问题。
给几个简单例子
- RAG
- Search Engine
- OCR
- Simulation Platform
- Web API
以上是简单的工具类型，目前这一领域发展十分迅速。当前已出现不少相关产品，如夸克、豆包的智能搜索，Cursor、Trae 等智能集成开发环境（IDE）等，今年出现的相对突出的工作就是MCP、A2A等。

## 如何学习
- 语言：python
- 调用 LLMs 的方式
	- [LangChain](https://www.langchain.com)
	- 其他类型大模型的 python 包
- [MCP](https://modelcontextprotocol.io/docs/getting-started/intro)
## 实战
- [Dify](https://github.com/langgenius/dify)
- [MetaGPT](https://github.com/geekan/MetaGPT)
- [chatchat](https://github.com/chatchat-space/Langchain-Chatchat)