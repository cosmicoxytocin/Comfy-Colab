## Manually Install SD3 (Google Drive) 📁

### Steps
1. Download SD3 weights from the offical 🤗[repo](https://huggingface.co/stabilityai/stable-diffusion-3-medium)
    - See [Model Versions](#model-versions)
2. Upload/Drag-and-drop `.safetensors` to `checkpoints` directory. (see path below)


**Path:** (default)
```
.
└── MyDrive/
    └── Comfy/
        └── ComfyUI/
            └── models/
                └── checkpoints/
                    └── <safetensors go here>
```

### Model Versions
| Model Name                                  | Size (gb) | Precision     | Included Encoders                | Additional Components                                                                                                                            |
|---------------------------------------------|-----------|---------------|----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| sd3_medium_incl_clips_t5xxlfp16.safetensors | 15.8 GB   | float16       | CLIP-G/14<br>CLIP-L/14<br>T5-XXL | None                                                                                                                                             | 
| sd3_medium_incl_clips_t5xxlfp8.safetensors  | 10.9 GB   | float8_e4m3fn | CLIP-G/14<br>CLIP-L/14<br>T5-XXL | None                                                                                                                                             |
| sd3_medium.safetensors                      | 4.34 GB   | N/A           | None                             | clip_g.safetensors<br>clip_l.safetensors<br>t5xxl_fp16.safetensors (Optional: 9.79 GB)<br>OR<br>t5xxl_fp8_e4m3fn.safetensors (Optional: 4.89 GB) |

If you choose `sd3_medium.safetensors` you **must** download at minimum both CLIP models. For improved quality, at the cost of performance you can also include **one** of the T5 autoencoder variants.<br>
Autoencoders can be found in the offical 🤗[repo](https://huggingface.co/stabilityai/stable-diffusion-3-medium/tree/main/text_encoders)
Downloaded encoders are uploaded to the same location in [Steps](#steps) (`Comfy//ComfyUI//models//checkpoints//`)


  
