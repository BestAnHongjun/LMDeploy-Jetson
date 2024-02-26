# LMDeploy-Jetson：Opening a new era of Offline Embodied Intelligence

***Deploying LLMs offline on the NVIDIA Jetson platform marks the dawn of a new era in embodied intelligence, where devices can function independently without continuous internet access.***

[[中文]](./README_zh.md) | [[English]](./README.md)

This project focuses on adapting [LMDeploy](https://github.com/InternLM/lmdeploy) for use with NVIDIA Jetson series edge computing cards, facilitating the implementation of [InternLM](https://github.com/InternLM/InternLM) series LLMs for **Offline Embodied Intelligence (OEI)**.

Demo：[[Bilibili]](https://www.bilibili.com/video/BV1iC411x76Q/)

## Latest News🎉

* [2024/2/26] This project has been included in the [LMDeploy](https://github.com/InternLM/lmdeploy) community.
* [2024/2/25] Updated support for [LMDeploy-v0.2.4](https://github.com/InternLM/lmdeploy/releases/tag/v0.2.4).

## Verified model/platform

* ✅：Verified and runnable
* ❌：Verified but not runnable
* ⭕️：Pending verification

|Models|InternLM-7B|InternLM-20B|InternLM2-1.8B|InternLM2-7B|InternLM2-20B|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Orin NX(16G)<br>Jetpack 5.1|✅<br>Mem:8.6G/16G<br>*7.39 token/s*|✅<br>Mem:14.7G/16G<br>*3.08 token/s*|✅<br>Mem:5.6G/16G<br>*22.96 token/s*|✅<br>Mem:9.2G/16G<br>*7.48 token/s*|✅<br>Mem:14.8G/16G<br>*3.19 token/s*|
|Xavier NX(8G)<br>Jetpack 5.1|❌|❌|✅<br>Mem:4.35G/8G<br>*28.36 token/s*|❌|❌|


**If you have more Jetson series boards, feel free to run benchmarks and submit the results via `Pull Requests` (PR) to become one of the community contributors!**

> Command of Benchmark Test: ```python profile_generation.py ../../models/internlm2-chat-1_8b-turbomind --concurrency 1 --prompt-tokens 128 --completion-tokens 128``` \
> Ref: [lmdeploy/benchmark](https://github.com/InternLM/lmdeploy/blob/main/benchmark/README.md)

## Future Work
* Testing on more Jetson boards such as Nano and AGX.
* ……

## Tutorial
[S1.Quantize on server by W4A16](./en/s1.md)

[S2.Install Miniconda on Jetson](./en/s2.md)

[S3.Install CMake-3.29.0 on Jetson](./en/s3.md)

[S4.Install RapidJson on Jetson](./en/s4.md)

[S5.Install Pytorch-2.1.0 on Jetson](./en/s5.md)

[S6.Port LMDeploy-0.2.4 to Jetson](./en/s6.md)

[S7.Run InternLM offline on Jetson](./en/s7.md)


## Citation

If this project is helpful to your work, please cite it using the following format:

```bibtex
@misc{hongjun2024lmdeployjetson,
    title={LMDeploy-Jetson：Opening a new era of Offline Embodied Intelligence},
    author={LMDeploy-Jetson Community},
    url={https://github.com/BestAnHongjun/LMDeploy-Jetson},
    year={2024}
}
```

## Acknowledgements

* [InternLM Practical Camp](https://github.com/InternLM/tutorial/)
* [Shanghai Artificial Intelligence Laboratory](https://www.shlab.org.cn/)
