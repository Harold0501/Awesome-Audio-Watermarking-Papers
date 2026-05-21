# Awesome-Audio-Watermarking-Papers

A collection list for audio watermarking papers

I categorize these papers into three types: **Post-Processing**, **Generative**, and **Benchmark / Surveys**

[Post-Processing](#post-processing): These papers mainly focus on how to hide more imperceptive and robust watermark into audio and ensure capacity of information. 

[Generative](#generative): These papers mainlt focus on how to let generative models (e.g. text-to-speech models) directly generate audios with watermark.

[Benchmark / Surveys](#benchmark--surveys): Some benchmark and survey papers on some specific technique or area. 

|Year|Venue|Title|Type|Paper|Code|
|----|-----|-----|----|-----|----|
|2023|ArXiv|WavMark: Watermarking for Audio Generation|Post-Processing|[Paper](https://arxiv.org/pdf/2308.12770)|[Code](https://github.com/wavmark/wavmark)|
|2024|NeurIPS|AudioMarkBench: Benchmarking Robustness of Audio Watermarking|Benchmark|[Paper](https://proceedings.neurips.cc/paper_files/paper/2024/file/5d9b7775296a641a1913ab6b4425d5e8-Paper-Datasets_and_Benchmarks_Track.pdf)|[Code](https://github.com/mileskuo42/AudioMarkBench)|
|2024|ICML|Proactive Detection of Voice Cloning with Localized Watermarking (AudioSeal)|Generative|[Paper](https://arxiv.org/pdf/2401.17264)|[Code](https://github.com/facebookresearch/audioseal)|
|2024|Interspeech|TraceableSpeech: Towards Proactively Traceable Text-to-Speech with Watermarking|Generative|[Paper](https://arxiv.org/pdf/2406.04840)|[Code](https://github.com/zjzser/TraceableSpeech)|
|2024|EMNLP|IDEAW: Robust Neural Audio Watermarking with Invertible Dual-Embedding|Post-Processing|[Paper](https://aclanthology.org/2024.emnlp-main.258.pdf)|[Code](https://github.com/PecholaL/IDEAW)|
|2024|International Conference on PST|Proactive Audio Authentication Using Speaker Identity Watermarking|Generative|[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10788060)|-|
|2025|Interspeech|WAKE: Watermarking Audio with Key Enrichment|Post-Processing|[Paper](https://arxiv.org/pdf/2506.05891)|[Code](https://github.com/thuhcsi/WAKE)|
|2025|ICML|XAttnMark: Learning Robust Audio Watermarking with Cross-Attention|Post-Processing|[Paper](https://arxiv.org/pdf/2502.04230)|[Code](https://liuyixin-louis.github.io/xattnmark/)|
|2025|ArXiv|GenMark: An Embedded Watermarking Scheme for Generative Audio Synthesis|Generative|[Paper](https://openreview.net/pdf?id=x9I1V6JY0r)|[Code](https://anonymous.4open.science/r/Gen-Mark-1F27/README.md)|
|2025|ArXiv|SoK: How Robust is Audio Watermarking in Generative AI models?|Benchmark|[Paper](https://arxiv.org/pdf/2503.19176)|[Code](https://sokaudiowm.github.io/)|
|2025|AAAI|Speech Watermarking with Discrete Intermediate Representations (DiscreteWM)|Post-Processing|[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/34600)|[Demo](https://discretewm.github.io/discrete_wm)|
|2025|USENIX Security Symposium|Audio Watermark: Dynamic and Harmless Watermark for Black-box Voice Dataset Copyright Protection|Post-Processing|[Paper](https://www.usenix.org/system/files/usenixsecurity25-guo-hanqing.pdf)|[Code](https://github.com/audiowatermark/audiowatermark.github.io)|
|2025|IEEE Transactions on Dependable and Secure Computing|When Unlearnable Examples Cooperate With Watermarking: A Dual Voice Data Protection Against Unauthorized Exploitation (Volto)|Generative|[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=11316260)|-|

## Post-Processing

**WavMark: Watermarking for Audio Generation**

ArXiv 2023

Guangyu Chen, Yu Wu, Shujie Liu, Tao Liu, Xiaoyong Du, Furu Wei

- Employs invertible neural networks for audio watermarking, ensuring the watermark’s resilience against manipulation while maintaining its inaudibility to human listeners.
- Propose a novel solution to the watermark localization problem, which offers simplicity in implementation and exhibits exceptional stability.
- Introduces various training and implementation strategies, including curriculum learning, weighted attack handling, and repeated encoding, collectively mitigating training complexities and improve implementation effectiveness.

Paper: https://arxiv.org/pdf/2308.12770

Code: https://github.com/wavmark/wavmark

**IDEAW: Robust Neural Audio Watermarking with Invertible Dual-Embedding**\

EMNLP 2024

Pengcheng Li, Xulong Zhang, Jing Xiao, Jianzong Wang

- Design a dual-embedding strategy to embed the watermark message and locating code separately, to accelerate the locating process.
- Introduce the balance block to alleviate the asymmetry caused by the attack layer between the invertible network and retain the symmetry of the invertible neural network.
- Able to embed more bits of watermark while ensuring imperceptibility and robustness.

Paper: https://aclanthology.org/2024.emnlp-main.258.pdf

Code: https://github.com/PecholaL/IDEAW

**WAKE: Watermarking Audio with Key Enrichment**

Interspeech 2025

Yaoxun Xu, Jianwei Yu, Hangting Chen, Zhiyong Wu, Xixin Wu, Dong Yu, Rongzhi Gu, Yi Luo

- The first key-controllable audio watermarking model, which uniquely embeds and decodes watermarks using specific keys.
- The first multi-watermark embedding and specific watermark extraction in the audio field.

Paper: https://arxiv.org/pdf/2506.05891

Code: https://github.com/thuhcsi/WAKE

**XAttnMark: Learning Robust Audio Watermarking with Cross-Attention**

ICML 2025

Yixin Liu, Lie Lu, Jihui Jin, Lichao Sun, Andrea Fanelli

- Introduce partial parameter sharing between the neural generator and the detector, with an embedding table as the bridge and a cross-attention module in the detector as the core, to allow for more efficient learning and accurate message retrieval.
- Introduce a simple yet effective message conditioning module that distributes the latent message temporally, boosting the attribution learning efficiency. 
- Introduce a new psychoacoustic-inspired temporal-frequency (TF) masking loss that captures per-tile masking effects.
- The only approach that can still successfully conduct watermark detection even with strong editing strength, testing on a zero-shot manner on unseen generative editing transformations. 

Paper: https://arxiv.org/pdf/2502.04230

Code: https://liuyixin-louis.github.io/xattnmark/

**Speech Watermarking with Discrete Intermediate Representations (DiscreteWM)**

AAAI 2025

Shengpeng Ji, Ziyue Jiang, Jialong Zuo, Minghui Fang, Yifu Chen, Tao Jin, Zhou Zhao

- The first attempt to embed watermark information in the robust discrete latent space.
- The proposed frame-wise strategy also resolves the challenges related to fixed-length training in speech watermarking and achieves 22.1x times faster detection speed.
- Allows users to freely manipulate the decoding capacity (up to 150 bits per second) and formats of the watermark without re-training the model.
- Propose a statistical Z-test to transform our frame-wise accuracy to utterance level for AI-generated content detection.

Paper: https://ojs.aaai.org/index.php/AAAI/article/view/34600

Demo: https://discretewm.github.io/discrete_wm

**Audio Watermark: Dynamic and Harmless Watermark for Black-box Voice Dataset Copyright Protection**

USENIX Security Symposium 2025

Hanqing Guo, Junfeng Guo, Bocheng Chen, Yuanda Wang, Xun Chen, Heng Huang, Qiben Yan, Li Xiao

- Propose the first voice dataset copyright protection approach, which offers adaptive and harmless functionality for protecting the speech dataset.
- Design a watermark generator comprising a style watermark generator, an audio effect synthesizer, an adversarial training module, and several tailored objective functions.

Paper: https://www.usenix.org/system/files/usenixsecurity25-guo-hanqing.pdf

Code: https://github.com/audiowatermark/audiowatermark.github.io

## Generative

**Proactive Detection of Voice Cloning with Localized Watermarking (AudioSeal)**

ICML 2024

Robin San Roman, Pierre Fernandez, Hady Elsahar, Alexandre Défossez, Teddy Furon, Tuan Tran

- The first audio watermarking technique designed for localized detection of AI generated speech up to the sample-level. 
- A novel perceptual loss inspired by auditory masking. 

Paper: https://arxiv.org/pdf/2401.17264

Code: https://github.com/facebookresearch/audioseal

**TraceableSpeech: Towards Proactively Traceable Text-to-Speech with Watermarking**

InterSpeech 2024

Junzuo Zhou, Jiangyan Yi, Tao Wang, Jianhua Tao, Ye Bai, Chu Yuan Zhang, Yong Ren, Zhengqi Wen

- Propose a proactively traceable TTS model jointly optimized for watermarking.
- Design a watermark embedding and extraction method tailored to TTS tasks, ensuring the watermark’s robustness as shown in the better extraction accuracy after resplicing attacks, while offering temporal flexibility in operation.

Paper: https://arxiv.org/pdf/2406.04840

Code: https://github.com/zjzser/TraceableSpeech

**Proactive Audio Authentication Using Speaker Identity Watermarking**

International Conference on PST 2024

Qi Li, Xiaodong Lin

- Propose an end-to-end framework that enhances robustness by repeatedly embedding watermark information and a synthesis layer with ensemble learning of five voice cloning encoders.
- Propose three extension strategies from different perspectives to address the common issue of limited watermark length.

Paper: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10788060

**GenMark: An Embedded Watermarking Scheme for Generative Audio Synthesis**

ArXiv 2025

Zihao Zhang, Wenlong Meng, Chen Gong, Guo Zhenyuan, Kui Su, Zunlei Feng, Chengkun Wei, Wenzhi Chen

- Propose a novel framework that embeds inaudible watermarks directly into generative audio models during training.
- Introduces a multi-scale discriminator and a mask model to improve audio quality and watermark robustness.

Paper: https://openreview.net/pdf?id=x9I1V6JY0r

Code: https://anonymous.4open.science/r/Gen-Mark-1F27/README.md

**When Unlearnable Examples Cooperate With Watermarking: A Dual Voice Data Protection Against Unauthorized Exploitation (Volto)**

IEEE Transactions on Dependable and Secure Computing 2025

Yunjie Ge, Ruxi Gu, Yuchen Liu, Lingchen Zhao, Bo Du, Qian Wang

- Introduce the first dual-function unlearnable audio, which not only discourages the unauthorized use of user data by model trainers but also empowers users to detect the misuse of their data via a watermark.

Paper: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=11316260)

## Benchmark / Surveys

**AudioMarkBench: Benchmarking Robustness of Audio Watermarking**

NeurIPS 2024 Track on Datasets and Benchmarks

Hongbin Liu, Moyang Guo, Zhengyuan Jiang, Lun Wang, Neil Zhenqiang Gong

- Introduce the first systematic and comprehensive benchmark for assessing the robustness of audio watermarking, focusing on evaluating robustness against watermark-removal perturbations and watermark-forgery perturbations. 
- Construct a new dataset AudioMarkData that meticulously sub-samples 20,000 audio samples from the Common Voice dataset. 

Paper: https://proceedings.neurips.cc/paper_files/paper/2024/file/5d9b7775296a641a1913ab6b4425d5e8-Paper-Datasets_and_Benchmarks_Track.pdf

Code: https://github.com/mileskuo42/AudioMarkBench

**SoK: How Robust is Audio Watermarking in Generative AI models?**

ArXiv 2025

Yizhu Wen, Ashwin Innuganti, Aaron Bien Ramos, Hanqing Guo, Qiben Yan

- Systematically analyze state-of-the-art audio watermarking schemes and identify several vulnerabilities.
- Propose and discover 8 new black-box attacks that effectively remove the watermark. The first to incorporate AI-induced distortions into watermark evaluations.

Paper: https://arxiv.org/pdf/2503.19176

Code: https://sokaudiowm.github.io/
