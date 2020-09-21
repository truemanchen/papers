# Facial video-based detection of physical fatigue for maximal muscle activity

## abstract

Physical fatigue reveals the health condition of a person at, for example, health checkup, fitness assessment, or rehabilitation training. 

**身体疲劳可以通过例如健康检查，体能评估或康复训练等方式揭示人的健康状况。**

This study presents an efficient non-contact system for detecting non-localised physical fatigue from maximal muscle activity using facial videos acquired in a realistic environment with natural lighting where subjects were allowed to voluntarily move their head, change their facial expression, and vary their pose. 

**这项研究提出了一种有效的非接触式系统，该系统使用在自然环境下的自然环境下采集的面部视频从最大的肌肉活动中检测非局部性的身体疲劳，在自然光线下，受试者可以自愿移动其头部，改变其面部表情并改变其姿势。**

The proposed method utilises a facial feature point tracking method by combining a ‘good feature to track’ and a ‘supervised descent method’ to address the challenges that originate from realistic scenario.

**所提出的方法利用面部特征点跟踪方法，将“良好的特征跟踪”和“有监督的下降方法”相结合，以应对源自现实场景的挑战。**

 A face quality assessment system was also incorporated in the proposed system to reduce erroneous results by discarding low quality faces that occurred in a video sequence due to problems in realistic lighting, head motion, and pose variation. Experimental results show that the proposed system outperforms video-based existing system for physical fatigue detection.

**面部质量评估系统也被并入提议的系统中，以通过丢弃由于现实照明，头部运动和姿势变化中的问题而在视频序列中出现的低质量面部来减少错误结果。实验结果表明，所提出的系统优于基于视频的现有系统进行身体疲劳检测。**

## introduction

Fatigue is an important physiological parameter that usually describes the overall feeling of tiredness or weakness in human body. 

疲劳是重要的生理参数，通常描述人体的整体疲劳或虚弱感。

Fatigue may be either mental or physical or both [1]. 

疲劳可能是精神上的，也可能是身体上的，或者两者都有[1]。

Mental fatigue is a state of cortical deactivation due to prolonged periods of cognitive activity that reduces mental performance.

由于长时间的认知活动会降低心理表现，因此精神疲劳是皮质失活的状态。

 On the other hand, physical fatigue refers to the declination of the ability of muscles to generate force. 

另一方面，身体疲劳是指肌肉产生力量的能力下降。

Stress, for example, makes people mentally exhausted, while hard work or extended physical exercise can exhaust people physically. 

例如，压力会使人精神疲惫，而艰苦的工作或长时间的体育锻炼会使人的身体疲惫。

Though, mental fatigue is related to cognitive activity, it can occur during a physical activity that comprises neurological phenomenon, for example directed attention as found in the area of intelligent transportation systems [2].

**虽然，精神疲劳与认知活动有关，但它可能发生在包括神经系统现象的体育活动中，例如在智能交通系统领域发现的定向注意力[2]。**

 Unlike mental fatigue that is related to cognitive performance, physical fatigue specifically refers to muscles’ inability to force optimally due to inadequate rest during a muscle activity [1]. 

不同于与认知表现有关的精神疲劳，身体疲劳具体是指肌肉在肌肉活动期间由于休息不足而无法最佳地施加力量[1]。

Physical fatigue occurs from two types of activities: sub-maximal muscle activity (e.g. using a cycle ergometer or motor driven treadmill) and maximal muscle activity (e.g. pressing a dynamometer or lifting a load with great force) [3]. 

身体疲劳是由两种类型的活动引起的：次最大的肌肉活动（例如，使用自行车测功机或机动跑步机）和最大的肌肉活动（例如，按下测功机或用很大的力抬起负荷）[3]。

This kind of fatigue is a significant physiological parameter, especially for athletes or therapists. 

这种疲劳是重要的生理参数，尤其对于运动员或治疗师而言。

For example, by monitoring the occurrence of a patient's fatigue during physical exercise in rehabilitation scenarios, a therapist can change the exercise, make it easier or even stop it if necessary. Estimating the fatigue time offsets can also provide information in posterity health analysis [1].

**例如，在康复情况下，通过监测体育锻炼过程中患者疲劳的发生，治疗师可以改变运动，使其变得更容易，甚至在必要时停止运动。估计疲劳时间偏移量也可以为后代健康分析提供信息[1]。**

A number of video-based non-invasive methods for fatigue detection and quantification have been proposed in the literature.

**文献中已经提出了许多基于视频的非侵入性方法来进行疲劳检测和量化。**

The methods utilised some features and clues, as shown in Fig. 1a, automatically extracted from a subject's facial video and discriminate between fatigue and non-fatigue classes automatically.

