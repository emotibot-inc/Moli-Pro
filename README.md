# README

# Moli-Pro

[Hugging Face](https://huggingface.co/emotibot-inc/Moli-Pro) | [GitHub](https://github.com/emotibot-inc/Moli-Pro) | [Model Scope](https://modelscope.cn/models/emotibotinc/Moli-Pro/summary) | [Emotibrain](https://brain.emotibot.com/?source=molipro_github)

# **模型介绍**

魔力-Pro是竹间智能基于超过2亿token的基础语料训练的基础模型。它具备以下特点：
1. 上下文长度：魔力大模型具有强大的上下文理解能力，其上下文长度可以达到4096个token。这意味着它可以处理和理解更长的文本段落，从而在生成或翻译长篇文章时提供更准确的结果。

2. 训练数据：魔力大模型接受了超过100万条人类标注进行训练。这使得该模型能够更好地理解和生成人类语言，提高了其在各种任务中的表现。

3. 模型优化：相比于llama模型，魔力大模型使用了优化的自回归Transformer。这种Transformer使得魔力大模型在处理复杂任务时更加高效。

4. 数据清理和混合更新：为了进一步提升性能，魔力大模型进行了更强大的数据清理，并更新了数据混合。这两项改进都有助于提高模型对输入数据的理解和处理能力，从而产生更准确、质量更高的输出结果。

# Model **benchmark**

## **中文评测** - **CMMLU**

### Result

| Model 5-shot | STEM | Humanities | Social Science | Other | China-specific | Average |
| --- | --- | --- | --- | --- | --- | --- |
| Multilingual-oriented |  |  |  |  |  |  |
| [GPT4](https://openai.com/gpt4) | 65.23 | 72.11 | 72.06 | 74.79 | 66.12 | 70.95 |
| [ChatGPT](https://openai.com/chatgpt) | 47.81 | 55.68 | 56.50 | 62.66 | 50.69 | 55.51 |
| [Falcon-40B](https://huggingface.co/tiiuae/falcon-40b) | 33.33 | 43.46 | 44.28 | 44.75 | 39.46 | 41.45 |
| [LLaMA-65B](https://github.com/facebookresearch/llama) | 34.47 | 40.24 | 41.55 | 42.88 | 37.00 | 39.80 |
| [BLOOMZ-7B](https://github.com/bigscience-workshop/xmtf) | 30.56 | 39.10 | 38.59 | 40.32 | 37.15 | 37.04 |
| [Bactrian-LLaMA-13B](https://github.com/mbzuai-nlp/bactrian-x) | 27.52 | 32.47 | 32.27 | 35.77 | 31.56 | 31.88 |
| Chinese-oriented |  |  |  |  |  |  |
| [Zhuzhi-6B](https://github.com/emotibot-inc/Zhuzhi-6B) | 40.30 | 48.08 | 46.72 | 47.41 | 45.51 | 45.60 |
| [Zhuhai-13B](https://github.com/emotibot-inc/Zhuhai-13B) | 42.39 | 61.57 | 60.48 | 58.57 | 55.68 | 55.74 |
| [Moli-7B](https://github.com/emotibot-inc/Moli-7B) | 28.44 | 29.45 | 31.28 | 32.54 | 28.65 | 30.07 |
| [Moli-Pro](https://github.com/emotibot-inc/Moli-Pro) | 30.2 | 37.5 | 36.22 | 39.71 | 33.55 | 35.44 |
| [Baichuan-13B](https://github.com/baichuan-inc/Baichuan-13B) | 42.38 | 61.61 | 60.44 | 59.26 | 56.62 | 55.82 |
| [ChatGLM2-6B](https://huggingface.co/THUDM/chatglm2-6b) | 42.55 | 50.98 | 50.99 | 50.80 | 48.37 | 48.80 |
| [Baichuan-7B](https://github.com/baichuan-inc/baichuan-7B) | 35.25 | 48.07 | 47.88 | 46.61 | 44.14 | 44.43 |
| [ChatGLM-6B](https://github.com/THUDM/GLM-130B) | 32.35 | 39.22 | 39.65 | 38.62 | 37.70 | 37.48 |
| [BatGPT-15B](https://github.com/haonan-li/CMMLU/blob/master) | 34.96 | 35.45 | 36.31 | 42.14 | 37.89 | 37.16 |
| [Chinese-LLaMA-13B](https://github.com/ymcui/Chinese-LLaMA-Alpaca) | 27.12 | 33.18 | 34.87 | 35.10 | 32.97 | 32.63 |
| [MOSS-SFT-16B](https://github.com/OpenLMLab/MOSS) | 27.23 | 30.41 | 28.84 | 32.56 | 28.68 | 29.57 |
| [Chinese-GLM-10B](https://github.com/THUDM/GLM) | 25.49 | 27.05 | 27.42 | 29.21 | 28.05 | 27.26 |
| Random | 25.00 | 25.00 | 25.00 | 25.00 | 25.00 | 25.00 |

| Model 0-shot | STEM | Humanities | Social Science | Other | China-specific | Average |
| --- | --- | --- | --- | --- | --- | --- |
| Multilingual-oriented |  |  |  |  |  |  |
| [GPT4](https://openai.com/gpt4) | 63.16 | 69.19 | 70.26 | 73.16 | 63.47 | 68.9 |
| [ChatGPT](https://openai.com/chatgpt) | 44.8 | 53.61 | 54.22 | 59.95 | 49.74 | 53.22 |
| [BLOOMZ-7B](https://github.com/bigscience-workshop/xmtf) | 33.03 | 45.74 | 45.74 | 46.25 | 41.58 | 42.8 |
| [Falcon-40B](https://huggingface.co/tiiuae/falcon-40b) | 31.11 | 41.3 | 40.87 | 40.61 | 36.05 | 38.5 |
| [LLaMA-65B](https://github.com/facebookresearch/llama) | 31.09 | 34.45 | 36.05 | 37.94 | 32.89 | 34.88 |
| [Bactrian-LLaMA-13B](https://github.com/mbzuai-nlp/bactrian-x) | 26.46 | 29.36 | 31.81 | 31.55 | 29.17 | 30.06 |
| Chinese-oriented |  |  |  |  |  |  |
| [Zhuzhi-6B](https://github.com/emotibot-inc/Zhuzhi-6B) | 42.51 | 48.91 | 48.85 | 50.25 | 47.57 | 47.62 |
| [Zhuhai-13B](https://github.com/emotibot-inc/Zhuhai-13B) | 42.37 | 60.97 | 59.71 | 56.35 | 54.81 | 54.84 |
| [Moli-7B](https://github.com/emotibot-inc/Moli-7B) | 28.48 | 32.53 | 33.45 | 35.8 | 31.09 | 32.27 |
| [Moli-Pro](https://github.com/emotibot-inc/Moli-Pro) | 30.46 | 36.05 | 37.07 | 38.72 | 32.62 | 34.98 |
| [Baichuan-13B](https://github.com/baichuan-inc/Baichuan-13B) | 42.04 | 60.49 | 59.55 | 56.6 | 55.72 | 54.63 |
| [ChatGLM2-6B](https://huggingface.co/THUDM/chatglm2-6b) | 41.28 | 52.85 | 53.37 | 52.24 | 50.58 | 49.95 |
| [Baichuan-7B](https://github.com/baichuan-inc/baichuan-7B) | 32.79 | 44.43 | 46.78 | 44.79 | 43.11 | 42.33 |
| [ChatGLM-6B](https://github.com/THUDM/GLM-130B) | 32.22 | 42.91 | 44.81 | 42.6 | 41.93 | 40.79 |
| [BatGPT-15B](https://github.com/haonan-li/CMMLU/blob/master) | 33.72 | 36.53 | 38.07 | 46.94 | 38.32 | 38.51 |
| [Chinese-LLaMA-13B](https://github.com/ymcui/Chinese-LLaMA-Alpaca) | 26.76 | 26.57 | 27.42 | 28.33 | 26.73 | 27.34 |
| [MOSS-SFT-16B](https://github.com/OpenLMLab/MOSS) | 25.68 | 26.35 | 27.21 | 27.92 | 26.7 | 26.88 |
| [Chinese-GLM-10B](https://github.com/THUDM/GLM) | 25.57 | 25.01 | 26.33 | 25.94 | 25.81 | 25.8 |
| Random | 25 | 25 | 25 | 25 | 25 | 25 |

# **推理对话**

您可以直接注册并登录竹间智能科技发布的大模型产品 [Emotibrain](https://brain.emotibot.com/?source=molipro_github)，并选择 **CoPilot**（**KKBot**） 进行的在线测试，注册即可立即使用；

![Untitled](./READMEjpg/Untitled.png)

# **模型训练**

您可以直接注册并登录竹间智能科技发布的大模型产品 [Emotibrain](https://brain.emotibot.com/?source=molipro_github)，并选择 Fine-tune 进行 **0 代码微调**，注册即可立即使用；

详细的训练流程您可以浏览此文档：[Emotibrain 快速入门](https://brain.emotibot.com/supports/model-factory/dash-into.html)（大约 5 分钟）

![Untitled](./READMEjpg/Untitled1.png)

![Untitled](./READMEjpg/Untitled2.png)

# **更多信息**

若您想了解更多 大模型训练平台 的相关信息，请访问 [Emotibrain 官网](https://brain.emotibot.com/?source=molipro_github) 进行了解；