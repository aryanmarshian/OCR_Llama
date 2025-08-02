# 🧠 OCR to Structured Table with LLaMA Vision & Groq API

This Streamlit application extracts both **printed and handwritten text** from images using **GROQ's LLaMA 3 Vision model**, intelligently processes overlapping text regions, and consolidates the content into a clean **Markdown table**.

## 📸 Features

* 🔍 Optical Character Recognition (OCR) using LLaMA 3.2 Vision model
* 🧠 Smart image splitting into horizontal overlapping stripes for better recognition
* 🧾 Consolidation of extracted Markdown outputs using LLaMA 3.3 model
* 🖼️ User-friendly interface to upload and preview images
* 📥 Downloadable structured table as a `.txt` file


## 🛠️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/llama-ocr-table.git
cd llama-ocr-table
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Add environment variable

Create a `.env` file in the root directory and add your Groq API key:

```env
GROQ_API_KEY=your_groq_api_key_here
```

---

## 💡 Usage

Run the Streamlit app:

```bash
streamlit run app.py
```

### On the sidebar:

1. Upload a JPG or PNG image containing text (printed or handwritten).
2. The app splits the image into horizontal overlapping stripes.
3. Each stripe is passed through the LLaMA-3.2 Vision model for OCR.
4. Results are merged and formatted into a single structured table using LLaMA-3.3.

You can then download the final table.

---

## 📁 Project Structure

```
├── app.py                 # Main Streamlit app
├── .env                  # Environment variable file (ignored by Git)
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

---

## ✅ Example Use Cases

* Extracting tabular data from scanned receipts, invoices, or notes
* Converting handwritten or mixed-format documents into structured digital formats
* AI-powered digitization pipeline for educational or office documents

---

## 🧠 Powered By

* [GROQ API](https://groq.com/)
* [Meta LLaMA 3 Models](https://ai.meta.com/llama/)
* [LangChain for Groq](https://python.langchain.com/docs/integrations/llms/groq)
* [Streamlit](https://streamlit.io/) for interactive UI

---

## 📌 To-Do / Future Improvements

* Add support for PDF and multi-page documents
* Add image preprocessing (deskewing, denoising)
* Save to CSV/Excel format
* Deploy to Hugging Face Spaces or Streamlit Cloud

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

