# Abstract 

There is a growing interest in computational approaches permitting accurate detection of nonverbal signs of depression and related symptoms (i.e., anxiety and distress) that may serve as minimally intrusive means of monitoring illness progression. The aim of the present work was to develop a methodology for detecting such signs and to evaluate its generalizability and clinical specificity for detecting signs of depression and anxiety. 

**允许精确检测抑郁症和相关症状（即焦虑和困扰）的非言语迹象的计算方法越来越引起人们的兴趣，这些手段可以作为监测疾病进展的最小干扰手段。本工作的目的是开发一种检测此类体征的方法，并评估其用于检测抑郁和焦虑体征的一般性和临床特异性。**

Our approach focused on dynamic descriptors of facial expressions, employing motion history image, combined with appearance-based feature extraction algorithms (local binary patterns, histogram of oriented gradients), and visual geometry group features derived using deep learning networks through transfer learning. 

**我们的方法专注于面部表情的动态描述符，采用运动历史图像，结合基于外观的特征提取算法（局部二进制模式，定向梯度的直方图）以及使用深度学习网络通过转移学习得出的视觉几何组特征。**

The relative performance of various alternative feature description and extraction techniques was first evaluated on a novel dataset comprising patients with a clinical diagnosis of depression (n = 20) and healthy volunteers (n = 45). Among various schemes involving depression measures as outcomes, best performance was obtained for continuous assessment of depression severity (as opposed to binary classification of patients and healthy volunteers). 

**首先在一个包含临床诊断为抑郁症的患者（n = 20）和健康志愿者（n = 45）的新型数据集上评估各种替代特征描述和提取技术的相对性能。在涉及抑郁测量作为结果的各种方案中，获得了最佳性能以连续评估抑郁的严重程度（与患者和健康志愿者的二元分类相反）。**

Comparable performance was achieved on a benchmark dataset, the audio/visual emotion challenge (AVEC’14). Regarding clinical specificity, results indicated that the proposed methodology was more accurate in detecting visual signs associated with self-reported anxiety symptoms. Findings are discussed in relation to clinical and technical limitations and future improvements.

**在基准数据集音频/视觉情感挑战（AVEC’14）上，可比的性能得以实现。关于临床特异性，结果表明，所提出的方法在检测与自我报告的焦虑症状相关的视觉症状方面更为准确。讨论了有关临床和技术局限性以及未来改进的发现。**



# intordution

Depression is the most prevalent mood disorder [1], with a structured clinical interview, according to the Diagnostic and Statistical Manual of Mental Disorders (DSM) criteria, being the standard procedure for depression diagnosis [2,3]. Clinical diagnosis of depression may be supported by selfreport questionnaires, such as the Beck Depression Inventory (BDI).

**抑郁症是最普遍的情绪障碍[1]，根据《精神障碍诊断和统计手册》（DSM）标准进行的结构化临床访谈是抑郁症诊断的标准程序[2,3]。抑郁症的临床诊断可以通过自我报告调查表（例如贝克抑郁量表（BDI））来支持。**

 These instruments are convenient and economical, but carry certain disadvantages, as they do not account for individual trait characteristics, other psychiatric and medical comorbidities (such as anxiety disorders and symptoms) and recent major stressors, and are vulnerable to intentional or unintentional reporting biases [4].

**这些工具既方便又经济，但具有某些不利条件，因为它们不能解决个人特征，其他精神病和医学合并症（例如焦虑症和症状）和近期的主要压力因素，并且容易受到有意或无意的报告偏见[ 4]**。

 Limited continuous monitoring of persons at risk (e.g., individuals with a history of mental illness or suffering from chronic, debilitating physical diseases) is one of the factors contributing to the high rate of underdiagnosed depressive episodes [5]. In this context, there is a rising interest for technological innovations to enhance accessibility to mental healthcare [6].

**对高危人群（例如，有精神病史或患有慢性，使人衰弱的身体疾病的患者）进行连续的有限监测是导致未充分诊断的抑郁发作高发生率的因素之一[5]。在这种情况下，人们对提高人们对精神保健的可及性的技术创新的兴趣不断提高[6]。**

Depression is typically manifested through a variety of nonverbal signs, including systematic patterns of facial expression and body posture [7,8]. Objective measures of psychoemotional status derived from facial image analysis could complement self-report instruments and help overcome some of their shortcomings [9], serving as a minimally intrusive tool for monitoring depression symptomatology.

