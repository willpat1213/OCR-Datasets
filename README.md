# 常用公开数据集整理

Table of Contents

1. [Detection](#Detection-&amp;-Recognition)
   1. [Synthetic Datasets](#Synthetic-Datasets)
      - [x] [SynthText](#SynthText)
   2. [Real Datasets](#Real-Datasets)
      - [x] [Chinese Text in the Wild(CTW)](#Chinese-Text-in-the-Wild)
      - [x] [COCO-TEXT](#COCO-TEXT)
      - [x] [Google FSNS](#Google-FSNS)
      - [x] [ICDAR2015](#ICDAR-2015)
      - [x] [ICDAR2019-ArT](#ICDAR2019-ArT)
      - [x] [ICDAR2019-MLT](#ICDAR2019-MLT)
      - [x] [MSRA-TD500](#MSRA-TD500)
      - [x] [SCUT-CTW1500](#SCUT-CTW1500)
      - [x] [The Uber Text](#The-Uber-Text-dataset)
      - [x] [Total-Text](#Total-Text)

2. [Recognition](#Recognition)
   1. [Synthetic Datasets](#Recog Synthetic Datasets)
      - [x] [Synthetic Datasets](#Synthetic-Datasets)
      - [x] [MJSynth](#MJSynth)
   2. [Real Datasets](#Recog Real Datasets)
      - [x] [CUTE80](#CUTE80)
      - [x] [IIIT5k-Words](#IIIT5k-Words)
      - [x] [Street View Text(SVT)](#Street View Text(SVT))
      - [x] [Street View Text Perspective(SVTP)](#Street View Text Perspective(SVTP))
      - [x] [Synthetic Chinese String](#Synthetic-Chinese-String)
      - [x] [The Chars74K dataset](#The Chars74K dataset)



## Detection & Recognition

### Synthetic Datasets

#### SynthText

1. **描述**：数据集采用自然图像与文本合成的方式生成，经过一些处理使得文字在图片中相对自然。常用作预训练模型。
2. **语言**：English
3. **尺寸**：90k
4. **标注形式**：每个文本实例均使用文本字符串、字级和字符级边界框进行注释。[标注介绍](https://www.robots.ox.ac.uk/~vgg/data/scenetext/readme.txt)
5. **下载链接**：http://www.robots.ox.ac.uk/~vgg/data/scenetext/



### Real Datasets

#### Chinese Text in the Wild

1. **描述**：图像源于腾讯街景，从中国的几十个不同城市中捕捉得到，不带任何特定目的的偏好。包含了平面文本、凸出文本、城市街景文本、乡镇街景文本、弱照明条件下的文本、远距离文本、部分显示文本等。
2. **语言**：Chinese
3. **尺寸**：32k
4. **标注形式**：对每个中文字符，数据集都标注了其真实字符、边界框和 6 个属性以指出其是否被遮挡、有复杂的背景、被扭曲、3D 凸出、艺术化，和手写体等。
5. **下载链接**：https://ctwdataset.github.io/



#### COCO-TEXT

1. **描述**：machine-printed vs. handwritten, legible vs. illgible, and English vs. non-English
2. **语言**：English
3. **尺寸**：63k
4. **下载连接**：https://bgshih.github.io/cocotext/#h2-download



#### Google FSNS

1. **描述**：从法国谷歌街景图片中街区的街道名称标志图片，每个图像包含同一街道名称标志的四个视图。路标上的文字最多可以跨越三行。每一个路标都有一个规范的抄本。
2. **语言**：France
3. **尺寸**：1080k
4. **标注形式**：
5. **下载链接**：http://rrc.cvc.uab.es/?ch=6&com=downloads



#### ICDAR 2015

1. **描述**：自然场景图像(图像分辨率较低)
2. **语言**：English
3. **尺寸**：1.5k, 1k for train, 500 for test.
4. **标注形式**：x1, y1, x2, y2, x3, y3, x4, y4, 顺时针(word-based)
5. **下载链接**：https://rrc.cvc.uab.es/?ch=4&com=downloads



#### ICDAR2019-ArT

1. **描述**：Arbitrary-Shaped Text，任意形状场景文字
2. **语言**：mix
3. **尺寸**：10k
4. **标注形式**：json格式标签，(segmentation-based)
5. **下载链接**：http://rrc.cvc.uab.es/?ch=14



#### ICDAR2019-MLT

1. **描述**：多种混合语言标注的自然场景图片
2. **语言**：Arabic、French、Chinese、German、Korean、Japanese、Italian、Bangladesh、Hindi（1000 per）
3. **尺寸**：10k for train; 10k for text
4. **标注形式**：x1, y1, x2, y2, x3, y3, x4, y4, 顺时针(character-based)
5. **下载链接**：https://rrc.cvc.uab.es/?ch=15&com=evaluation&task=1



#### MSRA-TD500

1. **描述**：以多方向文本和多语种为主要特征的一组自然场景图像，主要以广告牌为背景。
2. **语言**： multi-lingual
3. **尺寸**：total: 500——300 for train, 200 for test
4. **标注形式**：$(x, y, w, h, \theta)$, $(x, y)$表示水平矩形框时左上角的坐标
5. **下载链接**：http://www.iapr-tc11.org/dataset/MSRA-TD500/MSRA-TD500.zip



#### SCUT-CTW1500

1. **描述**：针对弯曲文本检测的数据集
2. **语言**：mainly Chinese & English
3. **尺寸**：1.5k
4. **标注形式**：每行共32个数字，前四个数字为该弯曲文本在整张图上的矩形框坐标值，剩下的28个值为14个点，为相对于矩形框左上角得误差补偿即为与左上角坐标所形成的差值，形成封闭的弯曲文本框(segmentation-based)
5. **下载链接**：https://github.com/Yuliang-Liu/Curve-Text-Detector



#### The Uber Text dataset

1. **描述**：包含了从车载传感器采集的街道级图像和由图像分析团队注释的Ground Truth。
2. **语言**：English
3. **尺寸**：110k
4. **标注形式**：segmentation-based
5. **下载链接**：https://s3-us-west-2.amazonaws.com/uber-common-public/ubertext/index.html



#### Total-Text

1. **描述**：Total-Text是最大弯曲文本数据集之一-ArT（任意形状文本数据集）训练集中的一部分。同时包含水平文本、多方向文本以及曲线文本。
2. **语言**：English & some of Chinese
3. **尺寸**：total: 1.5k, 1255 for train, 300 for test.
4. **标注形式**：word-based
5. **下载链接**：https://drive.google.com/file/d/1bC68CzsSVTusZVvOkk7imSZSbgD1MqK2/view?usp=sharing



## Recognition

### Recog Synthetic Datasets

#### MJSynth

1. **描述**：合成数据集
2. **语言**：Mix
3. **尺寸**：9m
4. **下载链接**
   1. official：http://www.robots.ox.ac.uk/~vgg/data/text/
   2. BaiduNetdisklink(passwd:emco)：https://pan.baidu.com/s/1PBJf-BtFa7mLkltIfTXPhQ

### Recog Real Datasets

#### CUTE80

1. **描述**：数据集包含一些带有歪曲文本的自然图像
2. **语言**：English
3. **尺寸**：80张图像，288个单词实例
4. **下载连接**：http://cs-chan.com/downloads_CUTE80_dataset.html

#### IIIT5k-Words

1. **描述**：该数据集从Google图像搜索中通过使用广告词，广告牌，门牌号，门牌号，电影海报等查询词来收集图像获得的。
2. **语言**：English
3. **尺寸**：5k
4. **下载连接**：http://cvit.iiit.ac.in/research/projects/cvit-projects/the-iiit-5k-word-dataset

#### Street View Text(SVT)

1. **描述**：图像来源自于Google Street View，数据集种的图像包含好质量和低质量的图像，通常低质量图片居多。
2. **语言**：English
3. **尺寸**：249张图像、647个单词实例
4. **下载连接**：http://vision.ucsd.edu/~kai/svt/

#### Street View Text Perspective(SVTP)

1. **描述**：数据集与SVT图像同源，图片大部分带有透视
2. **语言**：English
3. **尺寸**：238张图像、645个单词实例
4. **下载连接**：https://pan.baidu.com/s/1XgtAR6zVWSzblQaoYpJQX

#### Synthetic Chinese String

1. **描述**：数据集采自中国街景，并由街景图片中的文字行区域（例如店铺标牌、地标等等）截取出来而形成。
2. **语言**：Mix
3. **尺寸**：60k
4. **下载连接**：https://aistudio.baidu.com/aistudio/competition/detail/20/0/introduction

#### The Chars74K dataset

1. **描述**：10% for nature scene，5% for hand written，85%for synthetic 
2. **语言**：包括（0-9，A-Z，（a-z）
3. **尺寸**：74k
4. **下载连接**：http://www.ee.surrey.ac.uk/CVSSP/demos/chars74k/

