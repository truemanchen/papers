This study develops a framework for the detection and analysis of stress/anxiety emotional states through video-recorded facial cues. 

**这项研究开发了一个框架，用于通过视频记录的面部提示来检测和分析压力/焦虑情绪状态。**

A thorough experimental protocol was established to induce systematic variability in affective states (neutral, relaxed and stressed/anxious)through a variety of external and internal stressors. 

**建立了一个详尽的实验规程，以通过各种外部和内部压力源诱发情感状态（中性，放松和压力/焦虑）的系统变异。**

The analysis was focused mainly on non-voluntary and semi-voluntary facial cues in order to estimate the emotion representation more objectively. 

**该分析主要集中于非自愿和半自愿的面部暗示，以便更客观地估计情绪表示。**

Features under investigation included eyerelated events, mouth activity, head motion parameters and heart rate estimated through camera-based photoplethysmography.

**被调查的特征包括与眼睛有关的事件，嘴巴活动，头部运动参数和通过基于照相机的光电容积描记法估计的心率。**

 A feature selection procedure was employed to select the most robust features followed by classification schemes discriminating between stress/anxiety and neutral states with reference to a relaxed state in each experimental phase.

**采用特征选择程序来选择最鲁棒的特征，然后通过分类方案来区分压力/焦虑和中性状态，并参考每个实验阶段的放松状态。**

 In addition, a ranking transformation was proposed utilizing self reports in order to investigate the correlation of facial parameters with a participant perceived amount of stress/anxiety. 

**另外，提出了利用自我报告的等级变换，以调查面部参数与参与者感知到的压力/焦虑量的相关性。**

The results indicated that, specific facial cues, derived from eye activity, mouth activity, head movements and camera based heart activity achieve good accuracy and are suitable as discriminative indicators of stress and anxiety.

**结果表明，源自眼睛活动，嘴巴活动，头部运动和基于照相机的心脏活动的特定面部提示达到了良好的准确性，适合作为压力和焦虑的判别指标。**

# introduction

Stress and anxiety are common everyday life states of emotional strain that play a crucial role in the person’s subjective quality of life. 

压力和焦虑是日常生活中常见的情绪紧张状态，在人的主观生活质量中起着至关重要的作用。

These states consist of several complementary and interacting components (i.e., cognitive, affective, central and peripheral physiological) [1] comprising the organism’s response to changing internal and/or external conditions and demands [2].

**这些状态由几个互补和相互作用的成分（即认知，情感，中枢和外周生理）组成[1]，包括有机体对内部和/或外部条件和需求变化的响应[2]。**

 Historically, the potential negative impact of stress/anxiety on body physiology and health has long been recognized [3]. 

**长期以来，人们已经认识到压力/焦虑对身体生理和健康的潜在负面影响[3]。**

Although stress and, particularly, anxiety are subjective, multifaceted phenomena, which are difficult to measure comprehensively through objective means, more recent research is beginning to throw light on the factors that determine the degree and type of stress/anxiety-related impact on personal health, including characteristics of the stressor itself, and various biological and psychological vulnerabilities. 

**尽管压力，尤其是焦虑是主观的，多方面的现象，很难通过客观手段进行全面测量，但最近的研究开始阐明决定压力/焦虑相关的对个人健康影响程度和类型的因素包括压力源本身的特征以及各种生物学和心理上的脆弱性。**

However,there is evidence that they bear both direct and long term consequences on the person’s capacity to adaptto life events and function adequately, as well as to overall wellbeing [4]. 

**但是，有证据表明，它们对人的适应生活事件和适当功能的能力以及对整体健康的能力既有直接的影响又有长期的影响[4]。**

Stress is often described as a complex psychological, physiological and behavioural state triggered upon perceiving a significant imbalance between the demands placed upon the person and their perceivedcapacity tomeetthosedemands [5,6]. 

**压力通常被描述为一种复杂的心理，生理和行为状态，是在感知到对人的需求与其感知到的满足需求的能力之间的重大不平衡之后触发的[5,6]。**

From an evolutionary standpoint, it is an adaptive process characterized by increased physiological and psychological arousal. 

**从进化的角度来看，这是一个适应性过程，其特征是生理和心理唤醒增加。**

The two key modes of the stress response (“fight” and “flight”) were presumably evolved to enhance the survival capacity of the organism [1,7]. 

**据推测，应激反应的两个关键模式（“战斗”和“飞行”）已经进化为增强生物体的生存能力[1,7]。**

Nevertheless, prolonged stress can be associated with psychological and/or somatic disease [8]. 

**然而，长时间的压力可能与心理和/或躯体疾病有关[8]。**

Anxiety is the unpleasant mood characterized by thoughts of worry and fear, sometimes in the absence of real threat [9,10]. When anxiety is experienced frequently and at intensity levels that appear disproportional to the actual threat level, it can evolve to a broad range of disorders [11,12]. 

**焦虑是一种令人不愉快的情绪，其特点是担心和恐惧，有时甚至没有真正的威胁[9,10]。如果经常经历焦虑并且其强度水平与实际威胁水平不成比例，则焦虑会发展为多种疾病[11,12]。**

It should be noted that the terms stress and anxiety are often used interchangeably. Their main difference is that anxiety is usually a feeling not directly and apparently linked to external cues or objective threats. 

**应当指出，压力和焦虑是经常互换使用的术语。它们的主要区别在于，焦虑通常是一种与外部提示或客观威胁没有直接且明显的联系的感觉。**

On the other hand, stress is an immediate response to daily demands and is considered to be more adaptive than anxiety. Nevertheless, anxiety and stress typically involve similar physical sensations, such as higher heart rate, sweaty palms  and churning stomach [13], triggered by largely overlapping neuronal circuits [9] when the brain fails to distinguish the difference between a perceived and a real threat. 

**另一方面，压力是对日常需求的直接反应，被认为比焦虑更具有适应性。然而，焦虑和压力通常会涉及相似的身体感觉，例如更高的心率，手掌出汗和胃部蠕动[13]，这是由于大脑无法区分感知到的威胁与真实威胁之间的差异而引起的神经元回路重叠[9] 。**

These similarities extend to the facial expressions associated with each state and, accordingly, they were considered as a single state in the present study.

**这些相似性扩展到与每个状态相关的面部表情，因此，在本研究中将它们视为单个状态。**

# 1.1. Physical, mental and cognitive effects of stress/anxiety

Stress and anxiety have impact both on physical and mental health [14]. They are also implicated in the onset and progression of immunological, cardiovascular, circulatory or neurodegenerative diseases [15].

**压力和焦虑对身心健康都有影响[14]。它们也与免疫，心血管，循环系统或神经退行性疾病的发生和发展有关[15]。**

 Evidence from both animal experiments and human studies suggests that stress may attenuate the immune response and increase the risk for certain types of cancer [15].

