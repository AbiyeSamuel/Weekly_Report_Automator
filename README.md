# 📄 AI-Powered Weekly Report Automator

An enterprise-grade Streamlit web application designed to automate the generation of complex, highly-formatted Microsoft Word Weekly Training Reports. 

By integrating **Google Gemini AI (2.5-Flash)**, this tool completely eliminates the manual data entry process by reading unstructured instructor PDF modules, extracting the core curriculum data, and allowing administrators to seamlessly edit and format the data before injecting it into a strict corporate `.docx` template.

---

## ✨ Key Features

* **🤖 AI-Powered Document Extraction:** Upload an instructor's 50+ page PDF module, and the app uses Google Gemini AI to instantly extract the *Benefits*, *Learning Objectives*, *Learning Outcomes*, and a detailed *Course Outline*.
* **📊 Interactive Pandas Dataframes:** Review and edit the AI-generated course outline and Action Items directly within the browser using Streamlit's interactive `data_editor`.
* **🖼️ Automated Image Formatting:** Upload raw class photos, and the Python engine will automatically resize them to fit perfectly within standard A4 Word document margins.
* **🛡️ Bulletproof Word Table Generation:** Bypasses Microsoft Word's notorious hidden XML formatting bugs by dynamically drawing Python-native sub-documents (`docxcompose`) and injecting them directly into the template.
* **🌓 Theme Responsive:** Features a custom CSS UI that seamlessly adapts to both Light and Dark modes.

---

## 🛠️ Technology Stack

* **Frontend UI:** [Streamlit](https://streamlit.io/)
* **Data Handling:** [Pandas](https://pandas.pydata.org/)
* **AI Engine:** [Google Generative AI (Gemini)](https://aistudio.google.com/)
* **PDF Extraction:** [PyPDF2](https://pypi.org/project/PyPDF2/)
* **Document Automation:** [docxtpl](https://docxtpl.readthedocs.io/), `python-docx`, `docxcompose`

---
## 🙏 Acknowledgements

* **Management & Team:** Special thanks to the management and R&D team of CMOTD for providing the clear vision, and template structures needed to automate the Weekly Training Reports.
* **[Streamlit](https://streamlit.io/):** For the incredible, interactive web framework.
* **[Google Gemini AI](https://aistudio.google.com/):** For the powerful document extraction and reading capabilities.
* **[docxtpl](https://docxtpl.readthedocs.io/) & [docxcompose](https://pypi.org/project/docxcompose/):** To the open-source developers who made Python-to-Word template automation seamless.

---
*Built with Python, Streamlit, and Google Gemini AI.*

## 🚀 Installation & Local Setup

**1. Clone the repository:**
```bash
git clone [https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git](https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git)
cd YOUR-REPO-NAME