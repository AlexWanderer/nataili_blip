# nataili_blip
 Nataili BLIP: A Python library for captioning images with BLIP

# Installation

`pip install nataili_blip`

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
