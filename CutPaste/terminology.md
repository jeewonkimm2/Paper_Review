**Paper : [CutPaste: Self-Supervised Learning for Anomaly Detection and Localization][link]**

[link]: https://openaccess.thecvf.com/content/CVPR2021/papers/Li_CutPaste_Self-Supervised_Learning_for_Anomaly_Detection_and_Localization_CVPR_2021_paper.pdf

1. empirical 경험[실험]에 의거한, 실증적인 (↔theoretical)
  - Our **empirical** study on MVTec anomaly detection dataset demonstrates the proposed algorithm is general to be able to detect various types of real-world defects.

2. surveillance 감시 (=observation)
  - Many problems from different vision applications are anomaly detection, including manufacturing defect detection, medical image analysis, and video **surveillance**.

3. semantic 의미의, 의미론적인
  - However, the anomaly score defined as an aggregation of pixel-wise reconstruction error or probability densities lacks to capture a high-level **semantic** information.

4. parameterized 파라미터로 나타낸
  - For example, deep one-class classifier demonstrates an effective end-to-end trained one-class classifiers **parameterized** by deep neural networks.

5. counterparts 대응 관계에 있는 것(사람), 상대
  - It outperforms its shallow **counterparts**, such as one-class SVMs and reconstruction-based approaches such as autoencoders.

6. geometric 기하학의, 기하학적인
  - In self-supervised representation learning, predicting **geometric** transformations of an image, such as rotation or translation, and contrastive learning have hown to be successful in distinguishing normal data from outliers.

7. proxy (측정, 계산하려는 다른 것을 대표하도록 이용하는) 대용물
  - We follow the two-stage framework, where we first learn self-supervised represnetations by solving a **proxy** task, then build a generative one-class classifier on learned representations to distinguish data with anomalous patterns from normal ones.

8. specifically 구체적으로 말하면, 분명히, 명확하게
  - **Specifically**, we formulate a proxy classification task between normal training data and the ones augmented by the *CutPaste*, the proposed data augmentation strategy that cuts an image patch and pates at a random location of an image.

9. coarse 조잡한
10. approximation 근사
  - CutPaste augmentation is motivated to produce a spatial irrefularity to serve as a **coarse approximation**.

11. aspect 방향, 측면
  - Rectangular patches of different sizes, **aspect** ratios, and roattion angles are pated to generate diverse augmentations.

12. crude 대충의, 대강의, 대충 만든
  - Although CutPaste augmented samples are easily distinguishable from real defects and thus might be a **crude** approximation of a real anomaly distributio, we show that representations learned by detecting irregularity introduced by CutPaste augmentations generalize well on detecting real defects.

13. holistic 전체적인
  - An image-level representation makes a **holistic** decision for anomaly detection and is used to localize defect via GradCAM.

14. subsequently 그 뒤에, 나중에
  - **Subsequently**, in Section 2.1, we present a novel method for learning self-supervised representations by predicting CutPaste augmentation, and extend to learning and extracting representations from local patches in Secion 2.4.

15. naively 소박하게, 순진하게
16. sub-optimal 차선의
  - While popular methods including rotation prediction and contrastive learning have been studied in the context of semantic one-class classification, our study in Section 4.1 shows that **naively** applying existing methods, such as rotation prediction or contrastive learning, is **sub-optimal** for detecting local defects as we will show in Section 4.1.

17. conjecture 추측, 추측하다
  - We **conjecture** that geometric transformations, such as rotations and translations, are effective in learning representation of semantic concepts (e.g., objectness), but less of regularity (e.g., continuity, repetition).

18. enforce 집행하다, 강요하다
19. invariance 변하지 않음
  - Cutout is found to be a useful data augmentation that **enforces invariance**, leading to improved accuracy on multi-class classification tasks.

20. discriminate 식별하다, 차별하다
  - In contrast, we start by **discriminating** Cutout images from the normal ones.

21. At first glance 처음에는
  - **At first glance**, the task seems easy to solve by well-crafted low level image filters.

