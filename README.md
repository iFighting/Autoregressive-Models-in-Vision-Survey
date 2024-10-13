<div align=center>
<img src="img/ARV_logo.png" width="180px">
</div>
<h2 align="center"> Awesome Autoregressive Models in Vision <div align=center> </a></h2>
<h5 align="center"> If you like our project, please give us a star ⭐ on GitHub for the latest update.</h5>

<h5 align="center">


   [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
   [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FChaofanTao%2FAutoregressive-Models-in-Vision-Survey&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
   ![GitHub Repo stars](https://img.shields.io/github/stars/ChaofanTao/Autoregressive-Models-in-Vision-Survey)

</h5>

Autoregressive models have shown significant progress in generating high-quality content by modeling the dependencies sequentially. This repo is a curated list of papers about the latest advancements in autoregressive models in vision. **This repo is being actively updated, please stay tuned!**

## 📣 Update News

`[2024-10-13]` We released the repository.

## ⚡ Contributing

We welcome feedback, suggestions, and contributions that can help improve this survey and repository so as to make them valuable resources to benefit the entire community.
We will actively maintain this repository by incorporating new research as it emerges. If you have any suggestions regarding our taxonomy, find any missed papers, or update any preprint arXiv paper that has been accepted to some venue.

If you want to add your work or model to this list, please do not hesitate to [pull requests]([https://github.com/ChaofanTao/autoregressive-vision-survey/pulls](https://github.com/ChaofanTao/autoregressive-vision-survey/pulls)).
Markdown format:

```markdown
* [**Name of Conference or Journal + Year**] Paper Name. [[paper]](link) [[code]](link)
```

## 📖 Table of Contents
- [📣 Update News](#-update-news)
- [⚡ Contributing](#-contributing)
- [📖 Table of Contents](#-table-of-contents)
  - [Unconditional/Class-Conditioned Image Generation](#unconditionalclass-conditioned-image-generation)
  - [Text-to-Image Generation](#text-to-image-generation)
  - [Image-to-Image Translation](#image-to-image-translation)
  - [Image Editing](#image-editing)
  - [Medical Tasks in Vision](#medical-tasks-in-vision)
  - [Motion Generation](#motion-generation)
  - [Video Generation](#video-generation)
  - [Multi-Modal Tasks](#multi-modal-tasks)
  - [Other Generation](#other-generation)
  - [Accelerating](#accelerating)
  - [Evaluation Metrics](#evaluation-metrics)
- [👍 Acknowledgement](#-acknowledgement)
- [📑 Citation](#-citation)
- [♥️ Contributors](#️-contributors)

### Unconditional/Class-Conditioned Image Generation
  - #### Pixel-wise Generation
    - **[ICML, 2020]** **ImageGPT:** Generative Pretraining from Pixels [Paper](https://proceedings.mlr.press/v119/chen20s/chen20s.pdf)
    - **[ICML, 2018]** **Image Transformer** [Paper](https://arxiv.org/pdf/1802.05751) [Code](https://github.com/neocxi/pixelsnail-public)
    - **[ICML, 2018]** **PixelSNAIL:** An Improved Autoregressive Generative Model [paper](https://proceedings.mlr.press/v80/chen18h/chen18h.pdf) [Code](https://github.com/neocxi/pixelsnail-public)
    - **[ICML, 2017]** Parallel Multiscale Autoregressive Density Estimation [Paper](https://proceedings.mlr.press/v70/reed17a.html)
    - **[ICLR workshop, 2017]** **Gated PixelCNN**: Generating Interpretable Images with Controllable Structure [Paper](https://openreview.net/forum?id=Hyvw0L9el)
    - **[ICLR, 2017]** **PixelCNN++**: Improving the PixelCNN with Discretized Logistic Mixture Likelihood and Other Modifications [Paper](https://arxiv.org/pdf/1701.05517) [Code](https://github.com/openai/pixel-cnn)
    - **[NeurIPS, 2016]** **PixelCNN** Conditional Image Generation with PixelCNN Decoders [Paper](https://arxiv.org/pdf/1606.05328) [Code](https://github.com/anantzoid/Conditional-PixelCNN-decoder)
    - **[ICML,2016]** **PixelRNN** Pixel Recurrent Neural Networks [Paper](https://arxiv.org/pdf/1601.06759) [Code](https://github.com/j-min/PixelCNN)
    
  - #### Token-wise Generation
    - **[Arxiv, 2024.09]** **Open-MAGVIT2**: Democratizing Autoregressive Visual Generation [Paper](https://arxiv.org/pdf/2409.04410) [Code](https://github.com/TencentARC/Open-MAGVIT2)
    - **[Arxiv, 2024.06]** **OmniTokenizer**: A Joint Image-Video Tokenizer for Visual Generation [Paper](https://arxiv.org/pdf/2406.09399) [Code](https://github.com/FoundationVision/OmniTokenizer)
    - **[Arxiv, 2024.06]** Scaling the Codebook Size of VQGAN to 100,000 with a Utilization Rate of 99% [Paper](https://arxiv.org/pdf/2406.11837) [Code](https://github.com/zh460045050/VQGAN-LC)
    - **[Arxiv, 2024.06]** **Titok** An Image is Worth 32 Tokens for Reconstruction and Generation [Paper](https://arxiv.org/pdf/2406.07550) [Code](https://github.com/bytedance/1d-tokenizer)
    - **[Arxiv, 2024.06]** Wavelets Are All You Need for Autoregressive Image Generation*[Tokenizer]* [Paper](https://arxiv.org/pdf/2406.19997) 
    - **[Arxiv, 2024.06]** **LlamaGen** Autoregressive Model Beats Diffusion: Llama for Scalable Image Generation [Paper](https://arxiv.org/pdf/2406.06525) [Code](https://github.com/FoundationVision/LlamaGen)
    - **[ICLR, 2024]**  **MAGVIT-v2** Language Model Beats Diffusion -- Tokenizer is Key to Visual Generation [Paper](https://arxiv.org/pdf/2310.05737)
    - **[ICLR, 2024]** **FSQ** Finite scalar quantization: Vq-vae made simple [Paper](https://arxiv.org/pdf/2309.15505) [Code](https://github.com/google-research/google-research/tree/master/fsq)
    - **[ICCV, 2023]** **Efficient-VQGAN:** Towards High-Resolution Image Generation with Efficient Vision Transformers [Paper](https://arxiv.org/abs/2310.05400)
    - **[CVPR, 2023]** Towards Accurate Image Coding: Improved Autoregressive Image Generation with Dynamic Vector Quantization [Paper](https://arxiv.org/pdf/2305.11718) [Code](https://github.com/CrossmodalGroup/DynamicVectorQuantization)
    - **[CVPR, 2023, Highlight]**  **MAGVIT:** Masked Generative Video Transformer [Paper](https://arxiv.org/pdf/2212.05199)
    - **[AAAI, 2023]** Exploring Stochastic Autoregressive Image Modeling for Visual Representation [Paper](https://arxiv.org/pdf/2212.01610) [Code](https://github.com/qiy20/SAIM)
    - **[NeurIPS, 2023]**  **MoVQ:** Modulating Quantized Vectors for High-Fidelity Image Generation [Paper](https://arxiv.org/pdf/2209.09002)
    - **[BMVC, 2022]**  Unconditional image-text pair generation with multimodal cross quantizer  [Paper](https://arxiv.org/abs/2204.07537) [Code](https://github.com/ttumyche/MXQ-VAE)
    - **[ICLR, 2022]** **ViT-VQGAN** Vector-quantized Image Modeling with Improved VQGAN [Paper](https://arxiv.org/pdf/2110.04627) 
    - **[PMLR, 2021]** Generating images with sparse representations*[Tokenizer]* [Paper](https://arxiv.org/pdf/2103.03841)
    - **[CVPR, 2021]** **VQGAN** Taming Transformers for High-Resolution Image Synthesis [Paper](https://arxiv.org/pdf/2012.09841) [Code](https://github.com/CompVis/taming-transformers)
    - **[NeurIPS, 2019]** Generating Diverse High-Fidelity Images with VQ-VAE-2 [Paper](https://arxiv.org/pdf/1906.00446) [Code](https://github.com/rosinality/vq-vae-2-pytorch)
    - **[NeurIPS, 2017]** **VQ-VAE** Neural Discrete Representation Learning[Paper](https://arxiv.org/pdf/1711.00937)
    - **[Arxiv, 2024.10]** ImageFolder: Autoregressive Image Generation with Folded Tokens [Paper](https://arxiv.org/abs/2410.01756) [Code](https://github.com/lxa9867/ImageFolder)
    - **[Arxiv, 2024.08]** Scalable Autoregressive Image Generation with Mamba [Paper](https://arxiv.org/pdf/2408.12245) [Code](https://github.com/hp-l33/AiM)
    - **[Arxiv, 2024.06]** Autoregressive Pretraining with Mamba in Vision [Paper](https://arxiv.org/abs/2406.07537) [Code](https://github.com/OliverRensu/ARM)
    - **[Arxiv, 2024.06]** Autoregressive Image Generation without Vector Quantization [Paper](https://arxiv.org/pdf/2406.11838) [Code](https://github.com/LTH14/mar)
    - **[Arxiv, 2024.06]** **LlamaGen** Autoregressive Model Beats Diffusion: Llama for Scalable Image Generation [Paper](https://arxiv.org/pdf/2406.06525) [Code](https://github.com/FoundationVision/LlamaGen)
    - **[ICML, 2024]** **DARL**: Denoising Autoregressive Representation Learning [Paper](https://arxiv.org/pdf/2403.05196) 
    - **[ICML, 2024]** **DisCo-Diff**: Enhancing Continuous Diffusion Models with Discrete Latents [Paper](https://arxiv.org/pdf/2407.03300) [Code](https://github.com/gcorso/disco-diffdock)
    - **[ICML, 2024]** **DeLVM**: Data-efficient Large Vision Models through Sequential Autoregression [Paper](https://arxiv.org/pdf/2402.04841) [Code](https://github.com/ggjy/DeLVM)
    - **[CVPR, 2024]** **Beyond Text**: Frozen Large Language Models in Visual Signal Comprehension [Paper](https://arxiv.org/pdf/2403.07874) [Code](https://github.com/zh460045050/V2L-Tokenizer)
    - **[ICLR, 2024]** Finite Scalar Quantization: VQ-VAE Made Simple [Paper](https://arxiv.org/pdf/2309.15505) [Code](https://github.com/Nikolai10/FSQ)
    - **[NeurIPS, 2021]** **ImageBART**: Context with Multinomial Diffusion for Autoregressive Image Synthesis [Paper](https://arxiv.org/pdf/2108.08827) [Code](https://github.com/CompVis/imagebart)
    - **[CVPR, 2021]** **VQGAN** Taming Transformers for High-Resolution Image Synthesis [Paper](https://arxiv.org/pdf/2012.09841)  [Code](https://github.com/CompVis/taming-transformers)
    - **[ECCV, 2020]** **RAL**: Incorporating Reinforced Adversarial Learning in Autoregressive Image Generation [Paper](https://arxiv.org/pdf/2007.09923)
    - **[NeurIPS, 2019]** Generating Diverse High-Fidelity Images with VQ-VAE-2 [Paper](https://arxiv.org/pdf/1906.00446) [Code](https://github.com/rosinality/vq-vae-2-pytorch)
    - **[NeurIPS, 2017]** **VQ-VAE** Neural Discrete Representation Learning[Paper](https://arxiv.org/pdf/1711.00937)
    
  - #### Scale-wise Generation
    - **[CVPR, 2022]** **RQ-Transformer** Autoregressive Image Generation Using Residual Quantization [Paper](https://arxiv.org/pdf/2203.01941) [Code](https://github.com/kakaobrain/rq-vae-transformer)  
    - **[Arxiv, 2024.04]** **Visual Autoregressive Modeling:** Scalable Image Generation via Next-Scale Prediction [Paper](https://arxiv.org/pdf/2404.02905) [Code](https://github.com/FoundationVision/VAR)
    
### Text-to-Image Generation
  - **[Arxiv, 2024.10]** **DART**: Denoising Autoregressive Transformer for Scalable Text-to-Image Generation [Paper](https://arxiv.org/abs/2410.08159) [Code](https://github.com/daixiangzi/VAR-CLIP)
  - **[Arxiv, 2024.08]** **VAR-CLIP**: Text-to-Image Generator with Visual Auto-Regressive Modeling [Paper](https://arxiv.org/pdf/2408.01181) [Code](https://github.com/daixiangzi/VAR-CLIP)
  - **[Arxiv, 2024.08]** **Lumina-mGPT**: Illuminate Flexible Photorealistic Text-to-Image Generation with Multimodal Generative Pretraining [Paper](https://arxiv.org/pdf/2408.02657) [Code](https://github.com/Alpha-VLLM/Lumina-mGPT)
  - **[Arxiv, 2024.07]** **MARS**: Mixture of Auto-Regressive Models for Fine-grained Text-to-image Synthesis [Paper](https://arxiv.org/pdf/2407.07614) [Code](https://github.com/fusiming3/MARS)
  - **[Arxiv, 2024.06]** **LLM4GEN**: Leveraging Semantic Representation of LLMs for Text-to-Image Generation [Paper](https://arxiv.org/pdf/2407.00737) [Code](https://github.com/YUHANG-Ma/LLM4GEN)
  - **[Arxiv, 2024.06]** **STAR**: Scale-wise Text-to-image generation via Auto-Regressive representations [Paper](https://arxiv.org/pdf/2406.10797) [Code](https://github.com/krennic999/STAR)
  - **[Arxiv, 2024.05]** **Kaleido Diffusion**: Improving Conditional Diffusion Models with Autoregressive Latent Modeling [Paper](https://arxiv.org/pdf/2405.21048) 
  - **[TOG, 2023]** **IconShop**: Text-Guided Vector Icon Synthesis with Autoregressive Transformers (*svg image*) [Paper](https://arxiv.org/pdf/2304.14400) [Code](https://github.com/kingnobro/IconShop)
  - **[NeurIPS, 2023]** **LQAE** Language Quantized AutoEncoders: Towards Unsupervised Text-Image Alignment [Paper](https://arxiv.org/pdf/2302.00902) [Code](https://github.com/lhao499/language-quantized-autoencoders)
  - **[TMLR, 2022.06]** **Parti**: Scaling Autoregressive Models for Content-Rich Text-to-Image Generation [Paper](https://arxiv.org/pdf/2206.10789) [Code](https://github.com/google-research/parti)
  - **[NeurIPS, 2022]** **CogView2**: Faster and Better Text-to-Image Generation via Hierarchical Transformers [Paper](https://arxiv.org/pdf/2204.14217) [Code](https://github.com/THUDM/CogView2)
  - **[ECCV, 2022]** **Make-A-Scene:** Scene-Based Text-to-Image Generation with Human Priors [Paper](https://arxiv.org/pdf/2203.13131) 
  - **[CVPR, 2022]** **VQ-Diffusion:** Vector Quantized Diffusion Model for Text-to-Image Synthesis [Paper](https://openaccess.thecvf.com/content/CVPR2022/html/Gu_Vector_Quantized_Diffusion_Model_for_Text-to-Image_Synthesis_CVPR_2022_paper.html) [Code](https://github.com/cientgu/VQ-Diffusion)
  - **[CVPR, 2022]** **Make-A-Story:** Visual Memory Conditioned Consistent Story Generation (*storytelling*) [Paper](https://arxiv.org/pdf/2211.13319) 
  - **[NeurIPS, 2021]** **CogView**: Mastering Text-to-Image Generation via Transformers [Paper](https://arxiv.org/pdf/2105.13290) [Code](https://github.com/THUDM/CogView)
  - **[Arxiv, 2021.02]** **DALL-E 1:** Zero-Shot Text-to-Image Generation [Paper](https://arxiv.org/pdf/2102.12092)
   
### Image-to-Image Translation
  - **[Arxiv, 2024,06]** CAR: Controllable Autoregressive Modeling for Visual Generation [Paper](https://arxiv.org/abs/2410.04671) [Code](https://github.com/MiracleDance/CAR)
  - **[Arxiv, 2024,06]** ControlAR: Controllable Image Generation with Autoregressive Models [Paper](https://arxiv.org/abs/2410.02705) [Code](https://github.com/hustvl/ControlAR)
  - **[Arxiv, 2024,06]** **ControlVAR**: Exploring Controllable Visual Autoregressive Modeling [Paper](https://arxiv.org/pdf/2406.09750) [Code](https://github.com/lxa9867/ControlVAR)
  - **[ICML Workshop, 2024]** **MIS** Many-to-many Image Generation with Auto-regressive Diffusion Models [Paper](https://arxiv.org/pdf/2404.03109) 
  - **[Arxiv, 2024.03]** **SceneScript**: Reconstructing Scenes With An Autoregressive Structured Language Model [Paper](https://arxiv.org/pdf/2403.13064) [Project](https://www.projectaria.com/scenescript/)


### Image Editing 
  - **[ECCV, 2022]** **VQGAN-CLIP:** Open Domain Image Generation and Editing with Natural Language Guidance [Paper](https://arxiv.org/pdf/2204.08583)
  - **[ECCV, 2022]** **Make-A-Scene:** Scene-Based Text-to-Image Generation with Human Priors [Paper](https://arxiv.org/pdf/2203.13131)
  - **[NeurIPS, 2021]** **ImageBART**: Context with Multinomial Diffusion for Autoregressive Image Synthesis [Paper](https://arxiv.org/pdf/2108.08827) [Code](https://github.com/CompVis/imagebart)
  - **[ECCV, 2022]** **QueryOTR**: Outpainting by Queries [Paper](https://arxiv.org/pdf/2207.05312) [Code](https://github.com/Kaiseem/QueryOTR)
  
### Medical Tasks in Vision
  - **[arxiv, 2024]** Autoregressive Sequence Modeling for 3D Medical Image Representation [paper](https://arxiv.org/pdf/2409.08691v1) 
  - **[arxiv, 2024]** Medical Vision Generalist: Unifying Medical Imaging Tasks in Context [paper](https://arxiv.org/pdf/2406.05565) [code](https://arxiv.org/pdf/2406.05565)
  - **[MIDL, 2024]** Conditional Generation of 3D Brain Tumor ROIs via VQGAN and Temporal-Agnostic Masked Transformer [paper](https://openreview.net/pdf?id=LLoSHPorlM)
  - **[NMI, 2024]** Realistic morphology-preserving generative modelling of the brain [paper](https://www.nature.com/articles/s42256-024-00864-0) [code](https://github.com/AmigoLab/BrainSynth)
  - **[Arxiv, 2023]** Generating 3D Brain Tumor Regions in MRI using Vector-Quantization Generative Adversarial Networks [paper](https://arxiv.org/pdf/2310.01251)
  ```medical image-to-image translation```
  - **[ICCV, 2023]** Unaligned 2D to 3D Translation with Conditional Vector-Quantized Code Diffusion using Transformers [paper](https://openaccess.thecvf.com/content/ICCV2023/papers/Corona-Figueroa_Unaligned_2D_to_3D_Translation_with_Conditional_Vector-Quantized_Code_Diffusion_ICCV_2023_paper.pdf) [Code](https://github.com/samb-t/x2ct-vqvae)
  - **[MICCAI, 2022]** Morphology-preserving Autoregressive 3D Generative Modelling of the Brain [paper](https://arxiv.org/pdf/2209.03177) [code](https://github.com/AmigoLab/SynthAnatomy)
  ```medical image generation```
  - **[ICIP, 2021]** Generating Annotated High-Fidelity Images Containing Multiple Coherent Objects [paper](https://arxiv.org/pdf/2006.12150) [Code](https://github.com/Cynetics/MSGNet/)

### Motion Generation
  - **[AAAI, 2024]** **AMD**: Autoregressive Motion Diffusion [Paper](https://arxiv.org/pdf/2305.09381) [Code]()
  - **[CVPR, 2023]**  **T2M-GPT**: Generating Human Motion from Textual Descriptions with Discrete Representations [Paper](https://arxiv.org/pdf/2301.06052)
  - **[Arxiv, 2022]** **HiT-DVAE**: Human Motion Generation via Hierarchical Transformer Dynamical VAE [Paper](https://arxiv.org/pdf/2204.01565)
  - **[ICCV, 2021 oral]** **HuMoR**: 3D Human Motion Model for Robust Pose Estimation [Paper](https://geometry.stanford.edu/projects/humor/docs/humor.pdf) [Code](https://github.com/davrempe/humor)
  

### Video Generation

 - #### Unconditional Video Generation
    - **[ICML, 2017]** Video Pixel Networks [Paper](https://proceedings.mlr.press/v70/kalchbrenner17a.html?ref=https://githubhelp.com)
    - **[CVPR, 2018]** **MoCoGAN**: Decomposing Motion and Content for Video Generation [paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Tulyakov_MoCoGAN_Decomposing_Motion_CVPR_2018_paper.pdf) [Code](https://github.com/sergeytulyakov/mocogan)
    - **[ICLR, 2020]** Scaling Autoregressive Video Models [paper](https://arxiv.org/pdf/1906.02634) 
    - **[Arxiv, 2020.06]** Latent Video Transformer [paper](https://arxiv.org/pdf/2006.10704) [Code](https://github.com/rakhimovv/lvt)
    - **[Arxiv, 2021.04]** **VideoGPT**: Video generation using VQ-VAE and transformers [paper](https://arxiv.org/pdf/2209.07143) 
    - **[ECCV, 2022]**  Long Video Generation with Time-Agnostic VQGAN and Time-Sensitive Transformer [Paper](https://arxiv.org/pdf/2204.03638) [Code](https://github.com/SongweiGe/TATS)
    - **[CVPR, 2023]** **PVDM** Video Probabilistic Diffusion Models in Projected Latent Space [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Yu_Video_Probabilistic_Diffusion_Models_in_Projected_Latent_Space_CVPR_2023_paper.html)
    - **[ECCV 2024]** **ST-LLM**: Large Language Models Are Effective Temporal Learners [Paper](https://arxiv.org/pdf/2404.00308) [Code](https://github.com/TencentARC/ST-LLM)
    - **[ICLR, 2024]**  **MAGVIT-v2** Language Model Beats Diffusion -- Tokenizer is Key to Visual Generation [Paper](https://arxiv.org/pdf/2310.05737)

 - #### Conditional Video Generation
   - ##### Text-to-Video Generation
     - **[IJCAI, 2021]** **IRC-GAN**: Introspective Recurrent Convolutional GAN for Text-to-video Generation. [paper](https://www.ijcai.org/Proceedings/2019/0307.pdf)
     - **[Arxiv, 2022.05]** **GODIVA**: Generating Open-DomaIn Videos from nAtural Descriptions [paper](https://arxiv.org/pdf/2104.14806)
     - **[Arxiv, 2022.05]** **CogVideo**: Large-scale Pretraining for Text-to-Video Generation via Transformers [paper](https://arxiv.org/pdf/2205.15868) [Code](https://github.com/THUDM/CogVideo)
     - **[ECCV, 2022]** **NÜWA**: Visual Synthesis Pre-training for Neural visUal World creAtion [paper](https://arxiv.org/pdf/2111.12417) [Code](https://github.com/microsoft/NUWA)
     - **[NeurIPS, 2022]** **NUWA-Infinity**: Autoregressive over Autoregressive Generation for Infinite Visual Synthesis [paper](https://arxiv.org/pdf/2207.09814) [Code](https://github.com/microsoft/NUWA)
     - **[CVPR, 2024]** **ART-V**: Auto-Regressive Text-to-Video Generation with Diffusion Models [paper](https://arxiv.org/pdf/2311.18834) 
     - **[arxiv, 2024.02]** **Video-LaVIT**:  Unified Video-Language Pre-training with Decoupled Visual-Motional Tokenization [paper](https://arxiv.org/pdf/2402.03161) [code](https://github.com/jy0205/LaVIT)
     - **[Arxiv, 2024.02]** **LWM** World Model on Million-Length Video And Language With Blockwise RingAttention [Paper](https://arxiv.org/pdf/2402.08268) [Code](https://github.com/LargeWorldModel/LWM)
     - **[Arxiv, 2024.06]** **ViD-GPT**: Introducing GPT-style Autoregressive Generation in Video Diffusion Models [paper](https://arxiv.org/pdf/2406.10981) [Code](https://github.com/Dawn-LX/Causal-VideoGen)
     - **[Arxiv, 2024.06]** **iVideoGPT**: Interactive VideoGPTs are Scalable World Models [Paper](https://arxiv.org/pdf/2405.15223) [Code](https://github.com/thuml/iVideoGPT)
     - **[Arxiv, 2024.06]**  **Pandora**: Towards General World Model with Natural Language Actions and Video States [Paper](https://arxiv.org/pdf/2406.09455) [Code](https://github.com/maitrix-org/Pandora)
     - **[Arxiv, 2024.10]**  **Loong**: Generating Minute-level Long Videos with Autoregressive Language Models [Paper](https://arxiv.org/pdf/2410.02757)
     - **[Arxiv, 2024.10]**  Progressive Autoregressive Video Diffusion Models [Paper](https://arxiv.org/abs/2410.08151) [Code](https://github.com/desaixie/pa_vdm)
         
   - ##### Visual Conditional Video Generation
     - **[NeurIPS, 2015]** Convolutional LSTM network: A machine learning approach for precipitation nowcasting [paper](https://proceedings.neurips.cc/paper/2015/file/07563a3fe3bbe7e3ba84431ad9d055af-Paper.pdf)
     - **[NeurIPS, 2017]** **Predrnn**: Recurrent neural networks for predictive learning using spatiotemporal lstms [paper](https://proceedings.neurips.cc/paper_files/paper/2017/file/e5f6ad6ce374177eef023bf5d0c018b6-Paper.pdf)
     - **[ICLR, 2019]** Eidetic 3d lstm: A model for video prediction and beyond [paper](https://openreview.net/pdf?id=B1lKS2AqtX)
     - **[ICLR, 2018]** Stochastic variational video prediction [paper](https://openreview.net/pdf?id=rk49Mg-CW) 
     - **[CVPR, 2021]** Stochastic image-to-video synthesis using cinns [paper](http://openaccess.thecvf.com/content/CVPR2021/papers/Dorkenwald_Stochastic_Image-to-Video_Synthesis_Using_cINNs_CVPR_2021_paper.pdf) [Code](https://github.com/CompVis/image2video-synthesis-using-cINNs)
     - **[Arxiv, 2021.03]** Predicting Video with VQVAE [paper](https://arxiv.org/pdf/2103.01950)
     - **[ICIP, 2022]** **HARP**: Autoregressive Latent Video Prediction with High-Fidelity Image Generator [paper](https://arxiv.org/pdf/2209.07143)
     - **[CVPR, 2024]**  **LVM** Sequential Modeling Enables Scalable Learning for Large Vision Models [Paper](https://arxiv.org/pdf/2312.00785) [Code](https://github.com/ytongbai/LVM)

   - ##### Multimodal Conditional Video Generation
     - **[CVPR, 2022]** Make it move: controllable image-to-video generation with text descriptions [paper](http://openaccess.thecvf.com/content/CVPR2022/papers/Hu_Make_It_Move_Controllable_Image-to-Video_Generation_With_Text_Descriptions_CVPR_2022_paper.pdf) [Code](https://github.com/Youncy-Hu/MAGE)
     - **[CVPR, 2023]** **MAGVIT**: Masked Generative Video Transformer [paper](https://arxiv.org/pdf/2212.05199)
     - **[ICML, 2024]** **VideoPoet**: A Large Language Model for Zero-Shot Video Generation [paper](https://arxiv.org/pdf/2312.14125)
    
### Multi-Modal Tasks
  - **[Arxiv, 2024.10]** vACDC: Autoregressive Coherent Multimodal Generation using Diffusion Correction [paper](https://arxiv.org/pdf/2410.04721) [Code](https://acdc2025.github.io/)
  - **[Arxiv, 2024.08]** **Show-o:** One Single Transformer to Unify Multimodal Understanding and Generation [paper](https://arxiv.org/pdf/2408.12528) [Code](https://github.com/showlab/Show-o)
  - **[Arxiv, 2024.08]** **Transfusion:** Predict the Next Token and Diffuse Images with One Multi-Modal Model [paper](https://arxiv.org/pdf/2408.11039) [Code](https://github.com/lucidrains/transfusion-pytorch)
  - **[Arxiv, 2024.07]** **SEED-Story**: Multimodal Long Story Generation with Large Language Model [Paper](https://arxiv.org/pdf/2407.08683) [Code](https://github.com/TencentARC/SEED-Story)
  - **[Arxiv, 2024.05]**  **Chameleon**: Mixed-Modal Early-Fusion Foundation Models [paper](https://arxiv.org/pdf/2405.09818) [Code](https://github.com/facebookresearch/chameleon)
  - **[Arxiv, 2024.04]** **SEED-X** Multimodal Models with UnifiedMulti-granularity Comprehension and Generation [Paper](https://arxiv.org/pdf/2404.14396) [Code](https://github.com/AILab-CVC/SEED-X)
  - **[ICML, 2024]** **Libra**: Building Decoupled Vision System on Large Language Models [paper](https://arxiv.org/pdf/2405.10140) [Code](https://github.com/YifanXu74/Libra)
  - **[CVPR, 2024]** **Unified-IO 2**: Scaling Autoregressive Multimodal Models with Vision Language Audio and Action[paper](https://arxiv.org/pdf/2312.17172) [Code](https://github.com/allenai/unified-io-2)
  - **[CVPR, 2024]** **Anole**: An Open, Autoregressive and Native Multimodal Models for Interleaved Image-Text Generation [paper](https://arxiv.org/pdf/2407.06135) [Code](https://github.com/GAIR-NLP/anole)
  - **[Arxiv, 2023.11]** **InstructSeq**: Unifying Vision Tasks with Instruction-conditioned Multi-modal Sequence Generation [paper](https://arxiv.org/pdf/2311.18835) [Code](https://github.com/rongyaofang/InstructSeq)
  - **[ICLR, 2024]** **Kosmos-G**: Generating Images in Context with Multimodal Large Language Models [Paper](https://arxiv.org/pdf/2310.02992) [Code](https://github.com/xichenpan/Kosmos-G)
  - **[ICLR, 2024]** **LaVIT**: Unified Language-Vision Pretraining in LLM with Dynamic Discrete Visual Tokenization [paper](https://arxiv.org/pdf/2309.04669) [code](https://github.com/jy0205/LaVIT)
  - **[ICLR, 2024]** **SEED-LLaMA** Making LLaMA SEE and Draw with SEED Tokenizer [Paper](https://arxiv.org/pdf/2310.01218) [Code](https://github.com/AILab-CVC/SEED)
  - **[ICLR, 2024]** **EMU** Generative Pretraining in Multimodality [Paper](https://arxiv.org/pdf/2307.05222) [Code](https://github.com/baaivision/Emu)
  - **[Arxiv, 2023.09]** **CM3Leon:** Scaling Autoregressive Multi-Modal Models: Pretraining and Instruction Tuning [Paper](https://arxiv.org/pdf/2309.02591) [Code](https://github.com/kyegomez/CM3Leon)
  - **[Arxiv, 2023.07]** **SEED** Planting a SEED of Vision in Large Language Model [Paper](https://arxiv.org/pdf/2307.08041) [Code](https://github.com/AILab-CVC/SEED)
  - **[NeurIPS, 2023]** **SPAE**: Semantic Pyramid AutoEncoder for Multimodal Generation with Frozen LLMs[paper](https://arxiv.org/pdf/2306.17842)
  - **[ICLR, 2023]** **Unified-IO**: A unified model for vision, language, and multi-modal tasks [paper](https://arxiv.org/pdf/2206.08916) [Code](https://unified-io.allenai.org/)
  - **[ICML, 2023]** Grounding Language Models to Images for Multimodal Inputs and Outputs [paper](https://arxiv.org/pdf/2301.13823) [Code](https://github.com/kohjingyu/fromage)
  - **[Arxiv, 2021.12]** **ERNIE-ViLG**: Unified Generative Pre-training for Bidirectional Vision-Language Generation [Paper](https://arxiv.org/pdf/2112.15283) 
  - **[KDD, 2021]** **M6:** A Chinese Multimodal Pretrainer [Paper](https://arxiv.org/pdf/2103.00823)
  
### Other Generation
  - **[Arxiv, 2024.10]** DART: A Diffusion-Based Autoregressive Motion Model for Real-Time Text-Driven Motion Control [Paper](https://carxiv.org/pdf/2410.05260)
  - **[Arxiv, 2024.07]** Video In-context Learning [Paper](https://arxiv.org/pdf/2407.07356)
  - **[CVPR, 2024]** Sequential Modeling Enables Scalable Learning for Large Vision Models [Paper](https://arxiv.org/pdf/2312.00785) [Code](https://github.com/ytongbai/LVM)
  - **[AAAI, 2024]** Autoregressive Omni-Aware Outpainting for Open-Vocabulary 360-Degree Image Generation [Paper](https://arxiv.org/pdf/2309.03467) [Code](https://github.com/zhuqiangLu/AOG-NET-360)
  - **[arxiv, 2024]** **LM4LV**: A Frozen Large Language Model for Low-level Vision Tasks [paper](https://arxiv.org/pdf/2405.15734) [code](https://github.com/bytetriper/LM4LV)
  - **[CVPR, 2023]** **Visual Chain of Thought**: Bridging Logical Gaps with Multimodal Infillings [Paper](https://arxiv.org/pdf/2305.02317) 
  - **[ECCV, 2022]** Autoregressive 3D Shape Generation via Canonical Mapping [Paper](https://arxiv.org/pdf/2204.01955)
  - **[NeurIPS, 2022]** **Flamingo**: a Visual Language Model for Few-Shot Learning [Paper](https://arxiv.org/pdf/2204.14198)
  - **[NeurIPS, 2022]** Visual Prompting via Image Inpainting [Paper](https://arxiv.org/pdf/2209.00647) [Code](https://github.com/amirbar/visual_prompting)
  - **[EMNLP, 2022]** **MAGMA** – Multimodal Augmentation of Generative Models through Adapter-based Finetuning [Paper](https://arxiv.org/pdf/2112.05253)
  - **[NeurIPS, 2021]** Multimodal Few-Shot Learning with Frozen Language Models [Paper](https://arxiv.org/pdf/2106.13884)
  - **[ECCV, 2020]** Autoregressive Unsupervised Image Segmentation [paper](https://arxiv.org/pdf/2007.08247)

### Accelerating
  - **[Arxiv, 2024.10]** Accelerating Auto-regressive Text-to-Image Generation with Training-free Speculative Jacobi Decoding [Paper](https://arxiv.org/abs/2410.01699)
  - **[Arxiv, 2024.09]** Pre-trained Language Models Do Not Help Auto-regressive Text-to-Image Generation [Paper](https://arxiv.org/pdf/2311.16201)
  

### Evaluation Metrics
| Metric Name                        | Quantitative or Qualitative | Higher is better↑ / Lower is better↓ | Paper proposing the metric                            |
|-------------------------------------|-----------------------------|--------------------------------------|------------------------------------------------------|
| Inception Score (IS)                | Quantitative                | ↑                                    | [Salimans et al., 2016](https://arxiv.org/pdf/1606.03498)                                |
| Fréchet Inception Distance (FID)    | Quantitative                | ↓                                    | [Heusel et al., 2017](https://arxiv.org/pdf/1706.08500)                                  |
| Kernel Inception Distance (KID)     | Quantitative                | ↓                                    | [Binkowski et al., 2018](https://arxiv.org/pdf/1801.01401)                               |
| Precision and Recall                | Quantitative                | Depends on metric                    | [Powers, 2020](https://arxiv.org/pdf/2010.16061)                                 |
| CLIP Maximum Mean Discrepancy         | Quantitative                | ↓                                    | [Jayasumana et al., 2023](https://arxiv.org/pdf/2401.09603)                           |
| CLIP Score                          | Quantitative                | ↑                                    | [Hessel et al., 2021](https://arxiv.org/pdf/2104.08718)                                 |
| R-precision                         | Quantitative                | ↑                                    | [Craswell et al., 2009](https://doi.org/10.1007/978-0-387-39940-9_486)                                      |
| Perceptual Path Length              | Quantitative                | ↓                                    | [Karras et al., 2019](https://arxiv.org/pdf/1812.04948)                                  |
| Fréchet Video Distance (FVD)        | Quantitative                | ↓                                    | [Unterthiner et al., 2019](https://arxiv.org/pdf/1812.01717)                             |
| Aesthetic (Expert Evaluation)       | Qualitative                 | ↑                                    | Based on domain expertise                            |
| Turing Test                         | Qualitative                 | Pass/fail                            | [Turing, 1950](https://academic.oup.com/mind/article/LIX/236/433/986238)                                         |
| User Studies (ratings, satisfaction)| Qualitative                 | ↑                                    | Various, depending on the user study methodology     |

## ♥️ Contributors

<a href="https://github.com/ChaofanTao/Autoregressive-Models-in-Vision-Survey/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ChaofanTao/Autoregressive-Models-in-Vision-Survey" />
</a>

<!--
## 👍 Acknowledgement
To be continued

## 📑 Citation

Please consider citing 📑 our papers if our repository is helpful to your work, thanks sincerely!

```BibTeX
To be continued
–->

