Demo: 👉 [Hugging Face Spaces üzerinde deneyin](https://huggingface.co/spaces/dogukang/Food_101)

🍽️ Food101 - Image Classification with EfficientNet-B2
This project classifies food images from the Food101 dataset using a pretrained EfficientNet-B2 model.

## 📦 Teknolojiler
- 🔍 Model: EfficientNet-B2 (`torchvision`)
- 📚 Dataset: Food101 (101 sınıf)
- 🧠 Training: PyTorch, torchvision
- 🖼️ UI: Gradio
- 📁 Weights: Stored in `.pth`, auto-loaded on inference

## 🚀 Eğitim Özeti
- Epochs: 5
- Loss Function: `nn.CrossEntropyLoss(label_smoothing=0.1)`
- Optimizer: `Adam`

📌 Notes:
The model was loaded using torchvision.models.efficientnet_b2(weights=...).
The classifier head was replaced to fit 101 classes.

The image below shows the model successfully predicting the correct food classes:
![Sample Prediction](outputs/sample_prediction.png)
