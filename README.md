# MECR_CCAC2025
Emotion Change Reasoning in Multimodal Dialogues
## 背景介绍
第五届中国情感计算大会将于2025年7月18日至7月20日在四川成都召开，会议由西华大学承办。作为中国中文信息学会（国内一级学会）在情感计算领域的重要会议，CCAC聚焦于文本、语音、图像等各种模态下的情感认知和情感计算，为研讨和传播情感计算领域最新学术和技术成果提供了最广泛的高层次交流平台。

在本届大会中，我们将举办多模态交互中的情感变化推理评测项目。多模态交互中的情感变化推理旨在理解交互过程中目标对象情感变化的多模态影响因素，在自然人机交互、教育、医疗等场景具有广泛的应用。与传统的多模态情感识别任务不同，情感变化推理关注于对交互者情感原因及情感产生过程的深度理解。该任务需要充分挖掘多模态情境当中的情感刺激因素，建模交互者由刺激引发出的认知评价，进而推断出其情感反应。本评测项目鼓励参赛者从不同模态不同角度对多模态对话中的情感变化进行建模和推理，旨在推动多模态交互中情感理解相关研究的发展。

本届多模态交互中的情感变化推理评测由中国中文信息学会情感计算专委会（CIPS-CCAC）主办，中国人民大学AI·M³多媒体计算实验室、启元实验室共同承办，欢迎各界人士参与。

## 评测内容
本届多模态对话中的情感识别评测任务将采用INSIDE (emotIon chaNge reaSoning In multimoDal convErsations) 数据集作为支撑数据集，该任务的任务描述、数据集描述以及评测描述如下。

### 任务描述
本届多模态交互中的情感变化推理评测任务旨在对于多模态交互场景中交互者出现的情感变化情况进行深度理解。任务输入是双人多模态对话片段，包含对话视频、对话文本、每句话的情感状态，此外还会指定出要关注的交互者及其出现情感变化的位置，要求输出该交互者出现对应情感变化的原因，包括多模态的刺激因素，交互者的认知评价以及交互者最终的情感反应。

### 数据集描述
本次技术评测使用的标注数据集为INSIDE数据集，由中国人民大学AI·M³多媒体计算实验室提供，在M3ED数据集的基础上进一步标注而成。INSIDE数据集共计4147个样本，包含丰富的情感互动。我们将发布视频片段所对应的视频信息、文本信息以及对应的标注信息，其中文本信息和标注信息将以JSON格式发布，数据样例如下：

<img width="832" alt="image" src="https://github.com/user-attachments/assets/449e5ab1-4c44-4dcf-910a-1ced8892ed77" />

### 评测描述
本次评测将基于METEOR和BERTScore两项指标的综合排名进行评定。具体方法如下：首先，分别根据METEOR和BERTScore两项指标对所有参赛队伍进行独立排名；然后，将每支队伍在两项指标中的排名位次相加，总和最小的队伍位列前茅。若两支队伍的排名总和相同，则以BERTScore的高低作为最终排序依据，得分较高者优先。
## 报名网站
[多模态交互中的情感变化推理评测报名表](https://docs.qq.com/form/page/DY3hWV0JJZHZKU3BP)

## 注意事项
1.	本评测数据集的视频数据来源于网络，数据集仅限于本次技术评测及学术研究使用，未经许可不能作为商业用途或其他目的。
2.	训练集数据用于模型的学习，验证集和测试集用于模型的效果评测。评测期间将提供训练集和验证集的数据和标签，以及测试集的数据。参赛者在评测期间可以向主办方提交至多5次测试集上的预测结果，以最佳结果为最终成绩。
3.	如需使用本数据集进行课题研究及论文发表，请联系：qjin@ruc.edu.cn。
4.	仅允许使用所有参赛者均可获得的开源代码、工具以及外部数据。
5.	算法与系统的知识产权归参赛队伍所有，要求最终结果排名前5的队伍提供算法代码与系统报告（包括方法说明、数据处理、参考文献和使用开源工具等信息），供会议交流。
6.	本评测联系人：金琴（qjin@ruc.edu.cn）。
## 重要日期
时区：GMT+08:00
| 事项                             | 时间               |
|----------------------------------|--------------------|
| 任务发布与报名启动               | 2025年4月1日       |
| 训练集语料发布                   | 2025年5月上旬      |
| 测试集语料发布                   | 2025年6月上旬      |
| 提交截止                         | 2025年6月中旬      |
| 比赛结果公布                     | 2025年6月下旬      |
| CCAC2025大会召开及颁奖典礼       | 2025年7月18日-20日 |
训练集、验证集数据均已通过报名邮箱发布。

## 评委会成员
-	主席：金琴
-	评测委员会成员：赵金明

## 会务组成员
黄兆培（huangzhaopei@ruc.edu.cn） 张鑫洁（zhangxinjie827@ruc.edu.cn） 吴国正（wuguozheng@ruc.edu.cn)

## 联系方式
如有疑问，请致信评测会务组。

## 参考资料与文献
```bibtex
 @misc{RUCM3ED,  
   author={AIM3-RUC},  
   abstract={M3ED: Multi-modal Multi-scene Multi-label Emotional Dialogue Database. ACL 2022}, 
   year={2022},  
   url={https://github.com/AIM3-RUC/RUCM3ED},
   note={GitHub repository}
}
```

```bibtex
@inproceedings{zhao2022m3ed,
  title={M3ED: Multi-modal Multi-scene Multi-label Emotional Dialogue Database},
  author={Zhao, Jinming and Zhang, Tenggan and Hu, Jingwen and Liu, Yuchen and Jin, Qin and Wang, Xinchao and Li, Haizhou},
  booktitle={Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)},
  pages={5699--5710},
  year={2022}
}
```
## 致谢
- 主办方：中国中文信息学会情感计算专委会
- 承办方：中国人民大学、启元实验室