22. hindsight 뒤늦은 깨달음
  - Surprisingly, as we will show in Section 4, without the **hindsight** of knowing this, a deep convolution network does not learn these shortcuts.

23. jitter 조금씩 움직이다
  - Optionally, we rotate or **jitter** pixel values in the patch.

24. empirically 실증적으로
  - **Empirically**, they have their own advantages on different types of defects.

25. leverage 이점, 영향력, use (something) to maximum advantage.
  - To **leverage** the strength of both scales in the training, we formulate a finer-grained 3-way classification task among normal, CutPaste and CutPaste-Scar by treating CutPaste variants as two separate classes.

26. pseudo 허위의, 가짜의, 모조의
  - The success of CutPaste may be understood from outlier exposure, where we generate the **pseudo** anomalies CutPaste) during the trianing.

27. preserve 지키다
  - Apart from using natural images as in, CutPaste creates examples **preserving** more local structures of the normal examples (i.e., the pasted patch is from the same domain), which is more challenging for the model to learn to find thi irregularity.

28. mimic 흉내
  - A natural question is if the success of CutPaste is from a good **mimic** of real defects.

29. amenable (특정한 방식으로) 처리할 수 있는, 말을 잘 듣는; -을 잘 받아들이는
  - The proposed CutPaste prediction task is not only shown to have strong performance on defect detection, but also **amenable** to combine with existing methods, such as transfer learning from pretrained models for better performance or patch-based models for more accurate localization, which we demonstrate in Section 4.

30. discriminative 차이를 분간하는, 구별을 나타내는, 특이한
  - Moreover, unlike typical use of augmentations for learning invariant representations, we learn a representation that is **discriminative** to these augmentations.

31. denoising 잡음제거
  - [11] presents a **denoising** autoencoder with patch-swap augmentation as noise process.

32. performant 성능 기준에 맞춘
  - Our method is simpler (e.g., no need to ltrain decoder or GAN) while highly **performant**, thus more practical.

33. align 나란히 만들다, -을 조정하다
  - For **aligned** objects, although it performs well on toothbrush, it is sub-optimal on capsule.

34. surpass 능가하다, 뛰어넘다
  - With a finer-grained 3way classification to leverage different scale of CutPaste, we achieve the best 95.2 AUC, which **surpasses** existing works on learning from scratch, such as P-SVDD (92.1 AUC).

35. Localization 지방화
  - Defect **Localization**

36. qualitative 질적인
  - We show **qualitative** results in the second row of Figure 4, which are visually pleasing.

37. receptive (새로운 사상, 제안에 대해) 수용적인[선뜻 받아들이는]
  - At test time, we densely extract anomaly scores with a stride of 4 and propagate the anomaly scores via **receptive** field upsampling with Gaussian smoothing.

38. versatile (사람이)다재다능한, (식품, 건물 등이) 다용도의, 다목적의
  - Here we demonstrate that the proposed self-supervised learning via CutPaste is **versatile**, which can also be used to improve the pretrianed networks to better adapt to the data.

39. showcase 전시하다
  - Second, we **showcase** the representation learned via predicting CutPaste generalizes well to more crafted unseen defects.

40. plausible 타당한 것 같은, 이치에 맞는, 그럴듯한
41. superiority 우월성, 우월, 거만함
42. systematic 체계적인, 조직적인
  - A **plausible** hypothesis on the **superiority** of 3-way formulation in our case is that it is more natural to model CutPaaste and CutPaste-scar augmentations separately than together as there exists a **systematic** difference between them in the size, shape, and rotation angle of patches.

43. synthetic (인위적으로) 합성한, 인조의
  - CutPaste on **Synthetic** Anomaly Detection

44. envision (특히 앞으로 바라는 일을) 마음속에 그리다[상상하다]
45. cornerstone 주춧돌, (어떤 일의) 초석
  - We **envision** the CutPaste augmentation could be a **cornerstone** for building a powerful model for semi-supervised and unsupervised defect detection.
