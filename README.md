# Depression-Detection-using-EEG-Sensors

Depression and anxiety impact millions worldwide. Traditional diagnostic methods often fail to detect these conditions effectively. EEG sensors offer a promising solution by providing insights into cognitive and emotional states through brain wave patterns. This project leverages deep learning to automate depression detection using EEG data.

## Dataset and Experiment
The MODMA Dataset was used, involving experiments with 128 electrodes over 160 trials on participants. Each trial involved displaying stimuli and recording participant responses to assess cognitive reactions via EEG.

### Data Details
- **Total Subjects**: 53
- **Major Depressive Disorder Subjects**: 24
- **Healthy Control Subjects**: 29
- Data access is restricted and requires authorization via a signed license agreement.

### Data Preprocessing
- Raw EEG data was converted to CSV format for processing.
- Data was segmented into batches of 2000 data points per row to maintain the integrity of time series data.

## Solution Ideology
Two primary approaches were tested:
1. **2D Image Approach**: Treating data as 2D images and using 2D Convolutional Neural Networks (CNN).
2. **1D Time Series Approach**: Treating data as 1D time series signals and using 1D CNN models.

## Baseline Models
- ResNet and VGG models were adapted to 1D and 2D formats to accommodate EEG data characteristics.
- Additional models like EEGNet and EEGConformer were also evaluated.

## Challenges
- Limited data availability and difficulty in data extraction and preprocessing.
- Overfitting due to limited data, addressed through data augmentation and model experimentation.

## Results
- The best-performing approach was the Image Generation + ResNet50 model, which achieved the highest validation accuracy.

## Future Work
- Explore additional data augmentation techniques and incorporate multimodal data for comprehensive analysis.
- Consider using transfer learning from larger EEG datasets or related tasks to improve model performance.

