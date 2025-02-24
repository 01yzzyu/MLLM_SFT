# Awesome-Multimodal-Large-Language-Models-Supervised-Finetuning



## MLLM Preference Training Set

| Dataset | Model | Modality | Quantity | Notes | Link |
|---------|-------|----------|----------|-------|------|
|RLHF-V-Dataset | MiniCPM-V 2.0 | Image | 5.7k | | [RLHF-V-Dataset](https://huggingface.co/datasets/openbmb/RLHF-V-Dataset) |
| RLAIF-V-Dataset | MiniCPM-Llama3-V 2.5 | Image | 83k | | [RLAIF-V-Dataset](https://huggingface.co/datasets/openbmb/RLAIF-V-Dataset) |
| VLFeedback | Silkie | Image | 380k | | [VLFeedback](https://huggingface.co/datasets/MMInstruction/VLFeedback) |
| SPA-VL | SPA-VL-DP | Image | 100k | Safety | [SPA-VL](https://huggingface.co/datasets/sqrti/SPA-VL) |
| MMPR | InternVL2 | Image | 3M | | [MMPR](https://huggingface.co/datasets/OpenGVLab/MMPR) |
| CValues | - | Text | 145k | 开源价值对齐数据集，每个prompt含拒绝&正向建议、拒绝为主、风险回复三种类型，可用于增强SFT模型安全性或训练reward模型 | [CValues](https://github.com/X-PLUG/CValues) |
| GPT - 4 - LLM | - | Text | - | 开源由GPT4生成的多种数据集，含中英PPO数据，可用于奖励模型训练 | [GPT - 4 - LLM](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM) |
| zhihu_rlhf_3k | - | Text | 3k + 条 | 基于知乎问答的人类偏好数据集，每个知乎问题下有赞同数据较高和较低的回答，可用于奖励模型训练 | [zhihu_rlhf_3k](https://huggingface.co/datasets/liyucheng/zhihurlhf3k) |
| hh_rlhf_cn | - | Text | - | 基于Anthropic论文开源的helpful和harmless数据，使用翻译工具翻译 | [hh_rlhf_cn](https://huggingface.co/datasets/dikw/hhrlhfcn) |
| chatbot_arena_conversations | - | Text | - | 偏好数据集含20个LLM输出，包括GPT - 4和Claude - v1等，含先进模型失败案例，来自超13K用户无限制对话 | [chatbot_arena_conversations](https://huggingface.co/datasets/lmsys/chatbot_arena_conversations) |
| UltraFeedback | - | Text | 约64k条提示生成256k个样本 | 大规模、细粒度、多样化的偏好数据集，用于训练奖励模型和批评者模型，从多种资源收集提示，查询多个LLM生成回复 | [UltraFeedback](https://github.com/OpenBMB/UltraFeedback) |


## Pre-Training Dataset
| Dataset | Model | Modality | Quantity | Notes | Link |
|---------|-------|----------|----------|-------|------|
| MNBVC | - | Text | - | 超大规模中文语料集，含主流及小众文化、火星文数据，涵盖多种文本形式，数据源于互联网且持续更新 | [MNBVC](https://github.com/esbatmop/MNBVC) |
| WuDaoCorporaText | - | Text | - | 北京智源人工智能研究院构建，用于支撑大模型训练研究，由文本、对话等四部分组成 | [WuDaoCorporaText](https://data.baai.ac.cn/details/WuDaoCorporaText) |
| CLUECorpus2020 | - | Text | 100GB | 对Common Crawl中文部分语料清洗所得，可用于预训练等任务及简体中文NLP任务小词表 | [CLUECorpus2020](https://github.com/CLUEbenchmark/CLUECorpus2020) |
| WanJuan - 1.0 | - | Text、Image、Video | 超2TB | 书生·万卷多模态语料库首个开源版本，含文本、图文、视频数据集，已应用于书生系列模型训练 | [WanJuan - 1.0](https://opendatalab.org.cn/WanJuan1.0) |
| seq - monkey - data | - | Text | - | 用于训练出门问问序列猴子模型的数据集合，部分数据集向公众开放 | [seq - monkey - data](https://github.com/mobvoi/seq-monkey-data) |


## 🔥 MLLM Supervised Finetuning Dataset

| Dataset | Model | Modality | Quantity | Notes | Link |
|---------|-------|----------|----------|-------|------|
| LLaVA-Instruct-150K | LLaVA | Image | 150k |   | [LLaVA-Instruct-150K](https://huggingface.co/datasets/liuhaotian/LLaVA-Instruct-150K/blob/main/llava_instruct_150k.json)
| LLaVA-Instruct-665K | LLaVA-1.5 | Image | 665k |   | [LLaVA-Instruct-665K](https://huggingface.co/datasets/liuhaotian/LLaVA-Instruct-150K/blob/main/llava_v1_5_mix665k.json)
| CogVLM-SFT-311K | CogVLM | Image | 311k | English & Chinese | [CogVLM-SFT-311K](https://huggingface.co/datasets/THUDM/CogVLM-SFT-311K)
| LLaVA-OneVision-Data | LLaVA-OneVision | Image, Video | 1.6M |   | [LLaVA-OneVision-Data](https://huggingface.co/datasets/lmms-lab/LLaVA-OneVision-Data)
| ShareGPT4V | ShareGPT4V | Image | 1.2M | | [ShareGPT4V](https://huggingface.co/datasets/Lin-Chen/ShareGPT4V)
| ShareGPT4Video | ShareGPT4Video | Video | 4.8M | | [ShareGPT4Video](https://huggingface.co/datasets/ShareGPT4Video/ShareGPT4Video)
| Infinity-MM | Aquila-VL | Image | 34.7M | | [Infinity-MM](https://huggingface.co/datasets/Infinity-MM/Infinity-MM)
| LLaVA-Video-178K | LLaVA-OneVision (SI) | Video | 178k | Generated by GPT-4o | [LLaVA-Video-178K](https://huggingface.co/datasets/lmms-lab/LLaVA-Video-178K)
| M4-Instruct-Data | LLaVA-NeXT-Interleave | Image, Video | 1177.6K | Generated by GPT-4V | [M4-Instruct-Data](https://huggingface.co/datasets/lmms-lab/M4-Instruct-Data)
| InternVL-Chat-V1-2-SFT-Data | InternVL-Chat-V1-2 | Image | 1.2M | | [InternVL-Chat-V1-2](https://huggingface.co/datasets/OpenGVLab/InternVL-Chat-V1-2-SFT-Data)
| Cambrian-10M | Cambrian-1 | Image | 10M | | [Cambrian-10M](https://huggingface.co/datasets/nyu-visionx/Cambrian-10M)

### 中文SFT数据集
| Dataset | Model | Modality | Quantity | Notes | Link |
|---------|-------|----------|----------|-------|------|
| RefGPT | - | Text | RefGPT - Fact：5万中文事实性知识多轮对话；RefGPT - Code：3.9万中文编程相关多轮对话 | 基于RefGPT生成大量真实和定制的对话数据集 | [RefGPT](https://github.com/DA-southampton/RedGPT) |
| COIG | - | Text | - | 维护一套无害、有用且多样化的中文指令语料库，包含多种指令语料库 | [COIG](https://huggingface.co/datasets/BAAI/COIG) |
| generated_chat_0.4M | - | Text | 约40万条 | 由BELLE项目生成的个性化角色对话数据，含角色介绍，由ChatGPT产生，未严格校验 | [generated_chat_0.4M](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M) |
| alpaca_chinese_dataset | - | Text | - | 根据斯坦福开源alpaca数据集中文翻译并再制造对话数据 | [alpaca_chinese_dataset](https://github.com/hikariming/alpaca_chinese_dataset) |
| Alpaca - CoT | - | Text | - | 统一丰富IFT数据、多种训练效率方法及多种LLMs接口，打造LLM - IFT研究平台 | [Alpaca - CoT](https://github.com/PhoebusSi/Alpaca-CoT) |
| pCLUE | - | Text | 120万训练数据 | 基于提示的大规模预训练数据集，用于多任务和零样本学习，含73个Prompt，9个任务 | [pCLUE](https://github.com/CLUEbenchmark/pCLUE) |
| firefly - train - 1.1M | - | Text | 115万 | 23个常见中文数据集，人工书写指令模板保证数据质量与丰富度 | [firefly - train - 1.1M](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M) |
| BELLE - data - 1.5M | - | Text | - | 通过self - instruct生成，使用中文种子任务及openai的text - davinci - 003接口，涉及175个种子任务 | [BELLE - data - 1.5M](https://github.com/LianjiaTech/BELLE/tree/main/data/1.5M) |
| Chinese Scientific Literature Dataset | - | Text | 396,209篇 | 中文科学文献数据集，含中文核心期刊论文元信息及简单prompt | [Chinese Scientific Literature Dataset](https://github.com/ydli-ai/csl) |
| Chinese medical dialogue data | - | Text | <Andriatria_男科>94596个问答对；<IM_内科>220606个问答对；<OAGD_妇产科>183751个问答对；<Oncology_肿瘤科>75553个问答对；<Pediatric_儿科>101602个问答对；<Surgical_外科>115991个问答对，总计792099个问答对 | 中文医疗对话数据集 | [Chinese medical dialogue data](https://github.com/Toyhom/Chinese-medical-dialogue-data) |
| Huatuo - 26M | - | Text | 超2600万个 | 中文医疗问答数据集，涵盖疾病、症状等多方面 | [Huatuo - 26M](https://github.com/FreedomIntelligence/Huatuo-26M) |
| Alpaca - GPT - 4 | - | Text | 50K | 使用self - instruct技术，基于175条中文种子任务和GPT - 4接口生成的指令微调数据集 | [Alpaca - GPT - 4](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM) |
| InstructionWild | - | Text | - | 从网络收集自然指令过滤后结合ChatGPT接口生成指令微调数据集，指令主要来源Twitter、CookUp.AI、Github和Discard | [InstructionWild](https://github.com/XueFuzhao/InstructionWild) |
| ShareChat | - | Text | ChatGPT约九万个对话数据（英文68000，中文11000条，其他各国语言） | 倡议翻译高质量ShareGPT数据，推进国内AI发展，数据最终以CC0协议并入Multilingual Share GPT语料库 | [ShareChat](https://paratranz.cn/projects/6725) |
| Guanaco | - | Text | - | 使用Self - Instruct的多语言（主要中日英德）指令微调数据集 | [Guanaco](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset) |
| chatgpt - corpus | - | Text | 300万 | 开源ChatGPT3.5生成的自问自答数据，涵盖多领域，用于训练大模型 | [chatgpt - corpus](https://github.com/PlexPt/chatgpt-corpus) |
| SmileConv | - | Text | 56k个多轮对话 | 通过ChatGPT改写真实心理互助QA为多轮心理健康支持对话，对话更丰富多样 | [SmileConv](https://github.com/qiuhuachuan/smile) |





