# Soliton Biomedical Endoscopy CNN

![Soliton Biomedical Endoscopy CNN](https://img.shields.io/badge/Soliton%20Biomedical-Endoscopy%20CNN-blue)
![Python](https://img.shields.io/badge/Made%20with-Python-green)
![TensorFlow](https://img.shields.io/badge/Powered%20by-TensorFlow-orange)

Welcome to the Soliton Biomedical Endoscopy CNN project repository! This project focuses on developing an Endoscopic Classification Model (ECM) using Convolutional Neural Network (CNN) to predict the presence of abnormalities within endoscopic images. 

## Introduction
ECM is designed to classify endoscopic images into several classes of abnormalities, including Polyp, Hemorrhoid, and various grades of Ulcerative Colitis. The goal of ECM is to identify potential risks and enhance patient care by providing automated analysis of endoscopic images.

### Classes:
1. **Polyp**: Indicates the presence of a polyp in the endoscopic image.
2. **Hemorrhoid**: Indicates the presence of a hemorrhoid in the endoscopic image.
3. **Ulcerative Colitis Grade 0-3**: Indicates different grades of Ulcerative Colitis present in the endoscopic image.

The classes are defined based on the dataset used, and due to constraints, they have been limited to 8 classes.

## Methodology
- **Data Visualization**: Visualize training data using Plotly and Matplotlib. Histograms of pixel values are generated for each set of images based on previous labels.
- **Data Preprocessing**: Check for null values in the training dataset and preprocess images by resizing to decrease time and space complexity.
- **Model Building**: Utilize VGG-16 (CNN) to build a deep learning model on the image dataset and generate the classes.
- **Model Evaluation**: Evaluate the model using metrics such as F1-score, precision, recall, and accuracy.

### Findings:
- **Recall**: 92.14%
- **F1 Score**: 91.41%
- **Precision**: 92.51%
- **Accuracy**: 92.14%

Since the cost of false negatives is high, recall is designated as the most important evaluation measure. The model provides a recall value of 92.14%, ensuring its reliability. However, there is still room for improvement by fine-tuning the training dataset.

## Future Implications
The future implications of ECM lie in continuous fine-tuning of the model and alignment with emerging technologies. These efforts have the potential to significantly enhance diagnostic tools in gastroenterology, particularly in image classification, leading to improved patient outcomes and more efficient healthcare interventions.

## Resources
- **Training and Testing Data**: Provided by [OSF](https://osf.io/mh9sj/), an exploratory model on GI endoscopic images.
- **Other Sources**: 
  - [Springer Nature Figshare](https://springernature.figshare.com/articles/dataset/Metadata_record_for_HyperKvasir_A_comprehensive_multi-class_image_and_video_dataset_for_gastrointestinal_endoscopy/12759833?file=24463475)
  - [VGG16 Documentation](https://www.mathworks.com/help/deeplearning/ref/vgg16.html)

## Installation
To set up the environment for running this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/soliton-biomedical-endoscopy-cnn.git
   ```
2. Navigate to the project directory:
   ```bash
   cd soliton-biomedical-endoscopy-cnn
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Contributing
Contributions to this project are welcomed and appreciated. If you have any suggestions, feature requests, or bug reports, please feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
