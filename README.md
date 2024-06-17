---
title: HF_SPACE DEMO
emoji: 🐹
colorFrom: blue
colorTo: pink
sdk: gradio
sdk_version: 4.36.1
app_file: app.py
base_model: stabilityai/sdxl-turbo
model: SG161222/RealVisXL_V4.0
type: base_model, model
pinned: true
header: mini
theme: bethecloud/storj_theme
get_hamster_from: https://prithivhamster.vercel.app/
license: creativeml-openrail-m
short_description: Fast as Hamster | Stable Hamster | Stable Diffusion
---

## How to run hf spaces on local cpu (ex.intel i5 / amd ryzen 7) or by google colab with T4 gpu ❓

![alt text](assets/cpugpu.gif)

# Before getting into the demo, let's first understand how Hugging Face access tokens are passed from the settings on your profile ⭐

    You can see the hf token there : 👇🏻  in your profile
    
    https://huggingface.co/settings/tokens

![alt text](assets/at.png)

    Pass the access to Login locally to Hugging face

![alt text](assets/accesstokengpu.png)

## 1. Running in T4 GPU, Google Colab Space : Hardware accelerator

    Choose the run-as-gpu.ipynb file from the repo & take it on to the colab notebooks

![alt text](choose/6.png)

    In Colab Choose the T4 GPU as a Runtime Hardware ✅ as Google Compute Engine !!
    
![alt text](assets-gpu/gpu0.png)

    Run the modules one by one : first the requirements, sencond the hf_access_token -- Login successful!, third the main code block. After the components of the model which you have linked with the model id will be loaded.
    
![alt text](assets-gpu/gpu4.png)

    👇🏻👇🏻After Successfully running the code the live.server for gradio will give a link like this ...

    https://7770379da2bab84efe.gradio.live/
    
🚀Progress

    After loading to the gradio.live, the gradio interface like this.. & enter the prompt and process it


| ![alt text](assets-gpu/gpu3.png) |![alt text](assets-gpu/gpu1.png) |
|---------------------------|--------------------------|


    The Sample results 1 & 2 from the colab space

| ![alt text](assets-gpu/gpu5.png) |![alt text](assets-gpu/gpu6.png) |
|---------------------------|--------------------------|

    The original resultant image from the space // gradio.live 

| ![alt text](assets/image1.png) |![alt text](assets/image2.png) |
|---------------------------|--------------------------|

🚀Working Link for the Colab :

    https://colab.research.google.com/drive/1rpL-UPkVpJgj5U2WXOupV0GWbBGqJ5-p

.

.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------


## 2. Running in CPU, Local System : Hardware accelerator

    Choose the run-as-cpu.py file from the repo & take it on to the local code editor ( eg. vs.code )
    Statisfy all the requirement.txt ; pip install -r requirements.txt

![alt text](choose/7.png)

Run all the requirements

    accelerate
    diffusers
    invisible_watermark
    torch
    transformers
    xformers

🚀Run the run-as-cpu.py by ( python run-as-cpu.py )

![alt text](assets-cpu/cpu.png)

http://127.0.0.1:7861
