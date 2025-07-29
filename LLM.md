# 如果重学AI我会怎么学

~~不学，不如学前端就业~~   

## 基础

### 深度学习

**理论**：
- 李宏毅  [【機器學習2022】 - YouTube](https://www.youtube.com/playlist?list=PLJV_el3uVTsPM2mM-OQzJXziCGJa8nJL8)
- 名为机器学习实则是深度学习
- 适合大多数人，老师风趣幽默，钟爱宝可梦，偶有二次元要素
- 课程涵盖从简单MLP到生成模型，强化学习等前沿知识，偶有一些老师个人科研经验的分享，同时课程开设许久，有很多往年的课程(会更深入)可以观看，也有老师的博士生分享一些前沿课题，总的来说是不可多得的入门课程
- 另外的[课程网站 - ML 2022 Spring](https://speech.ee.ntu.edu.tw/~hylee/ml/2022-spring.php)有每节课对应的作业，基本都提供了一个基本的Pytorch风格的训练评估脚本，可以快速上手代码

**代码**：
- 初步深入代码建议通过李沐大神的《动手学深度学习》
- [《动手学深度学习》 — 动手学深度学习 2.0.0 documentation](https://zh.d2l.ai/index.html) 或者 [Dive into Deep Learning — Dive into Deep Learning 1.0.3 documentation](https://d2l.ai/)
	- 注意中文版和英文版有一些不同，有比较充足时间的话推荐英文版
- 动手学深度学习会提供了一个from scratch的模型实现和高级API的实现(涵盖主流高级接口，如Pytorch，Tensorflow等)，以代码为核心讲解深度学习知识，是很不错的代码能力巩固书籍


### 其它

可能需要学习的库  
- numpy: python 数据处理基本库
- pandas: 同上
- matplotlib:可视化基本库
- seaborn: 一个比较好看的可视化基本库
- scikit-learn: 机器学习基本库，有时会用到库里的工具函数

练手项目  
- 李宏毅课程的作业
	- 完全搞懂而且能跟上作业提供的改进建议已经比较充足了
- karpathy [Neural Networks: Zero to Hero - YouTube](https://www.youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ)
	- 难度比较大，从零实现一些常见的网络架构，可以选择一到两个尝试一下。

## 大模型基础

实际上比较难定义什么是大模型基础，所以这里写的内容以大模型知识了解为主  

#### 全局视角 
个人感觉形成一个全局的视角很重要，掌握整个架构和脉络会方便理解后续的发展  
- karpathy科普课两节
	- [Deep Dive into LLMs like ChatGPT - YouTube](https://www.youtube.com/watch?v=7xTGNNLPyMI)
	- [\[1hr Talk\] Intro to Large Language Models - YouTube](https://www.youtube.com/watch?v=zjkBMFhNj_g)
	- 这些课可能没什么内容，但是还是推荐一看，可以形成一个基本的认知。推荐同时看看大神的其它视频
- 比较深入的了解
	- [\[2303.18223\] A Survey of Large Language Models](https://arxiv.org/abs/2303.18223)
	- 高瓴AI box课题组的大语言模型综述，截止写下这些文字已经5000多引用，膜拜
	- 100多页的综述，涵盖大模型相关的大部分知识，包含但不限于数据，架构，预训练，后训练，应用，智能体，幻觉，社会影响等内容，个人感觉值得一读。
	- 由于是综述论文，所以可能有些地方很难看懂，可以是简单浏览+适当记录，如果对这些方向感兴趣再去搜索相关资料
- 如果还想再深入一点
	- 可以尝试复现 著名项目[GitHub - karpathy/nanoGPT: The simplest, fastest repository for training/finetuning medium-sized GPTs.](https://github.com/karpathy/nanoGPT) 
	- 或者简单阅读 llama源码 [transformers/src/transformers/models/llama/modeling\_llama.py at main · huggingface/transformers · GitHub](https://github.com/huggingface/transformers/blob/main/src/transformers/models/llama/modeling_llama.py)


#### 分点深入(简单版) 
- 模型架构
	- 注意力机制(self attention)
		- [Transformer - YouTube](https://www.youtube.com/watch?v=ugWDIIOHtPA)
		- [The Annotated Transformer](https://nlp.seas.harvard.edu/annotated-transformer/)
	- 位置编码
		- [Fetching Title#nk0m](https://kexue.fm/archives/8265)
	- Dense与MoE
		- [Mixture-of-Experts (MoE): The Birth and Rise of Conditional Computation](https://cameronrwolfe.substack.com/p/conditional-computation-the-birth)
		- [Mixture-of-Experts (MoE) LLMs - by Cameron R. Wolfe, Ph.D.](https://cameronrwolfe.substack.com/p/moe-llms)
- 预训练
	- llama3 的预训练(比较简单)
	- [Llama 3.1论文精读 · 2. 预训练数据【论文精读·54】\_哔哩哔哩\_bilibili](https://www.bilibili.com/video/BV1u142187S5/?spm_id_from=333.1387.homepage.video_card.click&vd_source=5485575f3489c27d39534b9a4de59820)
- 后训练
	- llama3 的后训练(比较简单)
	- SFT
	- RLHF
	- [从Llama 3报告出发的一些LLM技术整理 - 知乎](https://zhuanlan.zhihu.com/p/713794852)

可能需要学习的库  
- pytorch-lightning
- accelerate
- transformers


## 大模型进阶？

这个由于知识受限大概也不是进阶，就是再深入了解一些而已  

**分点深入**  
(这里的分类可能不是很合理)  
同样由于知识受限，而且比较前沿，学习需要更多地进行自己的探索，只提供一定的资料  

- 数据
	- llama3 数据处理，deepseek v3数据处理
	- 技术报告
		- [\[2407.21783\] The Llama 3 Herd of Models](https://arxiv.org/abs/2407.21783#:~:text=Modern%20artificial%20intelligence%20%28AI%29%20systems%20are%20powered%20by,natively%20support%20multilinguality%2C%20coding%2C%20reasoning%2C%20and%20tool%20usage.)
		- [\[2412.19437\] DeepSeek-V3 Technical Report](https://arxiv.org/abs/2412.19437)
	- **可能这两篇也不见得十分有参考意义，只是技术报告会是学习数据混合和处理的一个可能起点**
- 模型架构
	- 注意力
		- 注意力机制：FlashAttention
			- [ELI5: FlashAttention. Step by step explanation of how one of… \| by Aleksa Gordić \| Medium](https://gordicaleksa.medium.com/eli5-flash-attention-5c44017022ad)  好文推荐
			- [\[2205.14135v2\] FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness](https://arxiv.org/abs/2205.14135v2)
		- KV cache：MQA，GQA，MLA，PagedAttention(vLLM)
			- [Transformers Optimization: Part 1 - KV Cache \| Rajan Ghimire](https://r4j4n.github.io/blogs/posts/kv/)
			- [Transformers Key-Value Caching Explained](https://neptune.ai/blog/transformers-key-value-caching)
			- [缓存与效果的极限拉扯：从MHA、MQA、GQA到MLA - 科学空间\|Scientific Spaces](https://spaces.ac.cn/archives/10091/comment-page-1)
	- MoE
		- DeepseekMoE
		- [\[2401.06066\] DeepSeekMoE: Towards Ultimate Expert Specialization in Mixture-of-Experts Language Models](https://arxiv.org/abs/2401.06066)
		- 一些如MoE太大放不下怎么办的可能技术
			- [\[2412.14219\] A Survey on Inference Optimization Techniques for Mixture of Experts Models](https://arxiv.org/abs/2412.14219)
- 预训练
	- OpenAI scaling law / Google scaling law
		- [\[2001.08361\] Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361)
		- [\[2001.08361\] Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361)
		- [大模型(一): Scaling Laws - OpenAI 提出的科学法则](https://www.jarvis73.com/2024/06/30/Scaling-Laws-1/)
		- [大模型(二): DeepMind 的 Scaling Laws 有什么不同?](https://www.jarvis73.com/2024/06/30/Scaling-Laws-2/)
	- 并行策略
		- 流水线并行
		- 数据并行
		- 模型并行
		- 张量并行
		- 专家并行
		- ZERO，Megatron等常见框架
	- 量化
		- 超级巨头
- 后训练
	- PPO
	- DPO
		- 疑似已经没人用
	- GRPO
	- test time scaling law
- Infra/MLsys
	- Triton
		- python的高级库，编写python-like的CUDA程序
	- CUDA
		- ~~独一家是吧~~


一些优质博客  
- [科学空间\|Scientific Spaces](https://spaces.ac.cn/)  硬核，很干，强推
- [Lil'Log](https://lilianweng.github.io/)  伟大，无需多言

## 另外的

- 多模态大模型
	- 全模态大模型/any to any 模型可能会是一个注定的方向
	- [Awesome-Multimodal-Large-Language-Models](https://github.com/BradyFU/Awesome-Multimodal-Large-Language-Models)
		- 南大智科 米格小组维护的多模态大模型前沿发展
- RAG
	- 待补充
- Agent
	- [Overview](https://github.com/TIC-DLUT/roadmap/blob/main/Go.md)


## 扩散模型

除了大语言模型之外，强烈推荐学习扩散模型，这同样是生成模型中恢弘的一卷  
相比起大模型，哪怕是相比强化学习，扩散模型拥有**扎实的理论基础，严谨的数学证明，优雅的设计思想**，建议时不时到这个领域看看天才们的角逐。  

#### 入门

#### 常见的入门渠道(这样方便了解历史发展)   
- 先从DDPM开始
	- [\[2006.11239\] Denoising Diffusion Probabilistic Models](https://arxiv.org/abs/2006.11239)
- DDIM
	- [\[2006.11239\] Denoising Diffusion Probabilistic Models](https://arxiv.org/abs/2006.11239)
- Score-based，SDE框架，PF-ODE
	- [\[2011.13456\] Score-Based Generative Modeling through Stochastic Differential Equations](https://arxiv.org/abs/2011.13456)
- Flow Matching
	- [\[2210.02747\] Flow Matching for Generative Modeling](https://arxiv.org/abs/2210.02747)
- Consistency Model
	- [\[2303.01469\] Consistency Models](https://arxiv.org/abs/2303.01469)


#### 可能比较好的入门渠道(这样比较适合上手？)  
- Flow Matching
	- [\[2210.02747\] Flow Matching for Generative Modeling](https://arxiv.org/abs/2210.02747)
- Flow Matching 视角下的Diffusion系列
- Consistency Model
	- [\[2303.01469\] Consistency Models](https://arxiv.org/abs/2303.01469)


#### 看论文可能不是最优解，可以参考一些大神的博客  
- [Flow Matching and Diffusion Models](https://diffusion.csail.mit.edu/) Flow Matching 课程，入门的很好切入点  
- [What are Diffusion Models? \| Lil'Log](https://lilianweng.github.io/posts/2021-07-11-diffusion-models/) 伟大，无需多言
- [Generative Modeling by Estimating Gradients of the Data Distribution \| Yang Song](http://yang-song.net/blog/2021/score/) 宋飏博士，超级大神
- [生成扩散模型漫谈（一）：DDPM = 拆楼 + 建楼 - 科学空间\|Scientific Spaces](https://spaces.ac.cn/archives/9119) 苏神的整个系列，有他自己的理解

### 有趣的应用

**个性化生成**  
- DreamBooth (CVPR best student paper)
	- 关键词与对象绑定
	- [\[2208.12242\] DreamBooth: Fine Tuning Text-to-Image Diffusion Models for Subject-Driven Generation](https://arxiv.org/abs/2208.12242)
- ControlNet (ICCV best paper)  作者是张吕敏，大神
	- ~~二次元生成~~
	- [\[2302.05543\] Adding Conditional Control to Text-to-Image Diffusion Models](https://arxiv.org/abs/2302.05543)
- IP-Adapter
	- 与ControlNet类似
	- [\[2308.06721\] IP-Adapter: Text Compatible Image Prompt Adapter for Text-to-Image Diffusion Models](https://arxiv.org/abs/2308.06721)

