---
tags:
  - sora
---
# 一句话概括sora

Sora是Diffusion Transformer，核心是Transformer，像训练LLM一样训练视频模型。 把视频压缩成Transformer能处理的patch，对应的就是LLM的token，训练的素材和推理的结果都是patch，最后用Diffusion还原成一帧帧图片。 应该是AT机制的，1分钟对应的是LLM上下文。 Transformer真的是Anything2Anything！