**动物实验和人体研究的证据都表明，压力可能会减弱免疫反应并增加某些类型癌症的风险[15]。**

 Increased skeletal, smooth and cardiac muscle tension, gastric and bowel disturbances [13] are additional typical signs of stress and anxiety, which are linked to some oftheir most common symptoms and disorders, namely headache, hypertension, exaggeration of lower back and neck pain, and functional gastrointestinal disorders (such as irritable bowel syndrome) [4]. 

**骨骼肌，平滑肌和心肌张力升高，胃和肠功能紊乱[13]是压力和焦虑的其他典型征兆，这与他们最常见的症状和失调有关，例如头痛，高血压，下背部和颈部疼痛的加剧，和功能性胃肠道疾病（如肠易激综合征）[4]。**

These signs are frequently accompanied by restlessness, irritability, and fatigue [12]. From a psychological perspective, prolonged stress and anxiety is often identified as a precipitating factor for depression and panic disorders and may further interfere with the person’s functional capacity through impaired cognition (e.g., memory, attention [16] and decision making [17]). 

**这些体征常伴有躁动，烦躁和疲劳[12]。从心理学的角度来看，长时间的压力和焦虑通常被认为是抑郁和恐慌症的诱发因素，并可能通过认知能力受损（例如，记忆力，注意力[16]和决策[17]）进一步干扰人的功能。**

Stress can be detected through biosignals that quantify physiological measures. Stress and anxiety affect significantly upper cognitive functions [18] and their effects can be observed through EEG recordings [19,20]. Mainly, stress is identified through arousal related EEG features such as asymmetry [20,21], beta/alpha ratio [22] or increased existence of beta rhythm [23]. 

**可以通过量化生理指标的生物信号来检测压力。压力和焦虑会严重影响上层的认知功能[18]，并且可以通过脑电图记录[19,20]观察到它们的作用。主要是通过与唤醒相关的脑电图特征（例如不对称[20,21]，β/α比[22]或β节律的存在增加[23]）来识别压力。**

Stress regulates active sweat glands [24] increasing the skin conductance during stress conditions. Thus, stress can be detected with the use of Galvanic Skin response (GSR) which has been adopted as a reliable psychophysical measure [25,26]. Breathing patterns are also correlated with emotional status and can be used for stress and anxiety detection [27]. 

**压力调节活跃的汗腺[24]，在压力条件下增加皮肤的电导率。因此，可以使用皮肤电反应（GSR）来检测压力，皮肤电反应已被用作可靠的心理物理措施[25,26]。呼吸模式也与情绪状态相关，可用于压力和焦虑感的检测[27]。**

Studies report that respiration rate increases significantly under stressful situations [28]. Additionally, EMG is a biosignal measuring muscle action potentials, where trapezius muscle behaviour is considered to be correlated with stress [29–31]. Finally, speech features are affected in stress conditions [32], the voice fundamental frequency being the most investigated in this research field [33,34].

**研究报告说，在压力情况下，呼吸频率显着增加[28]。另外，肌电图是一种测量肌肉动作电位的生物信号，斜方肌的行为被认为与压力有关[29-31]。最后，语音特征在压力条件下会受到影响[32]，语音基本频率是该研究领域中研究最多的[33,34]。**

# 1.2. Effects of anxiety/stress on the human face

An issue of great interest is the correspondence between information reflected in and conveyed by the human face and the person’s concurrent emotional experience. 

**人们最感兴趣的问题是人脸所反映和传达的信息与人同时发生的情感体验之间的对应关系。**

Darwin argued that facial expressions are universal, i.e. most emotions are expressed in the same way on the human face regardless of race or culture [35].

**达尔文认为面部表情是普遍的，也就是说，无论种族或文化如何，大多数情绪都以相同的方式在人脸上表达[35]。**

 There are several recent studies reporting findings that facial signs and expressions can provide insights into the analysis and classification of stress [34,36,37]. 

**最近有几项研究报告发现面部表情和表情可以提供有关压力分析和分类的见识[34,36,37]。**

The main manifestations of anxiety on the human face involve the eyes (gaze distribution, blinking rate, pupil size variation), the mouth (mouth activity, lip deformations), the cheeks, as well as the behaviour of the head as a whole (head movements, head velocity). 

**人脸焦虑的主要表现包括眼睛（注视分布，眨眼速度，瞳孔大小变化），嘴巴（嘴巴活动，嘴唇变形），脸颊以及整个头部的行为（头部）动作，头部速度）。**

Additional facial signs related to anxiety may include a strained face, facial pallor and eyelid twitching [38]. In reviewing the relevantliterature, facial features of potential value as signs of anxiety and stress states were identified (as listed in Table 1) and are briefly described in this section. 

**与焦虑有关的其他面部症状可能包括紧张的面部，苍白的面部和眼睑抽搐[38]。在回顾相关文献时，识别出潜在价值的面部特征作为焦虑和压力状态的征兆（如表1所示），本节对此进行了简要描述。**

There have been reports that head movements can be used as a stress indicator, although their precise association has not yet been established. It has been reported that head movements during stressful conditions are more frequent [39], more rapid [37] and there is greater overall head motion [40]. 

**有报道称，头部运动可以用作压力指示器，尽管它们的精确关联尚未确定。据报道，在压力条件下头部的运动更为频繁[39]，速度更快[37]，并且头部的整体运动更大[40]。**

In [41] head nods and shakes were employed among other features in order to discriminate complex emotional situations. Regarding the eye region, features like the blink rate, eye aperture, eyelid response, gaze distribution and variation in pupil size have been studied.

 **[41]点头和摇头被用来区分其他复杂的情绪状况。关于眼睛区域，已经研究了眨眼率，眼孔，眼睑响应，凝视分布和瞳孔大小变化等特征。**

 Blinking can be voluntary but also as a reflex to external or internal stimuli and blinking rate typically increases with emotional arousal, including stress and anxiety levels [10,37,42,43]. The blinking rate is affected by various other states, such as lying [44], and disorders such as depression, Parkinson’s disease [45] and schizophrenia [46]. 

**眨眼既可以是自愿的，也可以是对外部或内部刺激的反射，眨眼的频率通常会随着情绪唤起而增加，包括压力和焦虑水平[10,37,42,43]。眨眼率受其他各种状态的影响，例如躺着[44]以及抑郁症，帕金森氏病[45]和精神分裂症[46]等疾病。**

It is also affected by environmental conditions such as humidity, temperature and lighting [47]. The percentage of eyelid closure induced by a light stimulus (increase in brightness) was significantly higher in a group of anxious persons when compared to the corresponding response of non-anxious individuals [48].

**它还受湿度，温度和照明等环境条件的影响[47]。与非焦虑者的相应反应相比，一组焦虑者由光刺激引起的眼睑闭合百分比（亮度增加）明显更高[48]。**

Similarly, gaze direction, gaze congruence and the size of the gaze-cuing effect are influenced by the level of anxiety or stress [49,50]. Persons with higher trait anxiety demonstrate greater gaze instability under both volitional and stimulus-driven fixations [51].

