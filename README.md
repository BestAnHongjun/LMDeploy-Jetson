# LMDeploy-Jetson：Opening a new era of Offline Embodied Intelligence

***Deploying LLMs offline on the NVIDIA Jetson platform marks the dawn of a new era in embodied intelligence, where devices can function independently without continuous internet access.***

[[中文]](./README_zh.md) | [[English]](./README.md)

This project focuses on adapting [LMDeploy](https://github.com/InternLM/lmdeploy) for use with NVIDIA Jetson series edge computing cards, facilitating the implementation of [InternLM](https://github.com/InternLM/InternLM) series LLMs for **Offline Embodied Intelligence (OEI)**.

Demo：[[Bilibili]](https://www.bilibili.com/video/BV1iC411x76Q/)

## Verified model/platform

* ✅：Verified and runnable
* ❌：Verified but not runnable
* ⭕️：Pending verification

|Models|InternLM-7B|InternLM-20B|InternLM2-1.8B|InternLM2-7B|InternLM2-20B|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Orin NX(16G)<br>Jetpack 5.1|✅<br>Mem:8.6G/16G|✅<br>Mem:14.7G/16G|✅<br>Mem:5.6G/16G|✅<br>Mem:9.2G/16G|✅<br>Mem:14.8G/16G|
|Xavier NX(8G)<br>Jetpack |⭕️|⭕️|⭕️|⭕️|⭕️|

## Future Work
* Testing the benchmark inference speed of various LLMs on the Jetson platform.
* Testing on more Jetson boards such as Nano and Xavier NX.
* ……

## Tutorial
[S1.Quantize on server by W4A16](./zh/s1.md)

[S2.Install Miniconda on Jetson](./zh/s2.md)

[S3.Install CMake-3.29.0 on Jetson](./zh/s3.md)

[S4.Install RapidJson on Jetson](./zh/s4.md)

[S5.Install Pytorch-2.1.0 on Jetson](./zh/s5.md)

[S6.Port LMDeploy-2.3.0 to Jetson](./zh/s6.md)

[S7.Run InternLM offline on Jetson](./zh/s7.md)


## Citation

If this project is helpful to your work, please cite it using the following format:

```bibtex
@misc{hongjun2024lmdeployjetson,
    title={LMDeploy-Jetson：Opening a new era of Offline Embodied Intelligence},
    author={Hongjun An},
    url={https://github.com/BestAnHongjun/LMDeploy-Jetson},
    year={2024}
}
```

## Acknowledgements

* The [InternLM Practical Camp](https://github.com/InternLM/tutorial/) organized by the [Shanghai Artificial Intelligence Laboratory](https://www.shlab.org.cn/) has provided valuable learning materials and computational resources for my study of LLM-related theories and technologies. Teachers have also provided tremendous assistance to me. I hereby express my sincere gratitude to all of them!

## Institution

**Hongjun An**, Ph.D. Student, School of Artificial Intelligence, Optics and ElectroNics (iOPEN)
> Email: an.hongjun@foxmail.com \
> Page: www.anhongjun.top

<div align="center">
<img src="./attach/logo.jpg" width="500px">
</div>