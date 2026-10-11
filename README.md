# Awesome-Audio-Watermarking-Papers

A collection list for audio watermarking papers

I categorize these papers into seven types: **Post-Processing**, **Key-based WM**, **Generative**, **Benchmark / Surveys**, **Identity / Copyright Protection**, **Integrity Protection**, and **Watermark-Free**.

[Post-Processing](#post-processing): These papers mainly focus on improving watermark imperceptibility, robustness, capacity, localization, and resistance to signal-processing or reconstruction attacks, in a separate post-hoc process.

[Key-based WM](#key-based-wm): These papers use secret keys as a core component of watermark embedding and detection, aiming to restrict unauthorized extraction, detection, or manipulation and improve watermark security.

[Generative](#generative): These papers mainly focus on how to let generative models (e.g. text-to-speech models) directly generate audios with watermark.

[Benchmark / Surveys](#benchmark--surveys): Some benchmark and survey papers on some specific technique or area.

[Identity / Copyright Protection](#identity--copyright-protection): These papers focus on protecting speaker identity or voice data ownership against unauthorized voice cloning, synthesis, or model training by enabling subsequent tracing or ownership verification.

[Integrity Protection](#integrity-protection): These papers focus on verifying whether the linguistic content or authenticity of a speech recording has been maliciously altered, while ideally remaining tolerant to benign processing that preserves the original content.

[Watermark-Free](#watermark-free): These papers explore traceability mechanisms that do not rely on explicitly embedding a watermark into the released audio.

|Year|Venue|Title|Type|Paper|Code|
|----|-----|-----|----|-----|----|
|2023|AAAI|DeAR: A Deep-Learning-Based Audio Re-recording Resilient Watermarking|Post-Processing|[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/26550)|-|
|2023|arXiv|WavMark: Watermarking for Audio Generation|Post-Processing|[Paper](https://arxiv.org/pdf/2308.12770)|[Code](https://github.com/wavmark/wavmark)|
|2023|ACM MM|Who is Speaking Actually? Robust and Versatile Speaker Traceability for Voice Conversion|Identity Protection|[Paper](https://dl.acm.org/doi/pdf/10.1145/3581783.3612333)|-|
|2024|NDSS|Detecting Voice Cloning Attacks via Timbre Watermarking|Identity Protection|[Paper](https://www.ndss-symposium.org/wp-content/uploads/2024-200-paper.pdf)|[Code](https://github.com/TimbreWatermarking/TimbreWatermarking)|
|2024|NeurIPS|AudioMarkBench: Benchmarking Robustness of Audio Watermarking|Benchmark|[Paper](https://proceedings.neurips.cc/paper_files/paper/2024/file/5d9b7775296a641a1913ab6b4425d5e8-Paper-Datasets_and_Benchmarks_Track.pdf)|[Code](https://github.com/mileskuo42/AudioMarkBench)|
|2024|ICML|Proactive Detection of Voice Cloning with Localized Watermarking (AudioSeal)|Post-Processing|[Paper](https://arxiv.org/pdf/2401.17264)|[Code](https://github.com/facebookresearch/audioseal)|
|2024|Interspeech|TraceableSpeech: Towards Proactively Traceable Text-to-Speech with Watermarking|Generative|[Paper](https://arxiv.org/pdf/2406.04840)|[Code](https://github.com/zjzser/TraceableSpeech)|
|2024|Interspeech|SilentCipher: Deep Audio Watermarking|Post-Processing|[Paper](https://www.isca-archive.org/interspeech_2024/singh24_interspeech.pdf)|[Code](https://github.com/sony/silentcipher)|
|2024|EMNLP|IDEAW: Robust Neural Audio Watermarking with Invertible Dual-Embedding|Post-Processing|[Paper](https://aclanthology.org/2024.emnlp-main.258.pdf)|[Code](https://github.com/PecholaL/IDEAW)|
|2024|PST|Proactive Audio Authentication Using Speaker Identity Watermarking|Identity Protection|[Paper](https://ieeexplore.ieee.org/abstract/document/10788060)|-|
|2025|Interspeech|WAKE: Watermarking Audio with Key Enrichment|Key-based WM|[Paper](https://arxiv.org/pdf/2506.05891)|[Code](https://github.com/thuhcsi/WAKE)|
|2025|Interspeech|VoiceMark: Zero-Shot Voice Cloning-Resistant Watermarking Approach Leveraging Speaker-Specific Latents|Identity Protection|[Paper](https://www.isca-archive.org/interspeech_2025/li25g_interspeech.pdf)|[Code](https://huggingface.co/spaces/haiyunli/VoiceMark/tree/main)|
|2025|ICML|XAttnMark: Learning Robust Audio Watermarking with Cross-Attention|Post-Processing|[Paper](https://arxiv.org/pdf/2502.04230)|[Code](https://liuyixin-louis.github.io/xattnmark/)|
|2025|arXiv|GenMark: An Embedded Watermarking Scheme for Generative Audio Synthesis|Generative|[Paper](https://openreview.net/pdf?id=x9I1V6JY0r)|-|
|2025|arXiv|SoK: How Robust is Audio Watermarking in Generative AI models?|Benchmark|[Paper](https://arxiv.org/pdf/2503.19176)|[Code](https://sokaudiowm.github.io/)|
|2025|AAAI|Speech Watermarking with Discrete Intermediate Representations (DiscreteWM)|Post-Processing|[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/34600)|[Demo](https://discretewm.github.io/discrete_wm)|
|2025|USENIX Security Symposium|Audio Watermark: Dynamic and Harmless Watermark for Black-box Voice Dataset Copyright Protection|Copyright Protection|[Paper](https://www.usenix.org/system/files/usenixsecurity25-guo-hanqing.pdf)|[Code](https://github.com/audiowatermark/audiowatermark.github.io)|
|2025|arXiv|Traceable TTS: Toward Watermark-Free TTS with Strong Traceability|Watermark-Free|[Paper](https://arxiv.org/pdf/2507.03887)|-|
|2025|IEEE Transactions on Dependable and Secure Computing|When Unlearnable Examples Cooperate With Watermarking: A Dual Voice Data Protection Against Unauthorized Exploitation (Volto)|Copyright Protection|[Paper](https://ieeexplore.ieee.org/abstract/document/11316260)|-|
|2026|Interspeech|DuraMark: Duration-Embedded Watermarking in LLM-based TTS|Generative|[Paper](https://arxiv.org/pdf/2606.15264)|[Code](https://github.com/muzw/DuraMark)|
|2026|Interspeech|Latent-Mark: An Audio Watermark Robust to Neural Codec Compression|Post-Processing|[Paper](https://arxiv.org/pdf/2603.05310)|[Code](https://github.com/yenshan0530/Latent-Mark)|
|2026|Interspeech|Countering Neural Audio Codec Distortions in Watermarking with Adaptive Restoration|Post-Processing|[Paper](https://www.isca-archive.org/interspeech_2026/park26d_interspeech.pdf)|-|
|2026|Interspeech|AudioNoisePrints: Model-free audio watermarking using spatial correlation in flow matching TTS|Generative|[Paper](https://www.isca-archive.org/interspeech_2026/tse26_interspeech.pdf)|-|
|2026|Interspeech|VoxWatermark: A Large-Scale Benchmark for Audio Watermark Detection under Perturbations|Benchmark|[Paper](https://www.isca-archive.org/interspeech_2026/sedaghati26_interspeech.pdf)|[Code](https://github.com/wailywang/VoxWatermark)|
|2026|Interspeech|Phoneme-Aware Mamba Watermark: An Active Defense System Against Purified Speech Deepfakes|Identity Protection|[Paper](https://www.isca-archive.org/interspeech_2026/shao26_interspeech.pdf)|-|
|2026|ICME|Feature-Aligned Speech Watermarking for Robustness to Reconstruction Distortions (AlignMark)|Post-Processing|[Paper](https://arxiv.org/pdf/2606.11828)|[Code](https://huggingface.co/haiyunli/AlignMark/tree/main)|
|2026|Odyssey|Latent Secret Spin: Keyed Orthogonal Rotations for Blind Speech Watermarking in Anisotropic Latent Spaces|Key-based WM|[Paper](https://www.eurecom.edu/en/publication/8752)|-|
|2026|ICASSP|AURA: A Stegaformer-Based Scalable Deep Audio Watermark with Extreme Robustness|Post-Processing|[Paper](https://ieeexplore.ieee.org/abstract/document/11462806)|-|
|2026|ICASSP|StreamMark: A Deep Learning-Based Semi-Fragile Audio Watermarking for Proactive Deepfake Detection|Integrity Protection|[Paper](https://ieeexplore.ieee.org/abstract/document/11463325)|-|
|2026|ICASSP|LINGUARD: Authenticating Speech Recordings Using Speech Recognition and Watermark|Integrity Protection|[Paper](https://ieeexplore.ieee.org/abstract/document/11462384)|-|
|2026|arXiv|Investigating Codec-Internal Latent Audio Watermarking for Neural Codec Robustness|Post-Processing|[Paper](https://arxiv.org/pdf/2607.21132)|-|
|2026|ACM MM|SSTMark: Robust Training-Free Semantic-Level Speech Watermarking|Post-Processing|[Paper](https://arxiv.org/pdf/2607.17592)|-|

## Post-Processing

**DeAR: A Deep-Learning-Based Audio Re-recording Resilient Watermarking**

AAAI 2023

Chang Liu, Jie Zhang, Han Fang, Zehua Ma, Weiming Zhang, Nenghai Yu

- Pioneer an end-to-end deep learning framework for embedding and extracting watermarks from audio carriers.
- Model the acoustic propagation, environmental response, and recording-device distortions of the re-recording process with differentiable layers for robust training.
- Achieve 98.55% average bit recovery accuracy at a 20 cm re-recording distance while maintaining an embedding SNR of 25.86 dB.

Paper: https://ojs.aaai.org/index.php/AAAI/article/view/26550

**WavMark: Watermarking for Audio Generation**

arXiv 2023

Guangyu Chen, Yu Wu, Shujie Liu, Tao Liu, Xiaoyong Du, Furu Wei

- Employs invertible neural networks for audio watermarking, ensuring the watermark’s resilience against manipulation while maintaining its inaudibility to human listeners.
- Propose a novel solution to the watermark localization problem, which offers simplicity in implementation and exhibits exceptional stability.
- Introduces various training and implementation strategies, including curriculum learning, weighted attack handling, and repeated encoding, collectively mitigating training complexities and improve implementation effectiveness.

Paper: https://arxiv.org/pdf/2308.12770

Code: https://github.com/wavmark/wavmark

**Proactive Detection of Voice Cloning with Localized Watermarking (AudioSeal)**

ICML 2024

Robin San Roman, Pierre Fernandez, Hady Elsahar, Alexandre Défossez, Teddy Furon, Tuan Tran

- The first audio watermarking technique designed for localized detection of AI generated speech up to the sample-level.
- A novel perceptual loss inspired by auditory masking.

Paper: https://arxiv.org/pdf/2401.17264

Code: https://github.com/facebookresearch/audioseal

**SilentCipher: Deep Audio Watermarking**

Interspeech 2024

Mayank Kumar Singh, Naoya Takahashi, Weihsiang Liao, Yuki Mitsufuji

- Integrate psychoacoustic masking thresholds into deep audio watermarking to keep embedded messages imperceptible, including in band-limited audio.
- Introduce pseudo-differentiable compression layers to improve robustness against non-differentiable audio codecs and other distortions.
- Remove the need for perceptual losses, support a user-controlled SDR bound, and operate on professional-quality 44.1 kHz audio.

Paper: https://www.isca-archive.org/interspeech_2024/singh24_interspeech.pdf

Code: https://github.com/sony/silentcipher

**IDEAW: Robust Neural Audio Watermarking with Invertible Dual-Embedding**

EMNLP 2024

Pengcheng Li, Xulong Zhang, Jing Xiao, Jianzong Wang

- Design a dual-embedding strategy to embed the watermark message and locating code separately, to accelerate the locating process.
- Introduce the balance block to alleviate the asymmetry caused by the attack layer between the invertible network and retain the symmetry of the invertible neural network.
- Able to embed more bits of watermark while ensuring imperceptibility and robustness.

Paper: https://aclanthology.org/2024.emnlp-main.258.pdf

Code: https://github.com/PecholaL/IDEAW

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

**Latent-Mark: An Audio Watermark Robust to Neural Codec Compression**

Interspeech 2026

Yen-Shan Chen, Shih-Yu Lai, Ying-Jung Tsou, Yi-Cheng Lin, Bing-Yu Chen, Yun-Nung Chen, Hung-yi Lee, Shang-Tse Chen

- Introduce the first zero-bit audio watermarking framework explicitly designed to survive neural codec compression.
- Optimize the waveform to induce a detectable directional shift in codec-invariant latent space while aligning perturbations with the natural audio manifold for imperceptibility.
- Use Cross-Codec Optimization across multiple surrogate codecs to achieve zero-shot transferability to unseen neural codecs.

Paper: https://arxiv.org/pdf/2603.05310

Code: https://github.com/yenshan0530/Latent-Mark

**Countering Neural Audio Codec Distortions in Watermarking with Adaptive Restoration**

Interspeech 2026

Sungho Park, Thien An Nguyen, Souhwan Jung

- Insert a codec-aware restoration stage before watermark extraction to recover watermark-relevant spectrogram details damaged by neural audio codecs.
- Combine a ConvNeXt-based U-Net with a lightweight codec classifier that dynamically selects a codec-specific restoration model.
- Improve bitwise watermark accuracy from near-random levels to over 98% for residual-vector-quantization-based codecs across a broad range of neural codecs.

Paper: https://www.isca-archive.org/interspeech_2026/park26d_interspeech.pdf

**Feature-Aligned Speech Watermarking for Robustness to Reconstruction Distortions (AlignMark)**

ICME 2026

Haiyun Li, Shuhai Peng, Zhisheng Zhang, Jingran Xie, Xiaofeng Xie, Hanyang Peng, Zhiyong Wu

- Align the watermark with the original speech feature distribution, allowing higher watermark energy and stronger robustness without sacrificing perceptual quality.
- Generate a pseudo-speech watermark with a pretrained speech codec and fuse it into the input spectrogram, guided by VAD and perceptual losses.
- Improve robustness against both seen and unseen speech reconstruction models while retaining imperceptibility comparable to existing methods.

Paper: https://arxiv.org/pdf/2606.11828

Code: https://huggingface.co/haiyunli/AlignMark/tree/main

**AURA: A Stegaformer-Based Scalable Deep Audio Watermark with Extreme Robustness**

ICASSP 2026

Linxi Li, Liwei Jin, Yechen Wang, Houmin Sun, Zi Hu, Carsten Maple

- Propose Stegaformer, which combines a Conformer backbone with Feature-wise Linear Modulation for deep fusion of audio features and watermark keys.
- Achieve strong perceptual quality and robustness against extreme transformations, including re-recording attacks and aggressive low-bitrate compression.
- Present the first empirical scaling-law study for audio watermarking and identify architectural principles for scaling capacity and performance.

Paper: https://ieeexplore.ieee.org/abstract/document/11462806

**Investigating Codec-Internal Latent Audio Watermarking for Neural Codec Robustness**

arXiv 2026

Zi Hu, Houmin Sun, Linxi Li, Yechen Wang, Liwei Jin, Carsten Maple, Ming Li

- Embed a 32-bit message directly into the continuous latent representation of a codec-like speech autoencoder before neural decoding.
- Combine a SEANet-style encoder-decoder, a Conformer-based message embedder, RVQ-guided latent decomposition, and a latent-domain detector trained under codec and signal-processing transformations.
- Characterize the trade-off between codec robustness and perceptual quality, with EnCodec-aware training substantially improving message recovery under EnCodec compression.

Paper: https://arxiv.org/pdf/2607.21132

**SSTMark: Robust Training-Free Semantic-Level Speech Watermarking**

ACM MM 2026

Kuan-Lin Chu, Jun-Cheng Chen, Chun-Shien Lu

- Introduce a training-free framework that embeds watermark information into the semantic content of generated speech through text watermarking.
- Detect the watermark from linguistic content recovered by speech-to-text, avoiding dependence on fragile waveform- or spectrogram-level patterns.
- Achieve the strongest average robustness on AudioMarkBench, improving detection by 4.6% on signal-processing edits and 16.9% on compression edits at a 1% false-positive rate.

Paper: https://arxiv.org/pdf/2607.17592

## Key-based WM

**WAKE: Watermarking Audio with Key Enrichment**

Interspeech 2025

Yaoxun Xu, Jianwei Yu, Hangting Chen, Zhiyong Wu, Xixin Wu, Dong Yu, Rongzhi Gu, Yi Luo

- The first key-controllable audio watermarking model, which uniquely embeds and decodes watermarks using specific keys.
- The first multi-watermark embedding and specific watermark extraction in the audio field.

Paper: https://arxiv.org/pdf/2506.05891

Code: https://github.com/thuhcsi/WAKE

**Latent Secret Spin: Keyed Orthogonal Rotations for Blind Speech Watermarking in Anisotropic Latent Spaces**

Odyssey 2026

Emma Coletta, Massimiliano Todisco, Michele Panariello, Antonio Faonio, Nicholas Evans

- Introduce a blind and training-free watermarking method that operates geometrically in the continuous latent space of a pretrained neural audio codec.
- Embed payloads through localized orthogonal rotations in principal-component planes selected by a secret-key-derived schedule.
- Create detectable covariance signatures that preserve perceptual quality, resist common signal transformations, and support flexible payload sizes.

Paper: https://www.eurecom.edu/en/publication/8752

## Generative

**TraceableSpeech: Towards Proactively Traceable Text-to-Speech with Watermarking**

Interspeech 2024

Junzuo Zhou, Jiangyan Yi, Tao Wang, Jianhua Tao, Ye Bai, Chu Yuan Zhang, Yong Ren, Zhengqi Wen

- Propose a proactively traceable TTS model jointly optimized for watermarking.
- Design a watermark embedding and extraction method tailored to TTS tasks, ensuring the watermark’s robustness as shown in the better extraction accuracy after resplicing attacks, while offering temporal flexibility in operation.

Paper: https://arxiv.org/pdf/2406.04840

Code: https://github.com/zjzser/TraceableSpeech

**GenMark: An Embedded Watermarking Scheme for Generative Audio Synthesis**

arXiv 2025

Zihao Zhang, Wenlong Meng, Chen Gong, Guo Zhenyuan, Kui Su, Zunlei Feng, Chengkun Wei, Wenzhi Chen

- Propose a novel framework that embeds inaudible watermarks directly into generative audio models during training.
- Introduces a multi-scale discriminator and a mask model to improve audio quality and watermark robustness.

Paper: https://openreview.net/pdf?id=x9I1V6JY0r

Code: https://anonymous.4open.science/r/Gen-Mark-1F27/README.md

**DuraMark: Duration-Embedded Watermarking in LLM-based TTS**

Interspeech 2026

Zhenwei Mou, Weili Jiang, Liping Chen, Zhen-Hua Ling, Kong Aik Lee, Kai Gao, Boyu Zhao

- Introduce an information-level generative watermark that encodes messages by editing syllable durations during LLM-based speech synthesis.
- Develop a duration-controllable TTS model and a duration extractor for precise watermark embedding and detection.
- Demonstrate substantially stronger robustness than signal-level baselines against neural codec and vocoder resynthesis attacks.

Paper: https://arxiv.org/pdf/2606.15264

Code: https://github.com/muzw/DuraMark

**AudioNoisePrints: Model-free audio watermarking using spatial correlation in flow matching TTS**

Interspeech 2026

Timothy Tin-Long Tse, Jian Zhu, Aidan Pine, Mengzhe Geng

- Introduce a training-free watermarking pipeline for flow-matching and diffusion TTS that exploits spatial correlations between the initial Gaussian noise and the generated audio.
- Detect provenance with cosine correlation while avoiding TTS retraining, post-hoc audio modification, and additional computation during generation.
- Extend the approach with a lightweight detector for stronger augmentations and demonstrate the same correlation property across F5-TTS, Matcha-TTS, and DiffWave.

Paper: https://www.isca-archive.org/interspeech_2026/tse26_interspeech.pdf

## Benchmark / Surveys

**AudioMarkBench: Benchmarking Robustness of Audio Watermarking**

NeurIPS 2024 Track on Datasets and Benchmarks

Hongbin Liu, Moyang Guo, Zhengyuan Jiang, Lun Wang, Neil Zhenqiang Gong

- Introduce the first systematic and comprehensive benchmark for assessing the robustness of audio watermarking, focusing on evaluating robustness against watermark-removal perturbations and watermark-forgery perturbations.
- Construct a new dataset AudioMarkData that meticulously sub-samples 20,000 audio samples from the Common Voice dataset.

Paper: https://proceedings.neurips.cc/paper_files/paper/2024/file/5d9b7775296a641a1913ab6b4425d5e8-Paper-Datasets_and_Benchmarks_Track.pdf

Code: https://github.com/mileskuo42/AudioMarkBench

**SoK: How Robust is Audio Watermarking in Generative AI models?**

arXiv 2025

Yizhu Wen, Ashwin Innuganti, Aaron Bien Ramos, Hanqing Guo, Qiben Yan

- Systematically analyze state-of-the-art audio watermarking schemes and identify several vulnerabilities.
- Propose and discover 8 new black-box attacks that effectively remove the watermark. The first to incorporate AI-induced distortions into watermark evaluations.

Paper: https://arxiv.org/pdf/2503.19176

Code: https://sokaudiowm.github.io/

**VoxWatermark: A Large-Scale Benchmark for Audio Watermark Detection under Perturbations**

Interspeech 2026

Farnaz Sedaghati, Yuxi Wang, Zicheng Weng, Wei Rao

- Construct a detection-oriented benchmark containing 91.09 million samples and approximately 126,514 hours of multilingual, multi-source audio produced with 10 neural and traditional watermarking methods.
- Introduce no-box, black-box, and white-box perturbation protocols to evaluate watermark detectors under realistic distribution shifts and adversarial conditions.
- Propose AudioWMD as a unified baseline for large-scale, multi-method, cross-distribution watermark detection.

Paper: https://www.isca-archive.org/interspeech_2026/sedaghati26_interspeech.pdf

Code: https://github.com/wailywang/VoxWatermark

## Identity / Copyright Protection

**Who is Speaking Actually? Robust and Versatile Speaker Traceability for Voice Conversion**

ACM MM 2023

Yanzhen Ren, Hongcheng Zhu, Liming Zhai, Zongkun Sun, Rubing Shen, Lina Wang

- Introduce VoxTracer, the first framework to investigate speaker traceability for voice conversion by recovering the source speaker identity and even the source speech.
- Use speaker embeddings and an asynchronously trained VAE-Glow structure to hide identity during voice conversion and recover it after lossy transmission.
- Achieve nearly 100% tracing accuracy under AAC, MP3, Opus, and SILK compression at bitrates down to 16 kbps using only 0.74 seconds of speech.

Paper: https://dl.acm.org/doi/pdf/10.1145/3581783.3612333

**Detecting Voice Cloning Attacks via Timbre Watermarking**

NDSS 2024

Chang Liu, Jie Zhang, Tianwei Zhang, Xi Yang, Weiming Zhang, Nenghai Yu

- Introduce timbre watermarking to proactively protect released speech and detect unauthorized voice cloning through watermarks transferred to cloned audio.
- Embed watermarks in the frequency domain with repeated embedding to resist common preprocessing and watermark-removal attacks.
- Model the shared voice-cloning process as a distortion layer to generalize across cloning systems, including real-world services and adaptive attacks.

Paper: https://www.ndss-symposium.org/wp-content/uploads/2024-200-paper.pdf

Code: https://github.com/TimbreWatermarking/TimbreWatermarking

**Proactive Audio Authentication Using Speaker Identity Watermarking**

PST 2024

Qi Li, Xiaodong Lin

- Propose an end-to-end framework that enhances robustness by repeatedly embedding watermark information and a synthesis layer with ensemble learning of five voice cloning encoders.
- Propose three extension strategies from different perspectives to address the common issue of limited watermark length.

Paper: https://ieeexplore.ieee.org/abstract/document/10788060

**VoiceMark: Zero-Shot Voice Cloning-Resistant Watermarking Approach Leveraging Speaker-Specific Latents**

Interspeech 2025

Haiyun Li, Zhiyong Wu, Xiaofeng Xie, Jingran Xie, Yaoxun Xu, Hanyang Peng

- Introduce the first watermarking method designed to survive zero-shot voice cloning without retraining the cloning model.
- Use speaker-specific neural-codec latents as the watermark carrier so the watermark transfers from an audio prompt into synthesized speech.
- Combine voice-cloning-simulated augmentations with a VAD-based loss, achieving over 95% detection accuracy across multiple zero-shot cloning models.

Paper: https://www.isca-archive.org/interspeech_2025/li25g_interspeech.pdf

Code: https://huggingface.co/spaces/haiyunli/VoiceMark/tree/main

**Audio Watermark: Dynamic and Harmless Watermark for Black-box Voice Dataset Copyright Protection**

USENIX Security Symposium 2025

Hanqing Guo, Junfeng Guo, Bocheng Chen, Yuanda Wang, Xun Chen, Heng Huang, Qiben Yan, Li Xiao

- Propose the first voice dataset copyright protection approach, which offers adaptive and harmless functionality for protecting the speech dataset.
- Design a watermark generator comprising a style watermark generator, an audio effect synthesizer, an adversarial training module, and several tailored objective functions.

Paper: https://www.usenix.org/system/files/usenixsecurity25-guo-hanqing.pdf

Code: https://github.com/audiowatermark/audiowatermark.github.io

**When Unlearnable Examples Cooperate With Watermarking: A Dual Voice Data Protection Against Unauthorized Exploitation (Volto)**

IEEE Transactions on Dependable and Secure Computing 2025

Yunjie Ge, Ruxi Gu, Yuchen Liu, Lingchen Zhao, Bo Du, Qian Wang

- Introduce the first dual-function unlearnable audio, which not only discourages the unauthorized use of user data by model trainers but also empowers users to detect the misuse of their data via a watermark.

Paper: https://ieeexplore.ieee.org/abstract/document/11316260

**Phoneme-Aware Mamba Watermark: An Active Defense System Against Purified Speech Deepfakes**

Interspeech 2026

Yanda Shao, Mengke Zhang, Zhixin Lin, Tianyi Yang

- Embed speaker-identity bitstrings with a bidirectional Mamba-based encoder so that the watermark transfers from protected speech to cloned speech.
- Use phoneme-guided stable spectral regions and purification-aware adversarial training to preserve the watermark against the diffusion-based PhonePuRe attack.
- Achieve near-100% source-tracing accuracy on cloned speech with approximately one-second latency while maintaining high perceptual quality.

Paper: https://www.isca-archive.org/interspeech_2026/shao26_interspeech.pdf

## Integrity Protection

**StreamMark: A Deep Learning-Based Semi-Fragile Audio Watermarking for Proactive Deepfake Detection**

ICASSP 2026

Zhentao Liu, Milos Cernak

- Introduce a deep learning-based semi-fragile watermark that remains robust to benign, semantics-preserving processing but breaks under malicious, semantics-altering manipulation.
- Use complex-domain embedding and an Encoder-Distortion-Decoder training architecture to distinguish compression, noise, and style transfer from voice conversion, TTS, and speech editing.
- Maintain high imperceptibility and robustness to real-world processing while driving watermark recovery toward chance level after deepfake attacks.

Paper: https://ieeexplore.ieee.org/abstract/document/11463325

**LINGUARD: Authenticating Speech Recordings Using Speech Recognition and Watermark**

ICASSP 2026

Shameer Faziludeen, Arun Sankar M. S., Phillip L. De Leon, Utz Roedig

- Protect linguistic content by signing the speech transcription and linking the signature to the recording through an embedded watermark.
- Combine automatic speech recognition, digital signatures, robust watermarking, and speaker verification to authenticate both content and speaker identity.
- Tolerate benign processing that preserves linguistic content while detecting deletion, insertion, or substitution of speech segments.

Paper: https://ieeexplore.ieee.org/abstract/document/11462384

## Watermark-Free

**Traceable TTS: Toward Watermark-Free TTS with Strong Traceability**

arXiv 2025

Yuxiang Zhao, Yunchong Xiao, Yushen Chen, Zhikang Niu, Shuai Wang, Kai Yu, Xie Chen

- Introduce the first TTS traceability framework that does not rely on explicitly embedding an n-bit watermark into generated speech.
- Jointly train a TTS model and discriminator so the detector can attribute speech to the specific model while preserving audio quality and remaining effective after vocoder replacement.
- Demonstrate improved out-of-domain traceability generalization using F5-TTS without the quality degradation and forgery risks of explicit watermarks.

Paper: https://arxiv.org/pdf/2507.03887
