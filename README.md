# 🐠 Underwater AI Pet Projects

A collection of my experimental projects around underwater scene generation, fish species generation models, and auxiliary (dataset, work with images) tools.  
Each project explores a separate stage of the pipeline — from image generation and model deployment to dataset preparation and notebook-based experimentation.

---

## ⚙️ Tech Used
- **Stable Diffusion 1.5** with **LoRA fine-tuning**, **ControlNet**, **pix2pix**, **cycleGAN** with perceptual loss
- **Diffusers**, **Accelerate**, **Transformers**
- **Replicate.com** deployment via **Cog + Docker**
- **Roboflow** for dataset labeling, augmentation, and export
- **YOLOv8** for fish species detection and dataset generation from real aquarium footage
- **Gradio** for web UIs development, **https://huggingface.co/** for UI deployment
- **Python scripts** for dataset automation
- **Colab / Jupyter** notebooks for experimentation

---

## 1️⃣ [underwater-style-transfer](https://github.com/taras-musakovskyi/underwater-style-transfer)
Deployment configuration for the `underwater-style-transfer` model on Replicate.  
Contains `Cog` and `Docker` setup for running fine-tuned `pix2pix` and `cycleGAN with perceptual loss` models. 
Includes two-option `Gradio UI` for room underwater style transfer to user image, with support for pix2pix and cycleGAN.

---

## 2️⃣ [deploy_fish-lora-sd15](https://github.com/taras-musakovskyi/deploy_fish-lora-sd15)
Deployment configuration for the `fish-lora-sd15` model on Replicate.  
Contains `Cog` and `Docker` setup for running fine-tuned `Stable Diffusion LoRA` models as reproducible endpoints.
The model itself is used for the particular looking fish species generation. `Gradio UI` is available to invoke those.

---

## 3️⃣ [deploy_fish_inpaint_replicate](https://github.com/taras-musakovskyi/deploy_fish_inpaint_replicate)
Replicate deployment `fish_inpaint_replicate` for the inpainting + generic room generation model that generates a generic underwater room adds fish to underwater environments.  
Implements a `LoRA-based SD` pipeline with `mask-based inpainting` logic and HF/Replicate integration. `Gradio` UI is available to draw or generate corresponding mask and preview inpainting results.

---

## 4️⃣ [fish-images-scripts](https://github.com/taras-musakovskyi/fish-images-scripts)
`Python` utilities for dataset preparation, cropping, augmentation, and verification.  
Includes scripts for generating `dry/wet` paired datasets, splitting images, verifying dataset integrity, work with images etc.

---

## 5️⃣ [colab-jupyter-fish-models](https://github.com/taras-musakovskyi/colab-jupyter-fish-models)
`Google Colab` and `Jupyter-based` notebooks used for model training and evaluation.  
Covers dataset preparation, LoRA, pix2pix, cycleGAN fine-tuning,  and (failed) experiments with underwater style transfer in latent space insead of full image as well as with ControlNET.

---

## 🧠 About These Projects
These pet projects explore the intersection of **computer vision** and **generative modeling** —  
building practical workflows for fine-tuning, inpainting, and dataset management in underwater and fish-related visual domains.

Each repository is self-contained and deployable, yet forms part of a cohesive research playground.

---

> Created and maintained by [@taras-musakovskyi](https://github.com/taras-musakovskyi)