**抑郁症通常通过多种非语言体征表现出来，包括面部表情和身体姿势的系统模式[7,8]。从面部图像分析中得出的心理情绪状态的客观测量可以补充自我报告工具，并帮助克服其某些缺点[9]，作为监测抑郁症症状的最低限度介入工具。**

 Furthermore, the widespread and relatively low-cost accessibility to computer and internet technologies, webcams, and smart phones, render an efficient system for depression assessment viable. However, given the current state-of-theart, video-based systems for depression assessment are not intended as standalone tools, but mainly as part of decision support systems assisting mental health professionals in remote monitoring of persons at risk. Considering that most of the nonverbal, facial signs of depression are dynamic [4,7,8] nearly all current approaches employ video-based, as opposed to frame-based (static), features.

**此外，对计算机和互联网技术，网络摄像头和智能电话的广泛且相对低成本的可访问性使抑郁症评估的有效系统可行。但是，考虑到当前的最新技术，基于视频的抑郁症评估系统并不是作为独立工具使用，而是主要作为决策支持系统的一部分，该系统可帮助精神卫生专业人员对危险人群进行远程监控。考虑到大多数的非语言，面部表情抑郁症都是动态的[4,7,8]，几乎所有当前方法都采用基于视频的功能，而不是基于帧（静态）的功能。**

Very few open datasets are available to support the development of novel technological solutions such as the AVEC’13-’141 and the DAIC-WOZ2 datasets, introduced as part of the Depression Recognition Sub-Challenge (DSC) of the audio visual emotion challenge (AVEC). The AVEC dataset provides full access to audiovisual recordings, annotated by self-reported BDI scores; 

**很少有开放数据集可用于支持新型技术解决方案的开发，例如AVEC'13-'141和DAIC-WOZ2数据集，它们是视听情感挑战的抑郁识别子挑战（DSC）的一部分（ AVEC）。 AVEC数据集提供对视听记录的完全访问权限，并通过自我报告的BDI分数进行注释；**

pre-extracted features and self-reported depression scale scores are available in the DAIC-WOZ dataset. The Pittsburgh3 dataset has also been made available to the research community in the same manner as the DAIC-WOZ, by sharing pre-extracted features, while the BlackDog dataset which has also been reported in several published reports [10] is kept private.

**预提取的特征和自我报告的抑郁量表得分可在DAIC-WOZ数据集中获得。通过共享预提取的功能，Pittsburgh3数据集也以与DAIC-WOZ相同的方式提供给研究团体，而在一些已发表的报告中也曾报道过的BlackDog数据集[10]保持私有。**

Cohn et al. [11] was one of the first attempts toward automatic assessment of depression based on facial image analysis. They achieved 79% overall accuracy for binary classification (depressed vs. non-depressed) on the Pittsburgh dataset using Active Appearance Models (AAM) with Support Vector Machines (SVM). Alghowinem et al. [10] achieved 88.3% recall (i.e., sensitivity) for the same binary problem on the BlackDog dataset; 

**Cohn等。 [11]是基于面部图像分析自动评估抑郁症的首批尝试之一。通过使用支持向量机（SVM）的主动外观模型（AAM），他们在匹兹堡数据集上进行二进制分类（抑郁与非抑郁）的总体准确性达到79％。 Alghowinem等。 [10]在BlackDog数据集上，相同的二进制问题的召回率（即敏感性）达到88.3％；**

they computed a total of 128 statistical features (“functionals”) from eyelid and eyecorners distances, also using SVM for the classification. In an earlier attempt toward binary classification of depression symptom severity on the AVEC dataset, our group achieved an F1 score of 87.4% using motion history image variants and Visual Geometry Group (VGG) features [12]. 

**他们还使用SVM进行了分类，从眼睑和眼角距离计算出总共128个统计特征（“功能”）。在对AVEC数据集上抑郁症症状严重程度进行二分类的早期尝试中，我们组使用运动历史图像变体和视觉几何组（VGG）功能获得了F1分数为87.4％[12]。**

Although previous work was extensive and tested several different algorithms, it focused on solving classification problems at the expense of fully appreciating the continuous nature of depression through regression methods. This gap in knowledge was  addressed by the proposed methodology which was further validated on video data, annotated for both depression- and anxiety-related visual features, obtained from patients diagnosed with depression. 

