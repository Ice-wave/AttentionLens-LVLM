# AttentionLens-LVLM

A lightweight and extensible toolkit **AttentionLens-LVLM** for visualizing attention flow in Large Vision-Language Models (LVLMs). It renders token-to-token attention maps, cross-modal attention paths, and layer–head attention dynamics, helping researchers diagnose abnormal attention behaviors. The currently supported LVLMs include *LLaVA-1.5-7B*.

![Logo](asset/Logo.png)

## Features

- **Attention Flow Visualization**: We support visualizing average attention maps, attention maps for output tokens, and attention maps for specified layers and heads. ***Attention sink*** ablation is also supported.

- **Token Evolution Analysis**: We visualize the semantic evolution of tokens—such as visual tokens—across layers, analyze the attention contributions to output tokens, and provide comparisons with the original image.

- **Multi-Model Support**: Currently supports the *LLaVA-1.5-7B* model, with more models to be added in the future.

- **Local Model Support**: Supports loading models locally to reduce network dependency.

## Quick Start

1. Clone this repository:
   ```bash
   git clone https://github.com/Ice-wave/AttentionLens-VLM.git
   cd AttentionLens-VLM
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. For usage examples, please refer to `AttentionLens-LVLM/llava1.5/llava_vis.ipynb`.

## Visualization at a Glance

***Layer-wise Attention Maps:***

<p float="left">
  <img src="asset/Layer-wise%20Attention%20Maps.png" width="100%" />
</p>


***Average Attention Map:***

<p float="left">
    <img src="asset/Attention%20Map.png" width="40%" />
</p>

***Output and Specific Attention Map:***

<p float="left">
    <img src="asset/Output%20Attention%20Map.png" width="43%" />
    <img src="asset/Specific%20Attention%20Map.png" width="52%" />
</p>

***Semantic Evolution Visualization:***

<p float="left">
    <img src="asset/Semantic%20Evolution%20Visualization.png" width="95%" />
</p>



## Supported Models

Currently supported models include:

- **LLaVA-1.5-7B**

More models coming soon™. If you can’t wait, feel free to drop in and contribute—we won’t stop you.

## Contributing

Contributions are welcome! Go ahead—fork with confidence and send us a pull request. We’ll take a look, nod thoughtfully, and (probably) merge it once it passes review.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

Thanks to the following projects for inspiration and support:

- [Hugging Face Transformers](https://github.com/huggingface/transformers)
- [Logit Lens](https://www.lesswrong.com/posts/AcKRB8wDpdaN6v6ru/interpreting-gpt-the-logit-lens)
- [LogitLens4LLMs](https://github.com/zhenyu-02/LogitLens4LLMs)
- [VLM-Visualizer](https://github.com/zjysteven/VLM-Visualizer)

***Code with joy!***
