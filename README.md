
#  Image Generator using Stable Diffusion

This project is a **Jupyter Notebook–based AI Image Generator** that leverages the **Stable Diffusion v1.5** model from Hugging Face’s `diffusers` library.  
It allows you to generate high-quality images from text prompts directly within a notebook environment using GPU acceleration.

---
 
##  Features

- Text-to-Image generation using **Stable Diffusion**
- GPU-accelerated inference with **PyTorch + CUDA**
- Simple and customizable prompts
- Easy integration with **Hugging Face Hub**
- Outputs displayed directly in the notebook

---

##  Requirements

Ensure you have **Python 3.9+** and **pip** installed.  
The notebook installs required dependencies automatically, but here’s the list:

```bash
pip install diffusers transformers accelerate torch safetensors Pillow
````

If you plan to use private models, log in to your Hugging Face account:

```python
from huggingface_hub import login
login("YOUR_HUGGINGFACE_TOKEN")
```

---

##  Model Details

* **Model ID:** `runwayml/stable-diffusion-v1-5`
* **Framework:** PyTorch
* **Pipeline:** `StableDiffusionPipeline` from `diffusers`
* **Precision:** float16
* **Device:** CUDA (GPU recommended)

---

##  How to Use

1. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/ImageGenerator.git
   cd ImageGenerator
   ```

2. Open the notebook:

   ```bash
   jupyter notebook ImageGenerator.ipynb
   ```

3. Follow the steps inside the notebook:

   * Install dependencies
   * Load the Stable Diffusion model
   * Enter a prompt (e.g., *"A futuristic cityscape at sunset, ultra-realistic"*)
   * Generate and display your image

---

##  Example

| Prompt                               | Output                              |
| ------------------------------------ | ----------------------------------- |
| *"A cyberpunk cat with neon lights"* | ![sample](assets/sample_output.png) |

*(You can replace this with your own sample output)*

---

##  Tips

* Use more descriptive prompts for detailed results.
* If you run out of GPU memory, switch to a smaller model (e.g., `stabilityai/sd-turbo`).
* Save generated images with:

  ```python
  image.save("output.png")
  ```




Would you like me to include a **“Results” section** (with code snippets showing how prompts map to images) or keep it concise for GitHub?
```
