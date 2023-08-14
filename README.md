# OpenLLaMA2

<div style="font-size: 1.5rem;">
  <a href="./README.md">English</a> |
  <a href="./README_cn.md">Chinese</a>
</div>

</br>

<h1 align="center">OpenLLaMA2</h1>
<div align="center">
  <a href="[https://github.com/catqaq/ChatPiXiu ↗](https://github.com/catqaq/ChatPiXiu)">
    <img src="./docs/imgs/pixiu.png" alt="Logo" height="210">
  </a>

<p align="center">
    <h3>A Deepspeed/Ray based High-performance LLaMA2 SFT/RLHF framework!</h3>
      <a href="https://github.com/openllmai/OpenLLaMA2/graphs/contributors">
        <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/catqaq/ChatPiXiu" />
      </a>
      <a href="https://github.com/catqaq/ChatPiXiu/issues">
        <img alt="Issues" src="https://img.shields.io/github/issues/catqaq/ChatPiXiu?color=0088ff" />
      </a>
      <a href="https://github.com/openllmai/OpenLLaMA2/discussions">
        <img alt="Issues" src="https://img.shields.io/github/discussions/openllmai/OpenLLaMA2?color=0088ff" />
      </a>
      <a href="https://github.com/openllmai/OpenLLaMA2/pulls">
        <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/openllmai/OpenLLaMA2?color=0088ff" />
      <a href="https://github.com/openllmai/OpenLLaMA2/stargazers">
        <img alt="GitHub stars" src="https://img.shields.io/github/stars/openllmai/OpenLLaMA2?color=ccf" />
      </a>
      <br/>
      <em>Open-source ChatGPT / Comprehensive / Lightweight / Easy-to-use</em>
      <br/>
      <a href="https://zhuanlan.zhihu.com/p/622065348/"><strong>Articles</strong></a>
        ·
      <a href="https://zhuanlan.zhihu.com/p/622065348"><strong>Videos</strong></a>
    </p>

</p>
</div>

> **The code is open-source, feel free to use it, contributions are welcome! Note: The license of the model depends on the provider of the model.**

- [💥Latest News](#latest-news)
- [💫OpenNLP Plan](#opennlp-plan)
- [💫OpenLLaMA2](#openllama2-project)
- [⛏️Usage Steps](#Uuage-steps)
- [📄Running Example](#running-llama2-example)
- [📄Result Display](#inference)
- [🛠️Common Errors](#common-errors)
- [💐References & Acknowledgements](#references-&-acknowledgements)
- [🌟Sponsor Us](#sponsor-us)
- [🌈Starchart](#starchart)
- [🏆Contributors](#contributors)

## Latest News

- 2023/8/13: LLaMA2 7B + SFT+ RM + PPO + DeepSpeed training features finished

- 2023/07/30: OpenLLaMA2 project officially launched:
  - Initial code submission

## OpenLLaMA2 Project

OpenLLaMA2 is the third official open source project of the OpenNLP plan, and it is the first practice project of openllmai. OpenLLaMA2 aims to develop a high-performance distributed LLaMA2 SFT/RLHF training framework.

The sister project of this project is [chinese-llama2 ↗](https://github.com/OpenLLMAI/chinese-llama2), which aims to fine-tune the Chinese LLaMA2 using SFT/RLHF.

### Development Progress:

- [✔️] Develop a fast LLaMA2 SFT/PPO Training Framework based on DeepSpeed.
- [WIP] Support Multiple RM models.
- [WIP] Develop Multi-nodes RLHF based on Ray.
- [WIP] Develop the Rejection Sampling.
- [TODO] Add wandb log support.
- [TODO] Develop the DPO.
- [TODO] Develop the Context Distillation.
- [TODO] Develop the Multi-nodes training scripts for Slurm.
- [TODO] Multi-nodes Performance Optimization
- [TODO] Develop the [RLHF datasets ↗](https://github.com/OpenLLMAI/OpenLLMData) for Multiple reward models.
- [TODO] Train a [chinese-llama2 ↗](https://github.com/OpenLLMAI/chinese-llama2) RLHF model.


## Usage Steps

Clone the repository: `git clone https://github.com/openllmai/OpenLLaMA2.git`

## Running LLaMA2 Example

```python
# launch nvidia container
cd examples/scripts
./docker_run.sh

# huggingface login 
/.local/bin/huggingface-cli login

# cd in container
cd /openllama2/examples/scripts

# build OpenLLaMA2
./build_openllama2.sh

# train SFT model
./train_sft_llama.sh

# train RM model
./train_rm_llama.sh

# train PPO model
./train_ppo_llama.sh
```

## Inference

After completing the training, you can evaluate of your model by using the `inference` script:

```python
./inference_llama.sh "Please introduce GPT model."
```

### Join Us

Who are we?

We are Xianyu Intelligence \[xianyu.ai/openllmai\], members include butnot limited to: researchers, engineers, students, enthusiasts from different industries and fields. We have a common goal: to promote the development of open source NLP, and make the technology more accessible and beneficial to all.

**How to Join?**

1. Email us at janhu9527@gmail.com. Please include the following details:
   - Your name
   - Your GitHub username
   - Your areas of interest
   - Your skills and experience related to NLP and/or AI
1. You can also join us through the official GitHub [OpenLLaMA2 ↗](https://github.com/openllmai/OpenLLaMA2) project page. Just create an issue about your interest to contribute and we will get back to you.

**What can you do?**

1. Join the team and participate in the development of OpenLLaMA2 project.
1. Contribute to the project by submitting pull requests.
1. Help improve documentation, fix bugs, or create new features.
1. Share the project and help us grow the community.


## References & Acknowledgements

We would like to express our gratitude to the following projects and organizations for their contributions to the field of AI and NLP:

- [Hugging Face Transformers ↗](https://github.com/huggingface/transformers)
- [OpenAI GPT ↗](https://github.com/openai/gpt-3)
- [LLaMA2 ↗](https://ai.meta.com/llama/)
- [DeepSpeed ↗](https://github.com/microsoft/DeepSpeed)
- [Ray ↗](https://github.com/ray-project/ray)

## Sponsor Us

Your sponsorship can help us maintain and improve OpenLLaMA2. If you find this project useful, please consider sponsoring us. You can sponsor us on [Open Collective ↗](https://opencollective.com/openllmai).

## Starchart


[![Star History Chart](https://api.star-history.com/svg?repos=openllmai/OpenLLaMA2&type=Date)](https://star-history.com/#openllmai/OpenLLaMA2&Date)

## Contributors

A big thank you to all our contributors! If you want to contribute, feel free to make a pull request or create an issue.

<a href="https://github.com/openllmai/OpenLLaMA2/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=openllmai/OpenLLaMA2" />
</a>

______________________________________________________________________

*OpenLLaMA2 © 2023 OpenLLMAI. All Rights Reserved.*
