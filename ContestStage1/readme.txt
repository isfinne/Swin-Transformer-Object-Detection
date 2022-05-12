大赛名称：小样本商标检测挑战赛
赛季名称：初赛
数据说明：
	fewshotlogodetection_round1_train_202204.zip 初赛训练数据（COCO格式）
	fewshotlogodetection_round1_test_202204.zip  初赛测试数据（COCO格式）
是否允许使用外部数据：否
是否允许使用预训练权重：仅限imagenet1k预训练模型，主要考虑包括：
	1. 大部分检测框架mmdetection、paddledetection以及比较经典的算法fasterRCNN、Mask-RCNN、YOLO、SSD系列都是以imagenet的pretrained进行衡量的，也包括大部分检测的文章对比；部分使用VOC、COCO、Objects365、OpenImages仅限于特殊比赛任务，或者文章中SOTA任务的说明。
	2. Few-shot的任务如果把主要精力花在pretrained的获取和加工上，novelty很难说明。
	3. 部分来自于工业界的选手可能获取到更多部分开源的数据集合上，例如CLIP训练的部分caption数据，或者是第七期的OpenBrands数据；
	因此考虑简化步骤到ImageNet的Pretrained，也方便后续regular paper的对比实验和ablation分析