**尽管先前的工作很广泛，并测试了几种不同的算法，但它专注于解决分类问题，但以通过回归方法充分认识抑郁症的连续性为代价。知识上的差距可以通过拟议的方法加以解决，该方法在视频数据中得到了进一步验证，该数据被标注为与抑郁症和焦虑症相关的视觉特征，这些特征来自于患有抑郁症的患者。**

****

Continuous assessment is becoming increasingly popular and a key topic of the AVEC-DSC, where contestants attempted to minimize the error of predicting (healthy) participants’ BDI scores. Error is usually quantiﬁed as Mean Absolute Error (MAE) and Root-Mean-Square Error (RMSE).

**持续评估正日益成为AVEC-DSC的一个重要主题，在此竞赛中，参赛者试图将预测（健康）参与者BDI分数的误差降至最低。误差通常被量化为平均绝对误差（MAE）和均方根误差（RMSE）。**

 Among top performing approaches, Jan et al. [13] achieved MAE/RMSE of 6.68 and 8.01, respectively, with a dynamic history histogram from VGG features using a weighted fusion technique on the Partial Least Square and LinearRegression.

**在效果最好的方法中，Jan等人。 [13]使用偏最小二乘和线性回归的加权融合技术，利用VGG特征的动态历史直方图分别实现了6.68和8.01的MAE / RMSE。**

Corresponding error rates obtained by de Meloetal.[14]were6.59and8.31;they extracted Convolutional 3D (C3D) network features with 3D Global Average Pooling combined from both the entire face and the eye region, using Linear Regression (for further video-based approaches see also [15–24]). 

**[14]获得的相应错误率分别为6.59和8.31；他们使用线性回归从整个脸部和眼睛区域提取了结合了3D全局平均池化的卷积3D（C3D）网络特征。基于方法的方法也请参见[15-24]）。**  

The AVEC dataset is suitable for assessing the generalizability of novel algorithms and analysis pipelines across cultures as it includes arange of video recording contexts and settings. 

**AVEC数据集包括各种视频录制环境和设置，因此适合评估新型算法的通用性和跨文化的分析管道。**

