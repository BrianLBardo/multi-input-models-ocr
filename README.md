# **Multimodal-OCR3**

Optical Character Recognition (OCR) unlocks numerous possibilities in data management.

By leveraging multi-modal modeling, paired with robust training and optimization, you'll deploy deep learning techniques to classify insurance codes from scanned insurance documents and develop an advanced OCR model.

## **Key Features**

* **Multi-Model Architecture:** Seamlessly switch between specialized models directly from the interface. Supported models include `Nanonets-OCR2-3B`, `Chandra-OCR`, `Dots.OCR`, and `olmOCR-2-7B-1025`.
* **Custom User Interface:** Features a bespoke, responsive Gradio frontend built with custom HTML, CSS, and JavaScript. It includes a drag-and-drop media zone, real-time output streaming, and an integrated advanced settings panel.
* **Granular Inference Controls:** Fine-tune the AI's output by adjusting text generation parameters such as Maximum New Tokens, Temperature, Top-p, Top-k, and Repetition Penalty.
* **Output Management:** Built-in actions allow users to instantly copy the raw output text to their clipboard or save the generated response directly as a `.txt` file.
* **Flash Attention 2 Integration:** Utilizes `kernels-community/flash-attn2` for optimized, memory-efficient inference on compatible GPUs.

### **Installation and Requirements**

To run multi-input-models-ocr locally, you need to configure a Python environment with the following dependencies. Ensure you have a compatible CUDA-enabled GPU for optimal performance.

**1. Install Core Requirements**
Install the necessary machine learning and UI libraries by running `pip install -r requirements.txt`.

### **Usage**

Once your environment is set up and the dependencies are installed, you can launch the application by running the main Python script:

```bash
python app.py
```

After the script initializes the interface, it will provide a local web address (usually `http://127.0.0.1:7860/`) which you can open in your browser to interact with the models. Note that the selected models will be downloaded and loaded into VRAM upon their first invocation.
