# How to use
![FLUX Finetuning scripts](./assets/flux-comfy-ui-nodes-dark-rev1.png)
![FLUX Finetuning scripts](./assets/image1.png)

## Installation:

1. Go to `ComfyUI/custom_nodes`
2. Clone this repo, path should be `ComfyUI/custom_nodes/x-flux-comfyui/*`, where * is all the files in this repo
3. Go to  `ComfyUI/custom_nodes/x-flux-comfyui/` and run `python setup.py`
4. Run ComfyUI after installing and enjoy!

After the first launch, the `ComfyUI/models/xlabs/loras` and `ComfyUI/models/xlabs/controlnets` folders will be created automatically. <br/>
So, to use lora or controlnet just put models in these folders. <br/>
After that, you may need to click "Refresh" in the user-friendly interface to use the models. <br/>
For controlnet you need install https://github.com/Fannovel16/comfyui_controlnet_aux <br/>
## Low memeory mode
```bash
python3 main.py --lowvram --preview-method auto --use-split-cross-attention
```
Use flux1-dev-Q4_0.gguf from this repo https://github.com/city96/ComfyUI-GGUF <br/>
Memory usage 12gb vram
## Models

We trained **Canny ControlNet**, **Depth ControlNet**, **HED ControlNet** and **LoRA** checkpoints for [`FLUX.1 [dev]`](https://github.com/black-forest-labs/flux) <br/>
You can download them on HuggingFace:

- [flux-controlnet-collections](https://huggingface.co/XLabs-AI/flux-controlnet-collections)
- [flux-controlnet-canny](https://huggingface.co/XLabs-AI/flux-controlnet-canny)
- [flux-RealismLora](https://huggingface.co/XLabs-AI/flux-RealismLora)
- [flux-lora-collections](https://huggingface.co/XLabs-AI/flux-lora-collection)
- [flux-furry-lora](https://huggingface.co/XLabs-AI/flux-furry-lora)
