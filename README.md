# Transformer效率优化
- An Attention Free Transformer: https://arxiv.org/abs/2105.14103

# 多模态Transformers
- E2E-VLP: https://arxiv.org/abs/2106.01804 
- 问题: 论文中transformer decoder generation存在输入信息泄漏
- 潜在提升点: 
   - 提出一个通用的解决视频 和 文本多模态预训练的统一的Framework, 视频Encoder-decoder解决视频相关的任务， 视频是否匹配
   - 图像任务分离, image Encoder-decoder(目标检测, caption generation, 分类等, 把imagenet 的图像label也利用起来),  text任务分离 MLM,  多模态Encoder(image-text matching)
   - 所有可以获取的数据放一起做预训练(COCO/Visual Genome/Conceptual Captions ) 