**同样，凝视的方向，凝视的一致性和凝视效果的大小也受焦虑或压力水平的影响[49,50]。性格焦虑较高的人在自愿和刺激驱动的注视下表现出更大的注视不稳定性[51]。**

 Moreover,highlevels of anxiety were foundtodisrupt saccadic control in the antisaccade task [52]. Anxious people tend to be more attentive and to make more saccades toward images of fearful and angry faces than others [53,54]. 

**此外，在反扫视任务中发现高水平的焦虑会破坏对扫视的控制[52]。与其他人相比，焦虑的人倾向于更专心，对恐惧和愤怒的面孔的扫视更多[53,54]。**

Various studies have documented an association between pupil diameter and emotional, sexual or cognitive arousal. In addition, pupil dilation can be employed as an index of higher anxiety levels [55,56].

**各种研究已证明瞳孔直径与情绪，性或认知唤醒之间存在关联。另外，瞳孔扩张可以用作焦虑程度较高的指标[55,56]。**

 Pupillary response to negatively valenced images also tends to be higher among persons reporting higher overall levels of stress [57]. Pupil size may also increase in response to positive, as well as negative arousing sounds as compared to emotionally neutral ones [58]. 

**在总体压力水平较高的人群中，瞳孔对负价图像的反应也往往较高[57]。与情绪中立的人相比，学生对正向和负向唤醒声音的反应也可能会增加[58]。**

There is also sufficient evidence in the research literature that mouth-related features, particularly lip movement, are affected by stress/anxiety conditions [37]. Asymmetric lip deformations have been highlighted as a characteristic of high stress levels [59]. 

**在研究文献中也有足够的证据表明，与口有关的特征，特别是嘴唇运动，受压力/焦虑状况的影响[37]。非对称唇形变形已被强调为高应力水平的特征[59]。**

In addition, it was found [60] that the frequency of mouth openings was inversely proportionalto stress level, as indexed by higher cognitive workload. A technique designed to detect facial blushing has been reported and applied to video recording data [61] concluding that blushing is closely linked to anger-provoking situations and pallor to feelings of fear or embarrassment. 

**另外，发现[60]，张口的频率与压力水平成反比，这是由较高的认知负荷所指示的。已经报道了一种旨在检测脸部红晕的技术，并将其应用于视频记录数据[61]，认为红晕与发怒的情况密切相关，而与恐惧或尴尬的感觉则微弱。**

The heart rate has also an effect on the human face, as facial skin hue varies in accordance to concurrent changes in blood volume transferred from the heart. There is the general notion in the literature that the heart rate increases during conditions of stress or anxiety [62–66] and that heart rate variability parameters differentiates stress and neutral states [66–68].

**心率也会对人脸产生影响，因为面部皮肤的色调会根据同时从心脏转移的血量变化而变化。文献中有一个普遍的概念，即在压力或焦虑状态下心率会增加[62-66]，而心率变异性参数会区分压力和中立状态[66-68]。**

 Finally, there are approaches that aim to detect stress through facial actions coding. The most widely used coding scheme in this contextis the Emotional FacialAction Coding System (EMFACS)[69]. This coding was used to determine facial manifestations of anxiety [10], to classify (along with cortisol, cardiovascular measures) stress responses [70] and to investigate deficits in social anxiety [71].

**最后，有一些方法旨在通过面部动作编码来检测压力。在这种情况下，使用最广泛的编码方案是情绪面部动作编码系统（EMFACS）[69]。该编码用于确定焦虑的面部表现[10]，分类（以及皮质醇，心血管指标）应激反应[70]和调查社交焦虑的不足[71]。**

# 1.3. Procedural issues of the available literature

Most of the relevant literature focuses on the automatic classification of basic emotions [72] based on the processing of facial expressions. Reports on stress detection are fewer, typically employing images [53,54,73], sounds [58], threats [51] or images mimicking emotions [74] as stressful stimuli. 

**大多数相关文献集中在基于面部表情处理的基本情绪的自动分类上[72]。关于压力检测的报道较少，通常使用图像[53,54,73]，声音[58]，威胁[51]或模仿情绪的图像[74]作为压力刺激。**

Results of some of these studies are often confounded by variability in stimulation conditions, e.g. videos with many colours and light intensity variations, which are known to affect the amplitude of pupillary responses. Perhaps more important with respect to the practical utility of automatic detection techniques is the validity ofthe experimental setup employed. 

**这些研究中的某些结果通常会因刺激条件的变化而混淆，例如：具有许多颜色和光强度变化的视频，这些视频会影响瞳孔反应的幅度。关于自动检测技术的实用性，也许更重要的是所采用的实验装置的有效性。**

Well-controlled laboratory conditions are necessary in the early phases of research in order to select pertinent facialfeatures and optimize detection and classification algorithms. These settings are, however, far from real-life conditions in which anxiety and stress are affected by a multitude of situational factors, related to both context and cognitive-emotional processes taking place within the individual and determining the specific characteristics and quality of anxiety and accompanying feelings (fear, nervousness, apprehension, etc.) [75].

**为了选择相关的面部特征并优化检测和分类算法，在研究的早期阶段必须对实验室条件进行良好控制。但是，这些设置远非现实生活中的情况，在这种情况下，焦虑和压力会受到多种情境因素的影响，这些情境因素与个体内发生的情境和认知情感过程有关，并决定着焦虑和情绪的特定特征和质量。伴随的感觉（恐惧，紧张，担忧等）[75]。**

# 1.4. Purpose of the paper

The work reported in this manuscript focuses on the automated identification of a set of facial parameters (mainly semi- or/and non-voluntary) to be used as quantitative descriptive indices in terms of their ability to discriminate between neutral and stress/anxiety state. 

**该手稿中报道的工作着重于自动识别一组面部参数（主要是半自愿或/和非自愿的），以区分中性和压力/焦虑状态作为定量的描述指标。**

In support of this objective, a thorough experimental procedure has been established in order to induce affective states (neutral, relaxed and stressed/anxious) through a variety of external and internal stressors designed to simulate a wide range of conditions. An emotion recognition analysis workflow used is presented in Fig. 1. 

**为了支持这个目标，已经建立了一个全面的实验程序，以通过设计用于模拟各种条件的各种外部和内部压力源来诱导情感状态（中性，放松和压力/焦虑）。图1中显示了使用的情绪识别分析工作流。**

The advantages of the present study relate to the fact that (a) a variety of semi voluntary facial features are jointly used for the detection of anxiety and/or stress instead of the traditional facial expression analysis, (b) the experimental protocol consists of various phases/stressful stimuli covering different aspects of stress and anxiety, and (c) the facial features that are involved in stress/anxiety states for different stimuli are identified through machine learning techniques.

**本研究的优势与以下事实有关：（a）代替传统的面部表情分析，将各种半自愿的面部特征联合用于检测焦虑和/或压力，（b）实验方案包括各种涵盖压力和焦虑不同方面的阶段/压力刺激，以及（c）通过机器学习技术识别参与不同刺激的压力/焦虑状态的面部特征。**

