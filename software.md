<iframe src="https://sumit-ai-ml-sam-with-yolo.hf.space" frameborder="0" width="850" height="800" ></iframe>


- **Input:**
This software has been meticulously engineered to seamlessly process 2D point-of-care ultrasound (POCUS) images, which are formatted as `.png` or `.jpg` files. These images exhibit dimensions of (x, y, 3), allowing for variations in size, and are fundamental to the core functionality of the software.


## Methodology

- **YOLOv8 Training**: We trained the YOLOv8 model using a limited set of 100 images and masks from each modality to generate boundary boxes.

- **Segmentation Models**: We implemented the SAM and HQ-SAM models for precise ROI segmentation. 

## Results and Evaluation

We extensively evaluated our approach using various metrics, including precision, recall, F1 score, and Dice Score, to quantify segmentation accuracy. 


## Key Findings

- **SAM Outperforms**: The SAM model exhibited higher segmentation accuracy and overall performance compared to the other models.

- **HQ-SAM**: While HQ-SAM offers potential advantages, its incremental gains over the standard SAM model may not justify the additional computational cost.

## Conclusion

Our findings suggest that the YOLOv8+SAM model holds promise for enhancing medical image segmentation and its clinical implications.

For more details, please refer to our paper [here](https://openaccess.thecvf.com/content/ICCV2023W/CVAMD/papers/Pandey_Comprehensive_Multimodal_Segmentation_in_Medical_Imaging_Combining_YOLOv8_with_SAM_ICCVW_2023_paper.pdf).

## How to Use

1. Clone this repository.
2. Install the required dependencies.
3. Run the provided scripts to train and evaluate the models on your own medical image datasets.

## Citation

If you find our work helpful, please consider citing our paper:

```
@InProceedings{Pandey_2023_ICCV,
    author    = {Pandey, Sumit and Chen, Kuan-Fu and Dam, Erik B.},
    title     = {Comprehensive Multimodal Segmentation in Medical Imaging: Combining YOLOv8 with SAM and HQ-SAM Models},
    booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) Workshops},
    month     = {October},
    year      = {2023},
    pages     = {2592-2598}
}
```



- **Hosting:**
The web application is hosted using the Hugging Face Spaces platform, providing a convenient and accessible environment for users to interact with the software's features and capabilities.

- **Privacy Assurance:**
We want to assure our users that this software respects your data privacy. We do not gather or retain any image data from interactions with this web software. Additionally, based on our current knowledge, the Hugging Face Spaces platform also upholds stringent privacy practices and does not collect image data. For a more comprehensive understanding of our privacy policies and those of Hugging Face, please refer to the following link: [Privacy Information](https://huggingface.co/docs/inference-endpoints/security). 

Please feel at liberty to delve into the depths of our software. Should any queries arise or if you find yourself yearning for a hearty discussion, fear not – for this is the realm where such conversations flourish. Your inquiries and insights are both valued and encouraged.

Don't hesitate to initiate a dialogue by visiting our dedicated space here: [Aorta-POCUS-Segmentation Discussions](https://github.com/sumit-ai-ml/Aorta-POCUS-Segmentation/discussions/1).

Your participation enriches our community, and we eagerly anticipate the conversations that will unfold.