This is a particularly important enterprise in view of extant research highlighting cultural differences in overt depression manifestations ([25,26]. However, the speciﬁcity of extracted visual features in assessing facial manifestations directly related to mood disturbances, as opposed to expressions of distress and anxiety, has not been assessed systematically in previous work.

**鉴于现有研究突出了明显的抑郁表现的文化差异，这是一个特别重要的事业（[25,26]。但是，提取的视觉特征在评估与情绪障碍直接相关的面部表现方面的特异性，而不是痛苦和表情的表达。焦虑，在先前的工作中尚未得到系统的评估。**

 In addition to the very high comorbidity of diagnoses of mood and anxiety disorders[27– 30], the two groups of disorders share common nonverbal manifestations

**除了诊断情绪和焦虑症的合并症非常高[27-30]外，两组疾病还具有共同的非语言表现**

The present study is addressing four speciﬁcaims.Firstly, to describe the development of a novel dataset comprising multimodal recordings from patients diagnosed with Major Depressive Disorder (MDD) and healthy volunteers. Data were obtained on a variety of experimental settings (including emotionally and cognitively neutral conditions andemotionally stimulatingsocialand non-social contexts). 

**本研究针对四个方面。首先，描述一个新的数据集的发展，该数据集包括来自诊断为重度抑郁症（MDD）的患者和健康志愿者的多模式记录。在各种实验设置（包括情绪和认知中性条件以及情感上刺激社会和非社会环境）下获得数据。**

Secondly, we aimed at developing a novel algorithmic pipeline for extracting facial expression elements from video recordings. In this context, various feature extraction and validation methods were employed and their relative performance was evaluated for (a) classiﬁcation of cases according to clinical diagnosis or expert ratings of overt facial manifestations of depression and (b) continuous assessment of depression symptomatology. 

**其次，我们旨在开发一种新颖的算法管道，用于从录像中提取面部表情元素。在这种情况下，采用了多种特征提取和验证方法，并针对（a）根据临床诊断或抑郁症明显面部表现的专家评级对病例进行分类，以及（b）连续评估抑郁症症状，对它们的相对性能进行了评估。**

Thirdly, the generalizability of the best-performing computational approach(i.e.,associated with the minimum prediction error for continuous assessment of depression symptomatology) was tested on the AVEC’14 dataset [21]. 

**第三，在AVEC’14数据集上测试了最佳计算方法的可推广性（即与用于抑郁症状持续评估的最小预测误差相关）[21]。**

Fourthly, given the known diversity of psychological and behavioral manifestations of depression, we evaluated the relative performance of this pipeline against self-rated anxiety symptoms, as well as expert ratings of visible facial manifestations of depression. 

**第四，考虑到已知的抑郁症心理和行为表现的多样性，我们评估了该管道针对自我评估的焦虑症状的相对性能，以及对抑郁症可见面部表现的专家评级。**



Investigating the co-occurrence of anxiety and depression symptoms is of clinical and research interest, in view of the signiﬁcant overlap in phenotypic presentations of related disorders [31]. 

**鉴于焦虑症和抑郁症的表型表现存在显着重叠，因此研究焦虑症和抑郁症的并发现象具有临床和研究意义[31]。**

To the best of our knowledge, there is a single other recent report addressing the common co-occurrence of depression- and anxiety-related visual signs[32].This earlier attempt did not employ persons with clinical diagnoses,a gap in the literature which is addressed in the current study.

**据我们所知，最近还有其他报告涉及与抑郁症和焦虑症有关的视觉症状的常见并发[32]。这种较早的尝试没有雇用具有临床诊断能力的人，文献上的空白本研究中已解决。**

# 2.1 Participants

The study included two groups of participants: healthy volunteers(n =45) aged 20–65 years without history of mental or neurological disorder, and patients suffering from MDD as diagnosed by their treating psychiatrists at the Psychiatry Outpatient Clinic,University Hospital of Heraklion(n = 20). 

**这项研究包括两组参与者：年龄在20-65岁之间，没有精神或神经系统疾病史的健康志愿者（n = 45），以及在伊拉克利翁大学医院精神病学门诊治疗的精神病医生诊断出患有MDD的患者（ n = 20）。**

Healthy volunteers were recruited through announcements in social media, ﬂyers posted at public sites, as well as through personal referrals. Patients were informed about the study by their physicians (psychiatrists at the outpatient clinic) during regular appointments and if they consented verbally the details of the study were explained to them both verbally and in writing by a research assistant (psychologist). The study was approved by the Bioethics Committee of the University Hospital of Heraklion (296/7/06-04-2016) and the National Data Protection Authority (Protocol No. ΓN/EΞ/392-2/21-04-2016). 

**通过在社交媒体上发布公告，在公共站点发布公告以及通过个人推荐来招募健康的志愿者。定期约诊期间，他们的医师（门诊诊所的精神科医生）将有关该研究的信息告知患者，如果他们口头同意，则研究助理（心理学家）会以口头和书面形式向研究人员解释研究的细节。该研究得到伊拉克利翁大学医院生物伦理学委员会（296/7 / 06-04-2016）和国家数据保护局（协议编号ΓN/EΞ/ 392-2 / 21-04-2016）的批准。**

Demographic information and scores on self-report anxiety and depression instruments can be found in Table 1 for each group. Both groups consisted of individuals of Greek ethnicity,with the exception of 1 patient and 2 healthy participants (immigrants from Albania, Italy, and Germany) who were permanent residents of Greece for over 20 years and competentinreading,speaking and understanding the Greek language. 

**表1为每组的人口统计信息和自我报告焦虑和抑郁工具的得分。两组均由希腊族裔组成，除了1名患者和2名健康参与者（来自阿尔巴尼亚，意大利和德国的移民）以外，他们是希腊的永久居民超过20年，并且能够读，说和理解希腊语。**

Although an effort was made to match the two groups with respect to demographics, the patient group was older and had completed fewer years of formal education than the control group. The two groups did not differ significantly on the percentage of women, which was higher than the percentage of men in both groups and especially among patients(85%)in accordance with the clinical literature[33]. 



The generalizability of the developed method was tested on the AVEC’14 dataset, comprising 300 video recordings from 83 participants obtained in the context of two conditions which are very similar to tasks used in the present study, namely reading a neutral text passage and completing a question-and-answer session with the experimenter.