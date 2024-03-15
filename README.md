# LMDeploy-Jetson Community

***Deploying LLMs offline on the NVIDIA Jetson platform marks the dawn of a new era in embodied intelligence, where devices can function independently without continuous internet access.***

[[中文]](./README_zh.md) | [[English]](./README.md)

This project focuses on adapting [LMDeploy](https://github.com/InternLM/lmdeploy) for use with NVIDIA Jetson series edge computing cards, facilitating the implementation of [InternLM](https://github.com/InternLM/InternLM) series LLMs for **Offline Embodied Intelligence (OEI)**.

## Latest News🎉

* [2024/3/15] Updated suppoort for [LMDeploy-v0.2.5](https://github.com/InternLM/lmdeploy/releases/tag/v0.2.5).
* [2024/2/26] This project has been included in the [LMDeploy](https://github.com/InternLM/lmdeploy) community.

## Community Recruitment

* Recruiting community managers (Contact: an.hongjun@foxmail.com)
* Recruiting benchmark testing data for more models of Jetson boards (please PR directly), such as:
    * Jetson Nano
    * Jetson TX2
    * Jetson AGX Xavier
    * Jetson Orin Nano
    * Jetson AGX Orin
* Recruiting developers to create Jetson-specific whl distributions
* README optimization, etc.

## Verified model/platform

* ✅：Verified and runnable
* ❌：Verified but not runnable
* ⭕️：Pending verification

|Models|InternLM-7B|InternLM-20B|InternLM2-1.8B|InternLM2-7B|InternLM2-20B|
|:-:|:-:|:-:|:-:|:-:|:-:|
|Orin NX(16G)<br>Jetpack 5.1|✅<br>Mem:8.6G/16G<br>*7.39 token/s*|✅<br>Mem:14.7G/16G<br>*3.08 token/s*|✅<br>Mem:5.6G/16G<br>*22.96 token/s*|✅<br>Mem:9.2G/16G<br>*7.48 token/s*|✅<br>Mem:14.8G/16G<br>*3.19 token/s*|
|Xavier NX(8G)<br>Jetpack 5.1|❌|❌|✅<br>Mem:4.35G/8G<br>*28.36 token/s*|❌|❌|


**If you have more Jetson series boards, feel free to run benchmarks and submit the results via `Pull Requests` (PR) to become one of the community contributors!**


## Future Work

* Updating benchmark testing data for more models of Jetson boards.
* Creating Jetson-specific whl distributions.
* Following up on updates to the LMDeploy version.

## Tutorial

[S1.Quantize on server by W4A16](./en/s1.md)

[S2.Install Miniconda on Jetson](./en/s2.md)

[S3.Install CMake-3.29.0 on Jetson](./en/s3.md)

[S4.Install RapidJson on Jetson](./en/s4.md)

[S5.Install Pytorch-2.1.0 on Jetson](./en/s5.md)

[S6.Port LMDeploy-0.2.5 to Jetson](./en/s6.md)

[S7.Run InternLM offline on Jetson](./en/s7.md)

## Appendix

* [Reinstall Jetpack for Jetson](https://www.anhongjun.top/blogs.php?id=1)
* [Test Benchmark of LMDeploy-Jetson](./en/benchmark.md)

## Community Projects

* InternDog: Offline embodied intelligent guide dog based on the InternLM2. [[Github]](https://github.com/BestAnHongjun/InternDog) [[Bilibili]](https://www.bilibili.com/video/BV1RK421s7dm)

## Citation

If this project is helpful to your work, please cite it using the following format:

```bibtex
@misc{2024lmdeployjetson,
    title={LMDeploy-Jetson：Opening a new era of Offline Embodied Intelligence},
    author={LMDeploy-Jetson Community},
    url={https://github.com/BestAnHongjun/LMDeploy-Jetson},
    year={2024}
}
```

## Acknowledgements

* [InternLM Practical Camp](https://github.com/InternLM/tutorial/)
* [Shanghai Artificial Intelligence Laboratory](https://www.shlab.org.cn/)
