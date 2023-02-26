# Product-Personalization

This project aim to programatically paste persons' faces into given background images

## How to run
1. Run the Jupyter notebook using google colab
2. Setup following config variables `capture_image_from_webcam`, `gdrive_products_path`

`capture_image_from_webcam` - configure from where we fetch the person's face image <br/>
`gdrive_products_path` - upload location of background images

sample backgorund(product) image folder file structure
* image_generation_config.json
* background_image_1.png
* background_image_2.jpg


### sample `image_generation_config.json` structure
```
[
    {
        "imageName": "General_wallclock.png",
        "personImage": {
            "offset": {
                "x_offset": 217,
                "y_offset": 169
            },
            "size": {
                "max_width": 54,
                "max_height": 46
            }
        }
    },
    {
        "imageName": "Generic_milkpowder.png",
        "personImage": {
            "center": {
                "x": 199,
                "y": 208
            },
            "size": {
                "max_width": 99,
                "max_height": 110
            }
        }
    }
]
```
