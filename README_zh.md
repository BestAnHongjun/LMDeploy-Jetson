# LMDeploy-Jetson：Opening a new era of Offline Embodied Intelligence

***在NVIDIA Jetson平台离线部署大模型，开启离线具身智能新纪元。***

[[中文]](./README_zh.md) | [[English]](./README.md)

本项目提供一种将[LMDeploy](https://github.com/InternLM/lmdeploy)移植到NVIDIA Jetson系列边缘计算卡的方法，并在Jetson计算卡上运行[InternLM](https://github.com/InternLM/InternLM)系列大模型，为**离线具身智能**提供可能。

演示视频：[[Bilibili]](https://www.bilibili.com/video/BV1iC411x76Q/)

## 已验证模型/平台

* ✅：已验证可运行
* ❌：已验证不可运行
* ⭕️：待验证

|Models|InternLM-7B|InternLM-20B|InternLM2-1.8B|InternLM2-7B|InternLM2-20B|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Orin NX(16G)<br>Jetpack 5.1|✅<br>Mem:8.6G/16G<br>*7.39 token/s*|✅<br>Mem:14.7G/16G<br>*3.08 token/s*|✅<br>Mem:5.6G/16G<br>*22.96 token/s*|✅<br>Mem:9.2G/16G<br>*7.48 token/s*|✅<br>Mem:14.8G/16G<br>*3.19 token/s*|
|Xavier NX(8G)<br>Jetpack 5.1|❌|❌|✅<br>Mem:4.35G/8G<br>*28.36 token/s*|❌|❌|

> 基准测试指令: ```python profile_generation.py ../../models/internlm2-chat-1_8b-turbomind --concurrency 1 --prompt-tokens 128 --completion-tokens 128``` \
> 参考: [lmdeploy/benchmark](https://github.com/InternLM/lmdeploy/blob/main/benchmark/profile_generation.py)

## 未来工作
* 在Nano/Xavier NX等更多Jetson板卡测试
* ……

## 部署教程
[S1.服务器端模型W4A16量化](./zh/s1.md)

[S2.Jetson端安装Miniconda](./zh/s2.md)

[S3.Jetson端安装CMake-3.29.0](./zh/s3.md)

[S4.Jetson端安装RapidJson](./zh/s4.md)

[S5.Jetson端安装Pytorch-2.1.0](./zh/s5.md)

[S6.Jetson端移植LMDeploy-2.3.0](./zh/s6.md)

[S7.Jetson端离线运行InternLM大模型](./zh/s7.md)


## 引用

如果本项目对您的工作有所帮助，请使用以下格式引用：

```bibtex
@misc{hongjun2024lmdeployjetson,
    title={LMDeploy-Jetson：Opening a new era of Offline Embodied Intelligence},
    author={Hongjun An},
    url={https://github.com/BestAnHongjun/LMDeploy-Jetson},
    year={2024}
}
```

## 致谢

* [上海人工智能实验室](https://www.shlab.org.cn/)组织的[书生·浦语大模型实战营](https://github.com/InternLM/tutorial/)为我学习大模型相关理论及技术提供了宝贵的学习资料及算力资源，浦语小助手等老师也为我提供了莫大的帮助，在此一并致以真挚的谢意！

## 作者单位

**安泓郡**，西北工业大学光电与智能研究院，博士生
> Email: an.hongjun@foxmail.com \
> Page: www.anhongjun.top

<div align="center">
<img src="./attach/logo.jpg" width="500px">
</div>