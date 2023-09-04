
# Medical Image Segmentation

This repository presents a comprehensive approach for segmenting Regions of Interest (ROI) in diverse medical imaging datasets, including ultrasound, CT scans, and X-ray images. Our method combines the YOLOv8 model for approximate boundary box detection across modalities with the Segment Anything Model (SAM) and High Quality (HQ) SAM for fully automatic and precise segmentation. 

[**Here is the Web-app:**](https://mlshots.live/YOLO-SAM/software).


## Methodology

- **YOLOv8 Training**: We trained the YOLOv8 model using a limited set of 100 images and masks from each modality to generate boundary boxes.

- **Segmentation Models**: We implemented the SAM and HQ-SAM models for precise ROI segmentation. 

## Results and Evaluation

We extensively evaluated our approach using various metrics, including precision, recall, F1 score, and Dice Score, to quantify segmentation accuracy. 

### Comparative Analysis

We conducted a comparative analysis to assess the performance of different models:

- **YOLOv8**: Our baseline model for approximate boundary box detection.
- **YOLOv8+SAM**: Combines YOLOv8 with the SAM model.
- **YOLOv8+HQ-SAM**: Combines YOLOv8 with the HQ-SAM model.

## Key Findings

- **SAM Outperforms**: The SAM model exhibited higher segmentation accuracy and overall performance compared to the other models.

- **HQ-SAM**: While HQ-SAM offers potential advantages, its incremental gains over the standard SAM model may not justify the additional computational cost.

## Conclusion

Our findings suggest that the YOLOv8+SAM model holds promise for enhancing medical image segmentation and its clinical implications.

For more details, please refer to our paper [here](link-to-paper).

## How to Use

1. Clone this repository.
2. Install the required dependencies.
3. Run the provided scripts to train and evaluate the models on your own medical image datasets.

## Citation

If you find our work helpful, please consider citing our paper:

```
@article{your-paper-citation,
  title={Comprehensive Approach for Medical Image Segmentation},
  author={Your Name and Co-Authors},
  journal={Medical Imaging Journal},
  year={Year},
  volume={Volume},
  pages={Page Numbers},
  doi={Your DOI},
}
```

## License

This project is licensed under the [MIT License](LICENSE.md).