# 2.1. Experimental setup

Study participants were seated in front of a computer monitor while a camera was placed at a distance of approximately 50 cm with its field of view (FOV) able to cover properly the participant’s face. At the start of the procedure, participants were fully informed about the details of the study protocol and the terms “anxiety” and “stress” were explained in detail. The experimental setup is shown in Fig. 2.

**研究参与者坐在计算机显示器前，同时将相机放置在大约50厘米的距离内，其视场（FOV）能够正确覆盖参与者的脸部。在程序开始时，参与者会充分了解研究方案的详细信息，并详细解释了“焦虑”和“压力”这两个术语。实验设置如图2所示。**

The equipment included a colour video camera placed on a tripod behind and above the pc monitor. Diffused lightning was generated by two 500W spotlights covered with paper. A checkerboard of 23-mm square size was used to calibrate the pixel size in calculating actual distances between facial features.

**该设备包括一台彩色摄像机，该摄像机放置在PC显示器前后的三脚架上。两个覆盖纸的500W聚光灯产生了弥散的闪电。在计算面部特征之间的实际距离时，使用23毫米见方的棋盘格来校准像素大小。**

# 2.2. Experimental procedure

The ultimate objective of the experimental protocol was to induce affective states (neutral, relaxed and stressed/anxious) through a variety of external and internal stressors designed to simulate a wide range of everyday life conditions. A neutral (reference) condition was presented at the beginning of each phase of the experiment as listed in Table 2.

**该实验方案的最终目的是通过设计用于模拟各种日常生活条件的各种外部和内部压力源来诱发情感状态（中性，放松和压力/焦虑）。如表2所示，在实验的每个阶段开始时都显示了中性（参考）条件。**

# 2.2.1. Social exposure phase

A social stressor condition was simulated by asking participants to describe themselves in a foreign language having its origin in the stress faced by an actor when he/she is at the stage. There is reported evidence that people talking a foreign language become more stressed [76].A third condition in the exposure phase entailed reading aloud an 85 word emotionally neutral literary passage. 

**通过要求参与者用外语描述自己来模拟社交压力源，这种外语源于演员在舞台上所面对的压力。有证据表明，说外语的人变得更加紧张[76]。暴露阶段的第三个条件是要朗读一个85字的情感中性文学作品。**

The latter aimed to induce moderate levels of cognitive load and was similar to the self-describing task, in the sense that both required overt speech.

**后者的目的是引起中等水平的认知负荷，并且类似于自我描述的任务，因为两者都需要公开讲话。**

# 2.2.2. Emotion recall phase

Negative emotions that resemble acute stress and anxiety were elicited by asking participants to recall and relive a stressful and an anxiety eliciting event from their past life as if it was currently happening.

**通过要求参与者回忆并重温过去生活中的压力和焦虑诱发事件，就好像当前正在发生那样，从而引起类似于急性压力和焦虑的负面情绪。**

# 2.2.3. Stressful images/mental task phase

Neutral and unpleasant images from the International Affective Picture System (IAPS) [77] were used as affect generating stimuli. Stimuli included images having stressful content such as human pain, drug abuse, violence against women andmen, armed children, etc. 

**来自国际情感图片系统（IAPS）的中性和令人不快的图像[77]被用作产生情感的刺激。刺激包括具有压力内容的图像，例如人的痛苦，药物滥用，对妇女和男子的暴力行为，武装儿童等。**

Each image was presented for 15 s. Higher levels of cognitive load were induced through a modified Stroop colour-word reading task, requiring participants to read colour names (red, green, and blue) printed in incongruous ink (e.g., the word RED appearing in blue ink) [78]. In the present task, difficulty was increased by asking participants to first read each word and then name the colour of the word.

**每个图像显示15秒钟。通过改进的Stroop彩色单词阅读任务可以诱导更高水平的认知负荷，要求参与者阅读以不协调的墨水（例如，红色的单词出现在蓝色的墨水中）打印的颜色名称（红色，绿色和蓝色）[78]。在当前任务中，要求参与者先阅读每个单词，然后命名单词的颜色，从而增加了难度。**

# 2.2.4. Stressful videos phase

Finally,three 2-min video segments were presented in attempting to induce low-intensity positive emotions (calming video), and stress/anxiety (action scene from an adventurefilm or scene involving heights to participants who indicated at least moderate levels of acrophobia, and a burglary/home invasion while the inhabitant is inside).

**最后，展示了3个2分钟的视频片段，以尝试诱发低强度的积极情绪（镇定视频）和压力/焦虑（从冒险电影或涉及身高的动作场景到参与者表示至少中等程度的恐高症的动作场景，以及居民在里面时发生盗窃/家庭入侵）。**

# 2.3. Data description

The participants in our study were 23 adults (16 men, 7 women) aged 45.1 ± 10.6 years. The study was approved by the NorthWest Tuscany ESTAV (Regional Health Service, Agency for the Technical-Administrative Services of Wide Area) Ethical Committee.

**我们的研究对象是23位成人（16位男性，7位女性），年龄45.1±10.6岁。该研究得到西北托斯卡纳ESTAV（区域卫生服务，广域技术管理服务局）伦理委员会的批准。**

 All participants gave informed consent. The clinical protocol described in Section 2.2 was applied, which lead to the generation of 12 videos (3 neutral, 8 anxiety/stress and 1 relaxed states) for each participant. Videos were sampled at 50 fps with a resolution of 526 × 696 pixels. The duration of these videos ranged between 0.5, 1 and 2 min as described in Table 2. After the end of tasks 3.1, 4.2, 4.3, and 4.4 participants were asked to rate the level of stress they experienced during the preceding video/image on a scale of 1 (very relaxed) to 5 (very stressful).

**所有参与者均表示知情同意。应用了第2.2节中描述的临床方案，从而为每个参与者生成了12个视频（3个中性，8个焦虑/压力和1个放松状态）。视频以50 fps采样，分辨率为526×696像素。如表2所述，这些视频的持续时间介于0.5、1和2分钟之间。在任务3.1、4.2、4.3和4.4结束后，要求参与者对他们在上一个视频/图像上经历的压力水平进行评分。从1（非常放松）到5（非常紧张）的等级。**

# 2.4. Data preprocessing

Video pre-processing involved histogram equalization for contrast enhancement, face detection, and region of interest (ROI) determination.

**视频预处理涉及直方图均衡化，用于对比度增强，面部检测和感兴趣区域（ROI）确定。**

##  2.4.1. Face ROI detection

 Face detection is a fundamental step of facial analysis via image/video recordings. It is an essential pre-processing step for facial expression and face recognition, head pose estimation and tracking, face modelling and normalization [79,80]. Early face detection algorithms can be classified into knowledge based, feature invariant, template matching, and appearance based. 

