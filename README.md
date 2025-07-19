# 🏥 Hebrew Medical RAG Assistant

**An end-to-end Hebrew-speaking Retrieval-Augmented Generation (RAG) chatbot for answering medical questions.**  
This project leverages FAISS, sentence embeddings, and a multilingual language model (`google/medgemma-4b-it`) to deliver helpful, context-aware medical answers in Hebrew.

---

## 📌 Features

- 💬 Chatbot interface with Gradio  
- 🧠 Retrieval-Augmented Generation (RAG) pipeline  
- 🗣️ Multilingual embeddings (`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`)  
- 🤖 Quantized LLM (`google/medgemma-4b-it`) for efficient Hebrew response generation  
- 🔍 Vector search with FAISS for semantic similarity  
- 📊 Uses real-world Hebrew Q&A data from Clalit Health Services  
- ⚙️ Robust fallback to CPU and memory management for limited environments  

---

## 🚀 Tech Stack

| Component              | Library/Model                                                                 |
|------------------------|-------------------------------------------------------------------------------|
| Interface              | [`Gradio`](https://www.gradio.app/)                                          |
| Embeddings             | [`SentenceTransformers`](https://www.sbert.net/) (`paraphrase-multilingual`) |
| Vector Search          | [`FAISS`](https://github.com/facebookresearch/faiss)                         |
| LLM                    | [`google/medgemma-4b-it`](https://huggingface.co/google/medgemma-4b-it)      |
| Language Modeling API  | [`Transformers`](https://huggingface.co/docs/transformers/index)             |
| Quantization           | [`BitsAndBytes`](https://huggingface.co/docs/transformers/main_classes/quantization) |
| Auth & Model Hosting   | [`Hugging Face Hub`](https://huggingface.co/)                                |
| Data Source            | Clalit Q&A dataset (CSV from GitHub)                                          |

---


## 🚀 How to Use (Colab)

> **No local installation needed!** You can run the entire system in Google Colab.

### ✅ Step-by-Step Instructions:

1. **Open the Notebook**  
   👉 [Click here to open the Colab notebook]([https://colab.research.google.com/drive/1JUSGMXLbGa4JrrBiRBX_m6c49y_JyC-8?usp=sharing])  


2. **Switch to GPU Runtime**  

3. **Run All Cells**  
Click `Runtime > Run all` or execute cells one by one.

4. **Enter Hugging Face Token When Prompted**  
See the instructions below for how to get your token.

5. **Chat With the Bot**  
A Gradio interface will launch with a public link. You can now ask medical questions in Hebrew.

---

## 🔐 Hugging Face Access Setup

1. **Create a Hugging Face account** (if you don’t already have one):  
👉 https://huggingface.co/join

2. **Accept the Model Terms**:  
👉 https://huggingface.co/google/medgemma-4b-it  
Click **“Access repository”** and accept the terms and conditions.

3. **Generate a Read Token**:  
- Go to: https://huggingface.co/settings/tokens  
- Click **New token**, select **Read** access, and copy the token.

4. **Paste Token in Colab When Prompted**  
The notebook will ask you to enter your token in a cell:

---
<img width="1935" height="663" alt="image" src="https://github.com/user-attachments/assets/d6238291-7046-49e9-8e50-387f62b9326a" />

---
<img width="1918" height="689" alt="image" src="https://github.com/user-attachments/assets/c6cf0454-a9fa-43f9-b2f5-f3c59333ee72" />


