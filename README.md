##ImagineAI – Resource-Efficient Text-to-Image Generation

ImagineAI is an AI-powered image generation and enhancement web application. It converts text prompts into images using Stable Diffusion Turbo and provides image enhancement using OpenCV.

## Project Overview

The project focuses on resource-efficient image generation by adjusting inference steps and image resolution while comparing generation speed and image quality.

## Features

- Generate images from text prompts.
- Select inference steps: 1, 2 and 4.
- Select image resolutions: 256×256, 384×384 and 512×512.
- View and download generated images.
- Upload images for enhancement.
- Choose 2× or 4× image upscaling.
- Apply denoising, contrast enhancement and sharpening.
- Evaluate text-image similarity using CLIP.

## Technologies Used

- Python
- PyTorch
- Hugging Face Diffusers
- Stable Diffusion Turbo
- OpenCV
- CLIP
- Flask
- HTML
- CSS
- JavaScript
- Google Colab
- GPU / CUDA

## System Architecture

User Input → Web Interface → Flask Backend → Stable Diffusion Turbo / OpenCV → Image Output.

## Main Modules

### 1. Text-to-Image Generation

Users enter a text prompt and select the inference steps and image resolution. Stable Diffusion Turbo generates the image, which can be viewed and downloaded.

### 2. Image Enhancement

Users upload an image and select 2× or 4× upscaling. OpenCV applies resizing, bilateral filtering, CLAHE-based contrast enhancement and sharpening.

### 3. Image Evaluation

CLIP is used to calculate text-image similarity between the input prompt and generated image.

## Execution Environment

The application is developed and executed using Google Colab with GPU acceleration.

### Steps to Run

1. Open the project notebook in Google Colab.
2. Connect the runtime and enable GPU acceleration.
3. Install the required Python libraries.
4. Load the pretrained Stable Diffusion Turbo model.
5. Execute the Flask application.
6. Start the server on port 5002.
7. Generate the website access link using:

```python
from google.colab import output

website_url = output.eval_js(
    "google.colab.kernel.proxyPort(5002)"
)

print(website_url)
```

8. Open the generated link in a web browser.

## Performance Evaluation

The project evaluates:

- Image generation time.
- Inference steps.
- Image resolution.
- GPU memory usage.
- Visual image quality.
- Text-image similarity using CLIP.

Actual experimental measurements should be reported in the project report.

## Limitations

- The application currently runs through Google Colab.
- The runtime must remain active while using the application.
- Generation speed depends on available GPU resources.
- Lower inference steps may affect image quality.
- OpenCV enhancement cannot guarantee recovery of missing image details.
- Permanent public deployment and direct mobile-device execution have not been implemented.

## Future Enhancements

- Optimize the model for mobile devices.
- Explore model quantization and memory optimization.
- Improve image quality and generation speed.
- Deploy the application as a permanent web service.
- Add more image enhancement techniques.

## GitHub Repository

https://github.com/priyabaisbtechl24-art/imagine-ai-project

## Acknowledgements

PyTorch, Hugging Face, Stable Diffusion Turbo, OpenCV, CLIP, Flask and Google Colab.

**ImagineAI – Turning Text into Images with Efficient AI Generation.**
