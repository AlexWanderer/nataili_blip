# nataili_blip
 Nataili BLIP: A Python library for captioning images with BLIP

# Installation

`pip install nataili_blip`

# Code Usage

Minimal example

```
from nataili_blip.model_manager import BlipModelManager
from nataili_blip.caption import Caption

image_path = "test.png"
image = PIL.Image.open(image_path).convert("RGB")

model_name = "BLIP"
mm = BlipModelManager()
mm.download_model(model_name)
mm.load_blip(model_name)
blip = Caption(mm.loaded_models[model_name]["model"], mm.loaded_models[model_name]["device"])

caption = blip(image)

print(caption)
```

# CLI Usage

```
nataili_blip --help
Usage: nataili_blip [OPTIONS] IMAGE_PATH

Options:
  --model_name [BLIP|BLIP_Large]  [default: BLIP]
  --precision [half|full]         [default: half]
  --gpu_id INTEGER                [default: 0]
  --blip_image_eval_size INTEGER  [default: 512]
  --sample                        [default: True]
  --num_beams INTEGER             [default: 3]
  --max_length INTEGER            [default: 30]
  --min_length INTEGER            [default: 10]
  --top_p FLOAT                   [default: 0.9]
  --repetition_penalty FLOAT      [default: 1.0]
  --help                          Show this message and exit.
  ```
  
# UI
`nataili_blip_ui`

<img width="960" alt="image" src="https://user-images.githubusercontent.com/106811348/208988851-b193b97e-87f6-4a2f-9948-af40edd620e2.png">
