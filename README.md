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
|2025|Interspeech|WAKE: Watermarking Audio with Key Enrichment|Post-Processing|[Paper](https://arxiv.org/pdf/2506.05891)|-|
|2025|ICML|XAttnMark: Learning Robust Audio Watermarking with Cross-Attention|Post-Processing|[Paper](https://arxiv.org/pdf/2502.04230)|[Code](https://liuyixin-louis.github.io/xattnmark/)|
|2025|ArXiv|GenMark: An Embedded Watermarking Scheme for Generative Audio Synthesis|Generative|[Paper](https://openreview.net/pdf?id=x9I1V6JY0r)|[Code](https://anonymous.4open.science/r/Gen-Mark-1F27/README.md)|
|2025|ArXiv|SoK: How Robust is Audio Watermarking in Generative AI models?|Benchmark|[Paper](https://arxiv.org/pdf/2503.19176)|[Code](https://sokaudiowm.github.io/)|


## Post-Processing

**WavMark: Watermarking for Audio Generation**

ArXiv 2023

Guangyu Chen, Yu Wu, Shujie Liu, Tao Liu, Xiaoyong Du, Furu Wei

- Early neural audio watermark baseline

- Use invertible neural networks (INN) to add watermark in the STFT domain

- Bias the audio branch via message-conditioned coupling, with 32-bit payload per 1-second audio segment

Paper: https://arxiv.org/pdf/2308.12770

Code: https://github.com/wavmark/wavmark

**WAKE: Watermarking Audio with Key Enrichment**

Interspeech 2025

Yaoxun Xu, Jianwei Yu, Hangting Chen, Zhiyong Wu, Xixin Wu, Dong Yu, Rongzhi Gu, Yi Luo

- Key Enrichment: message + secret key $\rightarrow$ enriched watermark
- Add authentication inot into the watermark

Paper: https://arxiv.org/pdf/2506.05891

**XAttnMark: Learning Robust Audio Watermarking with Cross-Attention**

ICML 2025

Yixin Liu, Lie Lu, Jihui Jin, Lichao Sun, Andrea Fanelli

- audio feature $\rightarrow$ cross-attention (message embedding) $\rightarrow$ watermarked audio
- More robust to complex attack

Paper: https://arxiv.org/pdf/2502.04230

Code: https://liuyixin-louis.github.io/xattnmark/

## Generative

**Proactive Detection of Voice Cloning with Localized Watermarking (AudioSeal)**

ICML 2024

Robin San Roman, Pierre Fernandez, Hady Elsahar, Alexandre Défossez, Teddy Furon, Tuan Tran

- Active method for AI voice detection (voice cloning detection)
- Localized Watermark: Watermark distributed in local time frames

Paper: https://arxiv.org/pdf/2401.17264

Code: https://github.com/facebookresearch/audioseal

**TraceableSpeech: Towards Proactively Traceable Text-to-Speech with Watermarking**

InterSpeech 2024

Junzuo Zhou, Jiangyan Yi, Tao Wang, Jianhua Tao, Ye Bai, Chu Yuan Zhang, Yong Ren, Zhengqi Wen

Paper: https://arxiv.org/pdf/2406.04840

Code: https://github.com/zjzser/TraceableSpeech

**GenMark: An Embedded Watermarking Scheme for Generative Audio Synthesis**

ArXiv 2025

Zihao Zhang, Wenlong Meng, Chen Gong, Guo Zhenyuan, Kui Su, Zunlei Feng, Chengkun Wei, Wenzhi Chen

- Embedding Watermark: Integrate watermark imbedding in the diffusion / generative pipeline
- More stable and less removable watermark

Paper: https://openreview.net/pdf?id=x9I1V6JY0r

Code: https://anonymous.4open.science/r/Gen-Mark-1F27/README.md

## Benchmark / Surveys

**AudioMarkBench: Benchmarking Robustness of Audio Watermarking**

NeurIPS 2024 Track on Datasets and Benchmarks

Hongbin Liu, Moyang Guo, Zhengyuan Jiang, Lun Wang, Neil Zhenqiang Gong

Introduce a unified benchmarking pipeline that simulates diverse real-world and adversarial audio transformations and evaluates watermark extraction reliability using BER-based statistical analysis and robustness curves across attack intensities.

Paper: https://proceedings.neurips.cc/paper_files/paper/2024/file/5d9b7775296a641a1913ab6b4425d5e8-Paper-Datasets_and_Benchmarks_Track.pdf

Code: https://github.com/mileskuo42/AudioMarkBench

**SoK: How Robust is Audio Watermarking in Generative AI models?**

ArXiv 2025

Yizhu Wen, Ashwin Innuganti, Aaron Bien Ramos, Hanqing Guo, Qiben Yan

Paper: https://arxiv.org/pdf/2503.19176

Code: https://sokaudiowm.github.io/