**该方法利用了一些特征和线索，如图1a所示，这些特征和线索是从对象的面部视频中自动提取的，并自动区分疲劳和非疲劳类别。**

 For example, the works in [4] use eye blink rate and duration of eye closure for detection of fatigue occurrence due to sleep deprivation or directed attention.

例如，[4]中的工作使用眨眼频率和闭眼持续时间来检测由于睡眠不足或定向注意力引起的疲劳发生。

 In addition to these features head pose and yawning behaviour in facial video is used in [5]. A review of facial video-based fatigue detection methods can be found in [2]. 

除了这些功能之外，[5]中还使用了面部视频中的头部姿势和打哈欠行为。可以在[2]中找到基于面部视频的疲劳检测方法的综述。

However, all of these methods address the detection of mental fatigue occurred from prolonged directed attention activity or sleep deprivation, more specifically known as driver fatigue, instead of physical fatigue occurred from maximal or sub-maximal muscle activity, as shown in Figs. 1b and c. 

**然而，所有这些方法都解决了检测由长期定向注意力活动或睡眠剥夺引起的精神疲劳的问题，更具体地称为驾驶员疲劳，而不是由最大或次最大的肌肉活动引起的身体疲劳，如图1和2所示。 1b和c。**

Most of the available technologies for detecting physical fatigue occurrence (in terms of fatigue time offsets and/or fatigue level) use contact-based sensors such as force gauge, electromyogram (EMG), and mechanomyogram (MMG).

**用于检测物理疲劳发生（就疲劳时间偏移和/或疲劳水平而言）的大多数可用技术都使用基于接触的传感器，例如测力计，肌电图（EMG）和机械功图（MMG）**。

 Force gauge is minimally invasive, but it requires a device like a hand grip dynamometer [6]. EMG uses electrodes which require wearing adhesive gel patches [7]. MMG is based on an accelerometer or goniometer that requires direct skin contact and is sensitive to noise [8]. 

**测力计是微创的，但它需要像手持测功机的设备[6]。 EMG使用需要佩戴粘性凝胶贴片的电极[7]。 MMG基于加速度计或测角计，需要直接与皮肤接触并且对噪声敏感[8]。**

To the best of our knowledge, the only video-based noninvasive system for non-localised (i.e. not restricted to a particular muscle) physical fatigue detection in a maximal muscle activity scenario (as shown in Fig. 1c) is the one introduced in [9] which uses head-motion (shaking) behaviour due to fatigue in video captured by a simple webcam.

据我们所知，唯一在最大肌肉活动情况下（如图1c所示）用于非定位（即不限于特定肌肉）身体疲劳的基于视频的非侵入性系统是[ 9]使用由于简单网络摄像头捕获的视频疲劳而导致的头部运动（抖动）行为。

 It takes into account the fact that muscles start shaking when fatiguing contraction occurs in order to send extra sensation signal to the brain to get enough force in a muscle activity and this shaking is reflected in the face. 

它考虑到了这样的事实，即在发生疲劳性收缩时，肌肉会开始晃动，以便向大脑发送额外的感觉信号，从而在肌肉活动中获得足够的力量，并且这种晃动会反映在面部。

Inspired by [10] for heartbeat detection from ballistocardiogram, in [9] some feature points on the region of interest (ROI) (forehead and cheek) of the subject's face in a video are selected and tracked to generate trajectories of the facial feature points, and to calculate the energy of the vibration signal, which is used for measuring the onset and offset of fatigue occurrence in a non-localised notion. 

受[10]启发从心动描记图进行心跳检测，在[9]中，选择并跟踪了视频中对象面部的感兴趣区域（ROI）（前额和脸颊）上的一些特征点，并进行跟踪以生成面部特征点的轨迹，并计算振动信号的能量，该能量用于测量非局部概念中疲劳发生的开始和偏移。

Though both physical fatigue and mental fatigue can occur simultaneously during a physical activity, the physiological mechanisms are not same. While mental fatigue represents the temporary reduction of cognitive performance, physical fatigue represents temporary reduction of force induced in muscle to accomplish a physical activity [2]. 

尽管在体育活动中身体疲劳和精神疲劳可以同时发生，但其生理机制并不相同。精神疲劳代表认知能力的暂时降低，而身体疲劳代表肌肉中为完成体育活动而产生的力的暂时降低[2]。

Unlike driver mental fatigue, physical fatigue for maximal muscle activity does not necessarily require a prolonged period. Thus, the visual clues found in the case of driver fatigue cannot be found in the case of physical fatigue from maximal muscle contraction. 

与驾驶员的精神疲劳不同，最大程度的肌肉活动所需的身体疲劳不一定需要长时间。因此，在驾驶员疲劳的情况下发现的视觉线索在最大肌肉收缩引起的身体疲劳的情况下找不到。



