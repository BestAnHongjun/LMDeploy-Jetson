# Test Benchmark of LMDeploy-Jetson

Please first refer to S2-S7 for deploying LMDeploy in Jetson.

Activate your conda environment.

```sh
conda activate lmdeploy
```

Enter the `lmdeploy/benchmark` directory.

```sh
cd ~/lmdeploy/benchmark
```

Run Benchmark.

```sh
python profile_generation.py \
    <path/to/your/model>/internlm2-chat-1_8b-turbomind \
    --concurrency 1 \
    --prompt-tokens 128 \
    --completion-tokens 128
```

Replace `internlm2 chat-1_8b turbomind` with your model path.

Record the speed benchmark.

![](../attach/benchmark.png)

During the inference process, the unified memory usage can be viewed through the `htop` command.

```sh
# Install htop (if already installed, please ignore)
apt-get install htop

# Run htop to check the usage of Mem.
htop
```

