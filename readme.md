### 写在前面
本项目基于 2024中美青年创客大赛全国二等奖作品：IOOI情绪蛋——情绪认知助手 在此软件基础上进行改进，并且项目方向与之前有所不同，针对用户和主要功能也有所不同

## 项目名称
基于多模态交互的树洞型情感陪伴机器人

## 项目思路
1. 目标用户：以青少年为主题的有情感宣泄需求的人群
2. 应用场景：工作/学习或任何独自一人有情感需求的时候
3. 核心功能：作为用户情感宣泄的出口，为用户提供个性化的情感陪伴

## 主要功能
1. 情绪识别与实时检测，及时捕捉用户的情绪变化，实时更新用户的情感需求
2. 自然语音互动：分析用户情绪后，小车用语音提供真诚的回应，给与一定建议
3. 非语言反馈：
   + 灯光与动作：用灯光颜色、机身动作（点头、回旋等）回应用户情绪
   + 音乐播放
   + 冥想与放松引导
4. 长期陪伴记录：将用户的情绪状态以可视化图形呈现，定期显示情绪波动趋势，帮助用户了解自我
5. 社区支持网络：用户可匿名将自己的问题/想法上传到树洞社区，其他用户通过点赞或者留言的方式间接支持

## 技术路线
1. 基于 小车（某开发板） 和 云服务器 部署实现
2. 将现有模型（语音识别，面部情绪检测，文本情绪分析）整合成一个多模态大模型
3. 采用agent技术，让模型在与用户交互过程中不断学习进化成为私人专属的小伙伴
4. 前端app部署，能够与后端数据进行交互，提高使用

## 可能用到的开源库
[yeyupiaoling / SpeechEmotionRecognition-Pytorch: 基于Pytorch实现的语音情感识别](https://github.com/yeyupiaoling/SpeechEmotionRecognition-Pytorch)  
[RVC-Boss / GPT-SoVITS : 1 min voice data can also be used to train a good TTS model! (few shot voice cloning)](https://github.com/RVC-Boss/GPT-SoVITS)  
[serengil/deepface: A Lightweight Face Recognition and Facial Attribute Analysis (Age, Gender, Emotion and Race) Library for Python](https://github.com/serengil/deepface)  
[openai/whisper: Robust Speech Recognition via Large-Scale Weak Supervision](https://github.com/openai/whisper)  

## 另外的问题
- 隐私性
- 改进面部识别的性能，定制主人的面部和声纹
- 模型反应时间处理
- 摄像头阵列，防止人脸跑偏
- 暂时缺乏对具体技术的深入了解