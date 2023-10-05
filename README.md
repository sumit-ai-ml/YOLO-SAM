
This repository presents a comprehensive approach for segmenting Regions of Interest (ROI) in diverse medical imaging datasets, including ultrasound, CT scans, and X-ray images. Our method combines the YOLOv8 model for approximate boundary box detection across modalities with the Segment Anything Model (SAM) and High Quality (HQ) SAM for fully automatic and precise segmentation. 

[**Here is the Web-app:**](https://mlshots.live/YOLO-SAM/software).


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

## License

This project is licensed under the [MIT License](LICENSE.md).