**人脸检测是通过图像/视频记录进行人脸分析的基本步骤。这是面部表情和面部识别，头部姿势估计和跟踪，面部建模和规范化的重要预处理步骤[79,80]。早期的面部检测算法可分为基于知识的，特征不变的，模板匹配的和基于外观的。**

These methods used different features, such as integrating edge, colour, size, and shape information and different modelling and classification tools, including mixture of Gaussians, shape templates, active shape models (ASM), eigenvectors, hidden Markov models (HMM), artificial neural networks (ANN), and support vector machines (SVM)[79].

**这些方法使用了不同的功能，例如整合边缘，颜色，大小和形状信息，以及使用不同的建模和分类工具，包括混合高斯，形状模板，活动形状模型（ASM），特征向量，隐马尔可夫模型（HMM），人工神经网络（ANN）和支持向量机（SVM）[79]。**

It appears thatthe last category of appearance based methods were the most successful [80]. Modern approaches of face detection are based on the Viola and Jones algorithm [81] which is widely adopted in the vast majority of real-world applications. This algorithm combines simple Haar-like features, integral images,the AdaBoost algorithm, and the attention cascade to significantly reduce computational load. Several variants of the original Viola and Jones algorithm are presented in [82].

**看起来基于外观的方法的最后一类是最成功的[80]。现代人脸检测方法基于Viola和Jones算法[81]，该算法已在绝大多数实际应用中广泛采用。该算法结合了简单的类似Haar的特征，完整的图像，AdaBoost算法和注意级联，从而大大减少了计算量。原始的Viola和Jones算法的几种变型在[82]中提出。**

# 2.5. Active appearance models



Active appearance models (AAM) [83,84] have been widely applied towards emotion recognition and facial expression classification, as they provide a stable representation of the shape and appearance of the face. In the present work, the shape model was built as a parametric set of facial shapes, described as a set of L landmarks ∈ R2 forming a vector of coordinates

**主动外观模型（AAM）[83,84]已被广泛应用于情感识别和面部表情分类，因为它们提供了面部形状和外观的稳定表示。在本工作中，将形状模型构建为面部形状的参数集，描述为形成坐标矢量的L个地标∈R2的集合**

A mean model shape s0 was formed by aligning face shapes through Generalized Procrustes Analysis (GPA) [85]. Alignment of two shapes S1 and S2 was performed by finding scale, rotation and translation parameters that minimize the Procrustes distance metric

**平均模型形状s0是通过广义Procrustes分析（GPA）对齐面部形状而形成的[85]。通过找到使Procrustes距离度量最小化的比例，旋转和平移参数来执行两个形状S1和S2的对齐**

For every new alignment step the mean shape was re-computed and the shapes were aligned again to the new mean. This procedure was iterated untilthe mean shape did not change significantly. Then, Principal Components Analysis (PCA) was employed projecting data onto an orthonormal subspace in order to reduce data dimension. According to this procedure, a shape s can be expressed as

**对于每个新的对齐步骤，均会重新计算平均形状，然后将形状再次对齐为新的均值。重复该过程，直到平均形状没有明显改变为止。然后，采用主成分分析（PCA）将数据投影到正交子空间上，以减小数据量。根据此过程，形状s可以表示为**

$$s=s_{0}+\sum p_{i} s_{i}$$

where s0 is the mean model shape and pi the model shape parameters. The appearance model was built as a parametric set of facial textures. A facial texture A of m pixels was represented by a vector of intensities gi

**其中s0是平均模型形状，pi是模型形状参数。外观模型被构建为面部纹理的参数集。 m个像素的面部纹理A由强度gi的向量表示**

$$A(x)=\left[g_{1} g_{2} \cdots g_{m}\right]^{T} \forall x \in S_{0}$$

Likewise the shape model was based on the mean appearance A0 and the appearance images Ai which were computed by applying PCA to a set of shape normalized training images. Each training image was shape normalized by warping the training mesh onto the base mesh s0 [84]. Following PCA, textures Ai can be expressed as

**同样，形状模型基于平均外观A0和外观图像Ai，这是通过将PCA应用于一组形状归一化训练图像来计算的。通过将训练网格扭曲到基础网格s0上，可以对每个训练图像进行形状归一化[84]。在PCA之后，纹理Ai可以表示为**

$$A(x)=A_{0}(x)+\sum \lambda_{i} A_{i}(x)$$

where A0(x) is the mean model appearance and i the model appearance parameters. When the model is created, it was fitted to new images or video sequences I by identifying the shape parameters pi and appearance parameters i that produced the most accurate fit. This nonlinear optimization problem aims to minimize the objective function

**其中A0（x）是平均模型外观，而i是模型外观参数。创建模型后，通过识别产生最精确拟合的形状参数pi和外观参数i，将其拟合到新的图像或视频序列I。这个非线性优化问题旨在最小化目标函数**

$$\sum_{x}\left[I(W(x ; p))-A_{0}(W(x ; \Delta p))\right]^{2} \forall x \in s_{0}$$

where W is the warping function. This minimization was performed using the inverse compositional image alignment algorithm [84].

**其中W是warp函数。使用逆构图图像对齐算法进行这种最小化[84]。**

remove artefactual spikes  去除人工峰值

For interpretation of the references to colour in this figure legend, the reader is referred to the web version of this article

# 3.1. Facial feature/cue extraction

# 3.1.1. Eye related features

Time series were detrended and filtered in order to remove artefactual spikes introduced when the model occasionally loses its tracking and to smooth highly varying segments. The average aperture aggregated over the entire time mean value of this time series determines the mean eye aperture that served as a feature in subsequent analyses

**对时间序列进行了去趋势分析和滤波，以消除模型偶尔失去跟踪时引入的人为峰值，并平滑变化较大的片段。在此时间序列的整个时间平均值上聚合的平均孔径确定了在随后的分析中充当特征的平均孔径**

A second eye-related feature, the number of blinks per minute, was extracted from the same timeseries. Each eye blink can be seen as a sharp aperture decrease as shown in Fig. 3. Detection of possible troughs was performed through signal’s derivative [90].

**从同一时间序列中提取出第二个与眼睛相关的功能，即每分钟眨眼次数。如图3所示，每一次眨眼都可以看作是光圈的急剧减少。通过信号的导数[90]来检测可能的波谷。**

 Then peak detection criteria [91] were applied based on the parameters of peak SNR, first derivative amplitude (peak slope), peak distance, peak duration to filter small peaks and select only timeseries sharp decreases as shown in the right panel of Fig. 3. Especially, the minimum peak duration parameter was setto 100 msec (corresponding to 5 consecutive data points) given that an eye blink typically lasts between 100 and 400 msec. 

**然后，根据峰值SNR，一阶导数幅度（峰值斜率），峰值距离，峰值持续时间的参数应用峰值检测标准[91]，以过滤小峰值并仅选择时间序列急剧下降，如图3右图所示。特别地，假设眨眼通常持续在100到400毫秒之间，则最小峰值持续时间参数被设置为100毫秒（对应于5个连续的数据点）。**

