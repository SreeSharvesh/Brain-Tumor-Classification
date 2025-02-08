# Brain Tumor Classification Application

This project provides a web-based application for classifying brain tumors from MRI scans using deep learning models. The application uses pre-trained models - Xception and a custom CNN model for the classification task. It also generates saliency maps to highlight the regions of the MRI scan that the model focuses on during prediction.

[Visit my app!](https://sharvesh-brain-tumor-classification.streamlit.app/)

## Features

- **Brain Tumor Classification**: Classifies MRI scans into four categories:
  - Glioma
  - Meningioma
  - Pituitary tumor
  - No tumor
- **Saliency Maps**: Highlights the regions of the MRI scan that the model focuses on during classification.
- **Model Explanation**: Provides explanations based on the saliency map, giving insight into the areas of the brain contributing to the classification.
- **Mock Case Generation**: Generates realistic mock history cases based on the AI predictions.
- **PDF Report Generation**: Generates a downloadable report with classification results, saliency map, and general recommendations.

## Technologies Used

- **Deep Learning Framework**: TensorFlow/Keras
- **Models**: Xception, Custom CNN
- **Web Framework**: Streamlit
- **Saliency Maps**: Grad-CAM-based saliency visualization
- **PDF Generation**: FPDF
- **Image Processing**: OpenCV, PIL
- **AI Services**: Google Gemini, Pixtral (for explanation generation)

## Models
- **Xception**: A deep convolutional neural network trained on the ImageNet dataset, fine-tuned for brain tumor classification.
- **Custom CNN**: A custom-designed convolutional neural network for brain tumor classification.


## Usage
1. **Upload an MRI Scan**: Select an MRI image of the brain from your local filesystem. Supported formats: JPG, PNG, JPEG.
2. **Choose a Model**: Select the deep learning model you wish to use for classification:
- Xception
- Custom CNN
3. **View Results**: The app will display the predicted class (glioma, meningioma, pituitary, or no tumor) along with a confidence score.
4. **Saliency Map**: A saliency map highlighting the regions of the MRI scan that contributed most to the classification decision is generated.
5. **Generate Report**: Download a PDF report containing the following:
    - Classification result and confidence
    - Saliency map
    - General recommendations
    - A simulated history of similar cases
