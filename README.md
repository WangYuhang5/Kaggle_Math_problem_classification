# Kaggle_Math_problem_classification
Kaggle的数学问题分类竞赛代码
第一次完整地参加一次Kaggle的竞赛，受益良多，文件Kaggle_Math_fixed是自己做的最终结果，使用"microsoft/deberta-v3-base"模型，通过同义词替换等数据增强手段，进行全量微调，分割训练集验证集以及早停策略，最终在测试集上得到了0.8507分，排名第72
其余的三个文件是冠军队伍的代码，使用Decoder-only形式的Qwen2.5-14b以及Qwen3-14b的QLoRA微调，在Kaggle的4张L4GPU上进行DDP分布式计算，进行3折的交叉验证，分别跑3个epoch，使用Qwen2.5-0.5b进行超参数的调优，最终得分在0.92左右