Data normality was checked in all experimental phases and tasks. Extreme value analysis was applied to the data excluding one participant who, upon visual inspection ofthe video recordings showed stereotypical movements (tics) involving the upper facial musculature. 

**在所有实验阶段和任务中检查数据的正常性。对数据进行了极值分析，排除了一名参与者，该参与者在对录像进行视觉检查时显示出涉及上面部肌肉组织的定型运动（抽动）。**

Repeated measures of one-way ANOVA [92] was used to compare eye related features (blinks, aperture) across tasks separately for each experimental phase. The results are presented in Table 3. Results indicate increased blink rate under stressful situations compared to the corresponding neutral or relaxed state. 

**单向方差分析[92]的重复测量用于比较每个实验阶段跨任务的与眼睛相关的特征（眨眼，光圈）。结果显示在表3中。结果表明与相应的中性或放松状态相比，在压力情况下眨眼速率增加**。

Specifically, statistically significant increased blink rate was found in the self-description (p < 0.05), the stressful event recall task (p < 0.01), and psychological pressure video viewing (p < 0.01).

**具体而言，在自我描述（p <0.05），压力事件回忆任务（p <0.01）和心理压力视频观看（p <0.01）中发现了统计上显着增加的眨眼率。**

 Stressful images viewing task was also associated with significantly increased blink rate (p < 0.05). On the other hand, eye blink frequency was reduced significantly (p < 0.01) during text reading, and increased during the Stroop colour-word task (both involved word reading). 

**高压的图像查看任务还与眨眼率显着增加相关（p <0.05）。另一方面，在阅读文本期间，眨眼频率显着降低（p <0.01），而在Stroop彩色单词任务期间（两者都涉及单词阅读），眨眼频率增加。**

Thus it appears that increased cognitive effort per se was associated with increased blinking rate, whereas reading a continuous text for comprehension may require persistent attention and increased saccadic activity. Mean eye aperture was increased in stressful situations (text reading and adventure/heights video viewing).

**因此，似乎增加的认知努力本身与增加的眨眼速度有关，而阅读连续的文本以进行理解可能需要持续的注意力和增加的扫视活动。在紧张的情况下（文本阅读和冒险/身高视频观看），平均眼圈增加了。**

## 3.1.2. Mouth related features

From the maximum magnitude signal in the mouth ROI (cf. Section 2.6)the following features were extracted:the variance oftime intervals between adjacent peaks (VTI), the energy ratio (ENR) of the autocorrelation sequence which was calculated as the ratio of the energy contained by the last 75% of the samples of the autocorrelation sequence to the energy contained by the first 25%, the median, variance, skewness, kurtosis, and Shannon entropy in 10 equally sized bins. 

**从嘴中ROI的最大幅度信号（参见第2.6节）中提取了以下特征：相邻峰之间的时间间隔（VTI）的方差，自相关序列的能量比（ENR），该能量比被计算为自相关序列的最后75％的样本所包含的能量与10个大小相等的仓中前25％的能量，中值，方差，偏度，峰度和香农熵所包含的能量。**

Features were not evaluated for tasks 1.2, 1.3, 3.1, 3.2 where mouth movements associated with speaking aloud would confound emotion-related activity. The results of the mouth related features are presented in Table 4. Inspection of Table 4 reveals that systematic variation in several metrics was restricted to the emotion recall conditions (associated with increased VTI and skewness, and reduced entropy as compared to the neutral condition). 

**没有针对任务1.2、1.3、3.1、3.2评估功能，其中与大声说话相关的嘴巴动作会混淆与情感相关的活动。表4给出了与嘴相关的特征的结果。对表4的检查表明，几种指标的系统变化仅限于情绪记忆条件（与中立状态相比，与增加的VTI和偏斜以及减少的熵有关）。**

VTI was used for estimating the periodicity of the movements based on the observation that rhythmic movements would produce variances close to zero. A higher VTI implies reduced rhythmicity of lip movements associated with increased levels of stress/anxiety. Increased skewness indicates higher asymmetry of the probability distribution, whereas entropy is an index of reduced disorder or spread within the energy of the signal. During watching stressful videos increased median and variance of the maximum magnitude were found indicating faster mouth movements.

**VTI用于根据节奏运动会产生接近零的方差的观察值来估计运动的周期性。较高的VTI意味着与压力/焦虑水平增加相关的嘴唇运动节律降低。偏度的增加表明概率分布的不对称性更高，而熵是减少的无序性或信号能量范围内扩散的指标。在观看紧张的视频过程中，发现中位数增加，并且最大震级出现差异，表明嘴巴运动更快。**

## 3.1.3. Head movements

Active Appearance Models as described in Section 2.5 were used to determine five specific facial landmarks pk, k = 1, 2,..., 5 on the nose as a highly stable portion of the face. The distribution of these specific landmarks, shown in the left-hand panel of Fig. 4, were selected in order to represent all types of translation and rotation head movements in the coronaltransverse planes. The 100th frame in the time series was used as reference and in each frame the Euclidean distance of these points from the corresponding points of the reference frame was calculated.

# 3.2. Relationship between self-reports and facial signs

The participants’ self-reports of perceived stress after sessions 4.2, 4.3, and 4.4 were used to assess potential associations between stress and facial signs at the individual level. Average (±s.d.) ratings were 1.55 ± 0.89 (relaxing video), 3.50 ± 1.11 (adventure/heights video), and 2.68 ± 1.06 (home invasion video). 

**在第4.2、4.3和4.4节后，参与者的自我感觉压力自我报告被用来评估个体水平上压力与面部症状之间的潜在关联。平均（±s.d。）评分为1.55±0.89（放松视频），3.50±1.11（冒险/身高视频）和2.68±1.06（家庭入侵视频）。**

One of the main problems in establishing associations relates to the different subjective scales implicitly applied by each person to mentally represent the entire range of experienced stress. Nonlinear models, such as pair-wise preference analysis, may be more appropriate to map individual physiological responses parameters to subjective stress ratings [93]. 

**建立联系的主要问题之一涉及每个人暗中应用的不同主观量表，这些量表在心理上代表所经历压力的整个范围。非线性模型（例如，成对偏好分析）可能更适合于将各个生理反应参数映射到主观压力等级[93]。**

In the current study preference pairs were constructed consisting of a stress rating and a single feature value estimated for each of the four tasks listed above. Correlation values were calculated using the test statistic [94]

**在当前的研究偏好对中，构成了压力等级和为上述四个任务中的每个任务估计的单个特征值。使用检验统计量计算相关值[94]**

where zi is 1 if there is an agreement between the rating difference (e.g. most stressful) and the corresponding difference in facial sign, and −1 if there is disagreement. N is the number of non-zero differences between self-reports and facial signs for each task. This statistic follows a binomial distribution

**如果在等级差异（例如压力最大）和相应的面部表情差异之间达成一致，则zi为1;如果分歧，则-1。 N是每个任务的自我报告和面部表情之间的非零差异数。此统计数据遵循二项分布**

