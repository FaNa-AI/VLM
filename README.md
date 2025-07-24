
# 🖼️ Image Captioning with BLIP (Vision-Language Model)

This project demonstrates how to generate captions for images using the **BLIP (Bootstrapped Language-Image Pretraining)** model by Salesforce, powered by the 🤗 Hugging Face Transformers library.

It is designed to run in **Google Colab** and uses a dataset of images (such as a subset of Flickr8k) to generate natural language captions.

---

## 📌 Features

- ✅ Uses `Salesforce/blip-image-captioning-base` for image captioning
- ✅ Automatically loads and processes images from a ZIP file
- ✅ GPU-accelerated via Google Colab
- ✅ Shows sample outputs using `matplotlib`
- ✅ Clean and modular Python code

---

## 📁 Dataset

The dataset used is a 2,000-image subset of the Flickr8k dataset.

📥 **Download here**:  
[https://www.kaggle.com/datasets/sanjeetbeniwal/flicker8k-2k](https://www.kaggle.com/datasets/sanjeetbeniwal/flicker8k-2k)

**Expected structure inside the ZIP file**:

```

Flickr8k\_2k.zip
└── Flicker8k\_2kDataset/
├── image1.jpg
├── image2.jpg
└── ...

````

Make sure to upload this ZIP file to your Colab environment before running the notebook.

---

## 🛠️ Dependencies

The following Python packages are required:

```bash
pip install torch torchvision torchaudio
pip install transformers
pip install matplotlib
````

All of these are automatically installed in the Colab notebook.

---

## 🚀 How It Works

1. **Setup**: Required libraries are installed and runtime is set to GPU.
2. **Dataset Unzipping**: The image dataset is unzipped in Colab.
3. **Model Loading**: BLIP processor and model are loaded to GPU.
4. **Captioning**: Random images are selected and captioned.
5. **Visualization**: Each image is displayed with its generated caption.

---

## 📸 Sample Output

```
Image: a child.jpg
Generated Caption: a child sitting in a play area

```

---

## 💡 Model Info

* Model: `Salesforce/blip-image-captioning-base`
* Library: [Hugging Face Transformers](https://huggingface.co/docs/transformers/index)
* Pretrained for general image-to-text tasks.

---

## ▶️ Usage Instructions

1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. Upload your dataset ZIP file to Colab (`Flickr8k_2k.zip`).
3. Set runtime to **GPU**:

   * `Runtime` → `Change runtime type` → `GPU`
4. Run all cells from top to bottom.
5. View the images and their generated captions.

---

## 📄 License

This project is for educational purposes and uses publicly available pretrained models under their respective licenses.


