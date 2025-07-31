# higgs-audio-windows-OneClick
higgs-audio对话型声音克隆文字转语音合成软件免安装部署一键启动整合包

![](https://raw.githubusercontent.com/aidayang/higgs-audio-windows-OneClick/refs/heads/main/hig.webp)
## Higgs Audio介绍

Higgs Audio v2，这是一个强大的音频基础模型，已基于超过 1000 万小时的音频数据和丰富的文本数据进行预训练。尽管无需后期训练或微调，Higgs Audio v2 凭借其对语言和声学的深度理解，在富有表现力的音频生成方面表现出色。

在EmergentTTS-Eval 测试中，它在“情绪”和“问题”类别上分别比“gpt-4o-mini-tts”取得了75.7%和55.7%的胜率。此外，它在 Seed-TTS Eval 和情感语音数据集 (ESD) 等传统 TTS 基准测试中也取得了最佳性能。此外，该模型还展示了以往系统罕见的功能，包括生成多种语言的自然多说话人对话、旁白过程中的自动韵律调整、使用克隆声音进行旋律哼唱以及同时生成语音和背景音乐。

## Higgs Audio 免安装整合包说明

首先将网盘内的软件压缩包下载到本地电脑上并解压，然后双击启动软件.exe启动。第一次使用的时候软件会自动下载模型文件。如果网络异常无法自动下载模型的话，可以将网盘内的hf.zip压缩包下载到项目文件夹higgs-audio内解压，注意不要有文件夹嵌套情况，文件夹层级结构如：higgs-audio–>hf–>models–bosonai–higgs-

audio-v2-generation-3B-base

待合成文本：就是你想要生成语音的文本内容。如果要生成对话语音的话，请把文本内容保存到txt文档中，然后将txt文档导入到软件中即可。

输入框中直接输入txt文档路径地址，或是鼠标左键按住txt文档拖到软件窗口里就可以把txt文档路径导入到软件。多人对话文本格式如下：


[SPEAKER0] I can't believe you did that without even asking me first!

[SPEAKER1] Oh, come on! It wasn't a big deal, and I knew you would overreact like this.

[SPEAKER0] Overreact? You made a decision that affects both of us without even considering my opinion!

[SPEAKER1] Because I didn't have time to sit around waiting for you to make up your mind! Someone had to act.

参考音频：合成语音想要使用的声音音色，留空的话随机使用已有音色。添加新音色方法：准备一段3-10的wav格式的音频文件，和同文件名的txt文档，txt文档内容为wav音频文本内容。将wav音频和txt文档复制到voice_prompts文件夹内。重启软件就可以在参考音频后面下拉列表中看到添加的声音。鼠标点击列表名字可直接添加到前

面的文本框内，单一说话人就选一个发音人，多人对话的话就选多个发音人，多个发音人之间用英文逗号”,”隔开。

最大tokens：要生成的新令牌的最大数量，整数类型，如2048，

temperature：用于对下一个词元概率进行取模运算的值，小数类型，如1.0，0.3

AISM:是否在系统消息中包含语音提示描述。

块方法：用于对提示文本进行分块的方法。选项有“speaker”（按说话者）、“word”（按单词）。默认情况下，默认为空，如果生成多人对话，请选择speaker。

seed：随机种子，整数类型，如123 ， 56987 等，用于重现相同声音，如何语音合成声音异常的话，可尝试修改seed值，或是设置为-1

场景描述：用于生成的场景描述提示。

具体参数效果可以自己生成音频体验。

视频教程及效果演示：https://www.youtube.com/watch?v=WFoP2paPhVI

## 注意事项
使用前先将英伟达显卡驱动更新到最新版本

英伟达显卡显存不低于6G

软件程序运行路径中请不要有非英文字符及空格

软件只支持Windows 10或11，不支持手机和MAC系统

## 声音克隆及多人对话语音合成软件higgs-audio整合包下载
https://pan.quark.cn/s/98c9872273c3

## 原项目链接
https://github.com/boson-ai/higgs-audio