# 3.3. Neutral and stress/anxiety states reference determination

Initially, each measure obtained from individual participants during all tasks were referenced to the task 4.2, which corresponds to the relaxed state of each subject as a baseline of facial cues, and all subsequent feature analyses were conducted on the difference values

**最初，从所有参与者在所有任务中获得的每种度量均参考任务4.2，该任务对应于每个受试者的放松状态作为面部提示的基线，并且随后对差异值进行所有后续特征分析**

where xref is the baseline condition (task 4.2) for each feature. This transformation generates a common reference to each feature across subjects providing data normalization.

**其中，外部参照是每个功能的基准条件（任务4.2）。此转换生成跨主题的通用参考，以提供数据标准化。**

# 3.4. Feature selection and ranking

In principle, classification efficiency is directly related to the number of relevant, complementary features employed in the procedure (as compared to univariate approaches). However, when the number of features entered into the model exceeds a particular level, determined by the characteristics of the data set used, classification accuracy may actually deteriorate.

**原则上，分类效率与程序中使用的相关互补特征的数量直接相关（与单变量方法相比）。但是，当输入模型的特征数量超过特定水平（由所使用的数据集的特征确定）时，分类精度实际上可能会下降。**

 In the present work, feature selection was performed using sequential forward selection (SFS) and sequential backward selection (SBS) methods [95] to reduce the number of features to be used for automatic discrimination of facial recordings according to experimental task. The objective function evaluating feature subsets was the area under the ROC curve (AUC) [96] using the classifier under investigation and reflecting emotional states differences within each experimental phase.

**在目前的工作中，特征选择是使用顺序前向选择（SFS）和顺序后向选择（SBS）方法[95]进行的，以减少根据实验任务自动识别面部记录的特征数量。使用研究中的分类器评估目标子集的目标函数是ROC曲线下的面积（AUC）[96]，并反映每个实验阶段的情绪状态差异。**

 The initial feature set consisted of 12 features, and SFS proved more effective than SBS to minimize the objective function. Mouth-related features were not evaluated for data from phases 1 and 3 because they involve at least one speaking aloud task. This procedure identified the sets of three to six most pertinent features across experimental phases presented in Table 8. An example ofthe area under curve as a function of the selected number of features through SFS is presented in Fig. 5.

**初始功能集包含12个功能，并且SFS被证明比SBS更有效地减少了目标功能。由于阶段1和阶段3的数据涉及至少一项语音任务，因此未评估与嘴相关的功能。此过程在表8中列出的实验阶段中确定了3至6个最相关的特征集。图5中显示了曲线下面积与通过SFS选择的特征数有关的示例。**

It should be stated that the effectiveness of a feature selection method depends on the evaluation metric, the classifier used for this metric, the distance metric and the selection method [97]. The most robust features are selected in most cases but different classification schemes may vary considering the selected least significant features as well as the overall order of selection.

**应该指出的是，特征选择方法的有效性取决于评估指标，用于该指标的分类器，距离指标和选择方法[97]。在大多数情况下，会选择最可靠的功能，但是考虑到所选的最低有效特征以及选择的总体顺序，不同的分类方案可能会有所不同。**

# 3.5. Classification performance results

The system’s classification procedure uses the feature set (referenced data) derived from the feature selection procedure for the data in each experimental phase (see Table 8). The classification methods that were used and tested are: K-nearest neighbours (Knn), Generalized Likelihood Ratio, Support Vector Machines (SVM), Naïve Bayes classifier and AdaBoost classifier. 

**系统的分类过程使用从特征选择过程中得出的特征集（参考数据）来处理每个实验阶段的数据（请参见表8）。使用和测试的分类方法是：K最近邻（Knn），广义似然比，支持向量机（SVM），朴素贝叶斯分类器和AdaBoost分类器。**

Each classification method was tested in terms of classification accuracy, i.e. its capacity to discriminate between feature sets obtained during the neutral expression of each phase and feature sets obtained during the remaining, stress-anxiety inducing tasks.A10-fold cross-validation was performed with the referred classifiers by randomly splitting the feature setinto 10 mutually exclusive subsets (folds) of approximately equal size. 

**对每种分类方法均进行了分类精度测试，即区分每个阶段的中性表达时获得的特征集与其余的压力焦虑诱导任务中获得的特征集的能力.A10倍交叉验证通过通过将特征集随机分割为10个大小相等的互斥子集（折叠），将这些分类器归类。**

In each case, the classifier was trained using 9 folds (90% of data) and tested on the remaining data (10% of data). The classification procedure was repeated 20 times and the average classification accuracy results are presented in Table 9 It can be observed that the classification results demonstrate good discrimination ability for the experimental phases performed. 

**在每种情况下，均使用9倍训练（90％的数据）训练分类器，并对其余数据（10％的数据）进行测试。重复分类程序20次，平均分类准确度结果列于表9中。可以看出，分类结果显示出对所进行的实验阶段具有良好的区分能力。**

In each experiment phase, classification accuracy that range between 80% and 90% taking into account the most effective classifier. The best classification accuracy was presented in the social exposure phase using Adaboost classifier achieving accuracy of 91.68%. The phase with Stroop-colour test and stressful images (phase 3) appeared to be more consistent across classifiers tested.

**在每个实验阶段，考虑到最有效的分类器，分类精度在80％到90％之间。在使用Adaboost分类器的社交曝光阶段，分类精度最高，达到91.68％。 Stroop彩色测试和压力图像的阶段（阶段3）在所有测试的分类器上似乎更加一致。**

# 4. Discussion

This study investigates the use of task elicited facial signs as indices of anxiety/stress in relation to neutral and relaxed states. 

**这项研究调查了使用任务引起的面部症状作为与中立和放松状态相关的焦虑/压力指标**。

Although there is much literature discussing recognition and analysis of the six basic emotions, i.e. anger, disgust, fear, happiness, sadness and surprise, considerably less research has focussed on stress and anxiety detection from facial videos. This can be justified partially by the fact that these states are considered as complex emotions that are linked to basic emotions (e.g. fear) making them more difficult to be interpreted in the human face. 

**尽管有很多文献讨论了对六种基本情绪的识别和分析，即愤怒，厌恶，恐惧，幸福，悲伤和惊奇，但针对面部视频中的压力和焦虑检测的研究却很少。这些事实被认为是与基本情感（例如恐惧）相关联的复杂情感，这使得它们在人脸中更难以解释，这一事实可以部分证明这一点。**

The sensitivity of specific measures of facial activity to situational stress/anxiety states was assessed in a step-wise manner, which entailed univariate analyses contrasting emotion elicitation tasks to their respective neutral reference conditions, followed by multivariate classification schemes.

