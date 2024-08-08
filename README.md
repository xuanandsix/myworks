# myworks
个人作品集，包括3D视觉，目标检测，语义分割，图像修复，生成，风格迁移等方向

[3D视觉](#3D) [目标检测及语义分割](#classificationANDdetection) [图像修复，生成，风格化](#srANDstyle)

## 3D视觉 <a name="3D"></a>
1、turin机器人无序抓取轴承套圈

（1）套圈检测及点云恢复，位姿估计

识别多个候选套圈
|位姿估计|
| :-: |
|<img src="https://github.com/xuanandsix/myworks/blob/main/images/bizhang/wuxu.gif" height="70%" width="70%">|

p.s. 红色检测框表示待抓取套圈，与下文仿真抓取的套圈一致。

（2）路径规划和避障效果。引导操纵机器人实现任意姿态套圈抓取和放置。同时设计了长杆手抓完成深框抓取。
|仿真效果|
| :-: |
|<img src="https://github.com/xuanandsix/myworks/blob/main/images/bizhang/bizhang.gif" height="50%" width="50%">|

p.s. 因客户现场禁止带手机，无法展示现场真实效果。夹爪模型因供应商原因做了简化处理。


2、fanuc机械人抓取大型轴承套圈

p.s. 红色表示当前最高层套圈优先抓取，绿色表示其余层，基于策略决定下一个抓取的套圈（高亮显示）。
||低亮度套圈|
| :-: |:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/grab/0.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/grab/1.gif" height="100%" width="100%">|
|杂乱场景下|识别倾斜严重无法抓取的套圈（蓝色框）|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/grab/2.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/grab/3.gif" height="100%" width="100%">|


|点云恢复，获得待抓取套圈的位姿|
| :-: |
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/grab/point.png" height="50%" width="50%">|

|工厂真实使用效果展示|
| :-: |
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/grab/grab.gif" height="100%" width="100%">|

清晰流畅视频点击链接下载
 https://github.com/xuanandsix/myworks/blob/main/images/grab/grab.mp4

## 目标检测及语义分割 <a name="classificationANDdetection"></a>
1、轴承滚子计数及混料检测

实例分割获得轴承滚子个数及面积尺寸，判断数目是否正确，是否混入其他型号。
|计数及混料检测|
| :-: |
|<img src="https://github.com/xuanandsix/myworks/blob/main/images/jishu/jishu.gif" height="60%" width="60%">|

2、工业零部件缺陷检测

（1）电池产品部分缺陷检测效果展示

|脏污|表皮破损|起泡|裂纹|
| :-: |:-:|:-:|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/dianchi/0.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/dianchi/1.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/dianchi/2.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/dianchi/3.gif" height="100%" width="100%">|

（2）轴承套圈产品各表面部分缺陷检测效果展示

p.s. 蓝色框为产品表面检测区域，红色框为缺陷检测结果且部分包围框做了外扩

|亮斑|磕碰|未超精|油污|
| :-: |:-:|:-:|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/taoquan/0.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/taoquan/1.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/taoquan/2.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/taoquan/3.gif" height="100%" width="100%">|

|车削、暗斑|暗斑|擦伤|工件停止|
|:-: |:-:|:-: |:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/taoquan/4.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/taoquan/5.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/taoquan/10.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/taoquan/8.gif" height="100%" width="100%">|

（3）凸轮产品表面部分缺陷检测效果展示

|磕伤|毛刺|压伤、磕伤|毛刺、锈|
|:-: |:-:|:-: |:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/tulun/0.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/tulun/1.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/tulun/2.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/tulun/3.gif" height="100%" width="100%">|


(4) 检测系统真实使用效果
|检测系统|
| :-: |
|<img src="https://github.com/xuanandsix/myworks/blob/main/images/taoquan/dv.gif" height="60%" width="60%">|


3、UV打印机视觉定位

双摄像头下视觉定位各种类型手机壳
| 左侧摄像头 | 右侧摄像头 |
| :-: |:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvdeta.gif">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvdetb.gif" >|

对检测区域进行语义分割确定打印区域
|随机展示部分分割结果|||||
|:-:|:-:|:-:|:-:|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvsega.gif" height="60%" width="60%"> |<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvsegb.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvsegc.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvsegd.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvsege.gif" height="60%" width="60%">|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvsegf.gif" height="60%" width="60%"> |<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvsegg.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvsegh.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvsegi.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/uvsegj.gif" height="60%" width="60%">|

|打印效果实物展示|
|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/uvdet/phone.jpg" height=346 width=462>|

4、常用商品抠图

支持30+种常用商品抠图
|马克杯|T恤|抱枕|部分遮挡严重下的T恤|
| :-: |:-:|:-:|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/commodityseg/commoditysega.gif" height="85%" width="85%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/commodityseg/commoditysegb.gif" height="95%" width="95%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/commodityseg/commoditysegc.gif" height="100%" width="100%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/commodityseg/commoditysegd.gif" height="100%" width="100%">|

5、移动端抠图算法

使用更轻量的网络，混合精度训练，结合模型剪枝缩小尺寸，知识蒸馏恢复精度。

检测包括猫头、狗头、人头、猫、狗、人、人脸、汽车、文字9类。
对卡通风格同样适用(第1行2列展示)，紧贴头部的饰品被视为身体的一部分（第2行3列）
||||
| :-: |:-:|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/9clsdeta.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/9clsdetb.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/9clsdetc.gif" height="60%" width="60%">|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/9clsdetd.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/9clsdete.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/9clsdeti.gif" height="40%" width="40%">|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/9clsdetf.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/9clsdetg.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/9clsdeth.gif" height="60%" width="60%">|

与服务端大模型性能对比
|目标检测模型|存储大小|mAP(0.5-0.95)|
|:-:|:-:|:-:|
|服务端大模型|378M(float32)|81.09%|
|移动端模型|1.1M(float16)|73.00%|

抠图包括对猫头、狗头、人头、猫、狗、人体进行分割。包括宠物头、宠物身体、人头、人身体四个语义分割模型。同样对抠图后的头部进行关键点检测用于素材对齐，包括宠物头和人头两个关键点检测。
||||
| :-: |:-:|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/4clssega.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/4clssegc.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/4clssege.gif" height="60%" width="60%">|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/4clssegb.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/4clssegd.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/detseg/4clssegf.gif" height="60%" width="60%">|

与服务端大模型性能对比
|语义分割模型|存储大小|mIOU|
|:-:|:-:|:-:|
|服务端大模型|167M(float32)|96.3%|
|移动端模型|628K(float16)|95.0%|

6、品牌LOGO检测

实现500+类品牌LOGO检测

正常业务场景下效果展示
||||
| :-: |:-:|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodeta.gif" height="80%" width="80%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodetb.gif" height="80%" width="80%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodetc.gif" height="80%" width="80%">|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodetd.gif" height="80%" width="80%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodete.gif" height="80%" width="80%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodetf.gif" height="80%" width="80%">|

复杂业务场景下效果展示
||||
| :-: |:-:|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodetg.gif" height="60%" width="60%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodeth.gif" height="70%" width="70%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodeti.gif" height="80%" width="80%">|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodetj.gif" height="70%" width="70%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodetk.gif" height="70%" width="70%">|<img src="https://github.com/xuanandsix/myworks/raw/main/images/logodet/logodetl.gif" height="80%" width="80%">|


7、智慧餐盘识别检测
|餐厅真实使用效果展示|
|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/platedet/platedet.gif" height="75%" width="75%">|

## 图像修复，生成，风格化 <a name="srANDstyle"></a>
1、宠物头及人头特定风格迁移

支持10种宠物头风格迁移和10种人头风格迁移
||
|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/style/headstylea.gif" height="70%" width="70%">|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/style/headstyleb.gif" height="70%" width="70%">|

对人头风格图进行动画操作，生成不同姿态表情效果
||
|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/style/image_animation.png" height="70%" width="70%">|

2、全景人像风格迁移

支持2种全景人像风格迁移
|||||
|:-:|:-:|:-:|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/style1/panoramastylea.gif" height=300 width=220>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/style1/panoramastyleb.gif" height=300 width=220>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/style1/panoramastylec.gif" height=300 width=220>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/style1/panoramastyled.gif" height=300 width=220>|

3、背景超分及人脸质量增强

支持人脸修复
||||
|:-:|:-:|:-:|
|<img src="https://github.com/xuanandsix/myworks/raw/main/images/facesr/facesra.gif" height=300 width=300>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/facesr/facesrb.gif" height=300 width=300>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/facesr/facesrc.gif" height=300 width=300>|

支持对不包括人脸的场景或动漫风格超分辨率
|||
|:-:|:-:|
<img src="https://github.com/xuanandsix/myworks/raw/main/images/facesr/facesrg.gif" height=320 width=480>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/facesr/facesrf.gif" height=320 width=480>|

4、图像生成
文生图
|LoRA微调||||
|:-:|:-:|:-:|:-:| 
|美式黑白线条|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/3-1.png" height=250 width=250>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/3-2.png" height=250 width=250>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/3-3.png" height=250 width=250>|
|复古卡通|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/4-1.png" height=250 width=250>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/4-2.png" height=250 width=250>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/4-3.png" height=250 width=250>|
|插画风格|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/2-1.png" height=350 width=250>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/2-2.png" height=350 width=250>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/2-3.png" height=350 width=250>|
|饥荒游戏风格|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/0-1.png" height=250 width=250>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/0-2.png" height=250 width=250>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/0-3.png" height=250 width=250>|
|特定人物多风格|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/1-5.png" height=250 width=250>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/1-3.png" height=250 width=250>|<img src="https://github.com/xuanandsix/myworks/raw/main/images/sd/1-4.png" height=250 width=250>|