Changes in facial features in these two different types of fatigue are very different: in the driver mental fatigue eye blinking, yawning, varying head pose, and degree of mouth openness are used (as shown in Fig. 1a), while in the nonlocalised maximal muscle contraction-based physical fatigue headmotion behaviour from shaking is used. 

在这两种不同类型的疲劳中，面部特征的变化是非常不同的：在驾驶员的精神疲劳中，使用眨眼，打哈欠，变化的头部姿势和张开程度（如图1a所示），而在非局部最大使用基于肌肉收缩的身体疲劳摇头动作。

Consequently, physical fatigue occurred from maximal muscle activity cannot be detected or quantised by the computer vision methods used for detecting driver mental fatigue.

因此，无法通过用于检测驾驶员精神疲劳的计算机视觉方法来检测或量化由最大肌肉活动引起的身体疲劳。

We denote internal motion as facial expression and external motion as head pose. 

**我们将内部运动表示为面部表情，将外部运动表示为头部姿势。**

In real-life scenarios there are, of course, both internal and external head motions.

**在现实生活中，当然存在内部和外部头部运动。**

 The current method, therefore, fails due to an inability to detect and track the feature points in the presence of internal and external motion, and low texture in the facial region.

**因此，当前的方法由于在存在内部和外部运动以及面部区域的质地低下时无法检测和跟踪特征点而失败。**

 Moreover, real-life scenarios challenge current methods due to low facial quality in video because of motion blur, bad posing, and poor lighting conditions [11]. 

**此外，由于运动模糊，不良姿势和不良照明条件，视频中的面部质量低下，现实生活中的场景挑战了当前的方法[11]。**

The proposed system in this paper extends [9] by addressing the abovementioned shortcomings and thereby allows for automatic and more reliable detection of fatigue time offsets from facial video captured by a simple webcam. 

**本文提出的系统通过解决上述缺点扩展了[9]，因此可以通过简单的网络摄像头从面部视频中自动，更可靠地检测疲劳时间偏移。**

To address the shortcomings, we introduce a face quality assessment (FQA) method that prunes the captured video data so that low quality face frames cannot contribute to erroneous results [12, 13]. 

为了解决这些缺点，我们引入了面部质量评估（FQA）方法，该方法会修剪捕获的视频数据，以使低质量的面部框架不会导致错误的结果[12，13]。

Following [10, 14], we track feature points (Fig. 2a) through a method good feature to track (GFT) with Kanady–Lucas–Tomasi (KLT) tracker, and then combine these trajectories with 49 facial landmark  trajectories (Fig. 2b), tracked by a supervised descent method (SDM) of [15, 16]. The idea of combining these two types of features has been developed in our paper [17], which was applied to heartbeat estimation from facial video. Here, we look at another application of this idea for physical fatigue estimation. The experiments are conducted on realistic datasets collected at the lab and a commercial fitness centre for fatigue measurement. The paper's contributions are as follows:

[10，14]之后，我们通过一种良好的方法来使用Kanady–Lucas–Tomasi（KLT）跟踪器跟踪特征点（GFT），跟踪特征点（图2a），然后将这些轨迹与49个面部标志性轨迹组合起来（图2a）。 2b），由[15，16]的监督下降方法（SDM）跟踪。结合这两种类型的功能的想法已经在我们的论文中提出[17]，该思想被应用于面部视频的心跳估计。在这里，我们看一下这种想法在物理疲劳估计中的另一种应用。实验是在实验室和商业健身中心收集的用于疲劳测量的真实数据集上进行的。该论文的贡献如下：

i. We identify the limitations of the GFT-based tracking used in previous methods for physical fatigue detection and propose a solution using SDM-based tracking.

**我们确定在以前的方法中用于物理疲劳检测的基于GFT的跟踪的局限性，并提出使用基于SDM的跟踪的解决方案。**

We provide evidence for the necessity of combining the trajectories from the GFT and the SDM, instead of using the trajectories from either the GFT or the SDM.

**ii。我们提供证据表明必须GFT和SDM的轨迹，而不是使用来自GFT或SDM的轨迹。**

iii. We introduce the notion of FQA in the physical fatigue detection context and demonstrate empirical evidence for its effectiveness.

**iii。我们在身体疲劳检测的背景下介绍FQA的概念，并证明其有效性。**

The rest of the paper is organised as follows. Section 2 describes the proposed method. The results are summarised in Section 3. Finally, Section 4 concludes the paper.

**本文的其余部分安排如下。第二节描述了所提出的方法。结果总结在第3节。最后，第4节总结了论文。**

## proposed methods

所提出的方法的框图如图3所示。
以下小节将说明这些步骤。

### 2.1 Face detection and FQA

Automated facial video-based recognition of depression and anxiety symptom severity: cross-corpus validation