**以逐步的方式评估面部活动的特定量度对情景压力/焦虑状态的敏感性，这需要进行单因素分析，将情绪激发任务与其各自的中性参考条件进行对比，然后采用多元分类方案。**

 The ultimate goal of these analyses was to identify sets of facial features, representing involuntary or semi-voluntary facial activity that can reliably discriminate emotional from neutral states through unsupervised procedures. The facial cues finally used in this study involved eye related features (blinks, eye aperture), mouth activity features (VTI, ENR, median, variance, skewness, kurtosis and Shannon entropy), head movement amplitude, head velocity and heart rate estimation derived from variations in facial skin colour.

**这些分析的最终目标是确定面部特征集，这些面部特征代表可以通过无监督程序可靠地将情绪与中立状态区分开的非自愿或半自愿面部活动。最终在这项研究中使用的面部提示涉及与眼睛相关的特征（眨眼，眼孔），嘴巴活动特征（VTI，ENR，中位数，方差，偏度，峰度和香农熵），头部运动幅度，头部速度和心率推导面部肤色的变化。**

 All these features provide a contactless approach of stress detection not interfering with human body in relation to other related studies employing semiinvasive measurements like ECG, EEG, galvanic skin response (GSR) and skin temperature. In addition,this approach incorporates information from a broad set of features derived from different face regions providing a holistic view of the problem under investigation. 

**与使用半侵入性测量（例如ECG，EEG，皮肤电反应（GSR）和皮肤温度）的其他相关研究相比，所有这些功能都提供了一种不干扰人体的压力检测非接触方法。另外，这种方法结合了来自不同面部区域的广泛特征信息，从而提供了对所研究问题的整体看法。**

The sensitivity of these features was tested across different experimental phases employing a wide variety of stress/anxiety eliciting conditions. It was deduced that certain features are sensitive to stress/anxiety states across a wide range of eliciting conditions, whereas others display a more restricted, task-specific performance. It can be concluded that eye blink rate increases during specific stress and anxiety conditions. In addition, head movement amplitude and velocity is also related to stress, in the form of small rapid movements. 

**这些特征的敏感性在使用各种压力/焦虑诱发条件的不同实验阶段进行了测试。可以推断，某些功能在广泛的引发条件下对压力/焦虑状态敏感，而其他功能则表现出更严格的任务特定性能。可以得出结论，在特定的压力和焦虑状态下，眨眼频率会增加。另外，头部运动的幅度和速度也与压力有关，以小的快速运动形式出现。**

Regarding mouth activity, the median and temporal variability (VTI) of the maximum magnitude increased while watching a stressful video whereas Shannon entropy appears to decrease. Finally, increased heart rate was observed during stress andanxiety states, where themost apparentdifferences werenoted in the social exposure phase (self-describing speech, text reading) and mental task (Stroop colour-word test). The feature selection procedure led to identifying specific features as being more robust in discriminating between stress/anxiety and a neutral emotional mode.

**关于口部活动，观看压力视频时，最大幅度的中位数和时间变异性（VTI）增加，而香农熵似乎降低。最后，在压力和焦虑状态下观察到心率增加，其中在社交暴露阶段（自我描述的语音，文本阅读）和心理任务（Stroop彩色单词测试）中发现了最明显的差异。特征选择过程导致将特定特征识别为在区分压力/焦虑和中性情绪模式方面更强大。**

The classification accuracy reached good levels as compared to the results ofthe few related studies available [25,34,37,98,99],taking into account the complexity and situational specificity of these emotional states. Studies [37] and [98] used, among other features, facial features achieving 75%–88% and 90.5% classification accuracy respectively. Biosignals like Blood Volume Pulse (BVP), Galvanic Skin Response (GSR), Pupil Diameter (PD) and Skin Temperature (ST) are used also in literature for discriminating stress situation as in [25,99,100] achieving 82.8%, 90.1% and 90.1% classification accuracies respectively. 

**考虑到这些情绪状态的复杂性和情境特异性，与少数相关研究[25,34,37,98,99]相比，分类准确性达到了良好的水平。研究[37]和[98]除其他特征外，还使用了面部特征，分别达到75％–88％和90.5％的分类精度。在文献[25,99,100]中，诸如血容量脉冲（BVP），皮肤电反应（GSR），瞳孔直径（PD）和皮肤温度（ST）之类的生物信号也用于区分压力状况，分别达到82.8％，90.1％和分类准确率分别为90.1％。**

To our knowledge,the best accuracy achieved is 97.4% in discriminating among 3 states of stress [30], but the techniques used (ECG, EMG, RR, GSR) are semi-invasive and therefore less convenientin real life applications.An intuitive review of stress detection techniques with corresponding classification accuracies is presented in [34]. 

**据我们所知，在区分三种压力状态时可达到的最佳精度为97.4％[30]，但是所使用的技术（ECG，EMG，RR，GSR）是半侵入性的，因此在实际应用中不太方便。 [34]中介绍了具有相应分类精度的压力检测技术。**

On the other hand, some limitations of the experimental procedure and analysis should be noted. The duration of facial recording may affect results, especially if it is very short and the consequent analysis of specific facial cues can be dubious. Based on our experiences, it is suggested that a video recording of at least 1 min duration could yield more reliable estimates and should be used for future recordings. 

**另一方面，应注意实验过程和分析的某些局限性。面部记录的持续时间可能会影响结果，尤其是当它很短并且因此对特定面部提示的分析可能令人怀疑时。根据我们的经验，建议至少持续1分钟的视频记录可以得出更可靠的估计，应该用于以后的记录。**

Moreover, elicitation of anxiety and stress states took place in a controlled, laboratory environment somehow limiting the generalizability of results to real-life situations where the intensity and valence of stressors may vary more widely. Physical conditions during facial recordings are found to affect the sensitivity of certain features, such as pupil size variation or blink rate where global monitor luminance changes induced by alternating static or dynamic visual stimuli (video scenes) are affecting some physiological features independently of cognitive and emotional state variables.

**此外，焦虑和压力状态的诱发是在受控的实验室环境中进行的，从而将结果的可推广性限制在现实生活中，在这种情况下，压力源的强度和效价可能会发生更大的变化。发现面部记录期间的身体状况会影响某些功能的敏感性，例如瞳孔大小变化或眨眼率，其中静态或动态视觉刺激（视频场景）交替引起的全局监视器亮度变化正在影响某些生理功能，而与认知和情绪无关状态变量。**

 Individual differences in both static and dynamic aspects of facial features represent another source of unwanted variability in the association between preselected facial features and individual emotional states. In the present study, a personspecific, reference condition was used to scale each facial feature to a common baseline prior to classification. An active reference was selected (viewing a relaxing video), which was intended to elicit facial activity related to attention and visual/optokinetic tracking, without triggering intense emotions

**面部特征的静态和动态方面的个体差异代表了预选面部特征与个人情绪状态之间关联性的另一个不期望的可变性来源。在本研究中，使用个人特定的参考条件将每个面部特征缩放到共同的基线，然后再进行分类。选择了一个活跃的参考对象（观看轻松的视频），该参考对象旨在引起与注意力和视觉/光动力学跟踪有关的面部活动，而不会引发强烈的情绪**