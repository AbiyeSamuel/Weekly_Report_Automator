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

## 📖 Quick Start: How to Use the App

Follow these simple steps to generate your first automated Weekly Training Report:

### Step 1: Secure Your AI Access
1. Go to **[Google AI Studio](https://aistudio.google.com/)** and sign in with your Google account.
2. Click **"Get API key"** and copy your free key.
3. *Note: If the system administrator has already configured the Streamlit Secrets vault, the app will securely load the key in the background and you can skip this step!*

### Step 2: The AI Extraction (Sidebar)
1. Look at the **⚙️ AI Assistant** panel on the left sidebar.
2. If prompted, paste your Gemini API Key.
3. Click **"Browse files"** and upload the Instructor's Course Module (PDF).
4. Click the blue **✨ Extract Course Details** button. 
5. Wait about 10–15 seconds. The AI will read the document, extract the core data, and instantly populate the main form for you!

### Step 3: Review & Complete the Form (Main Screen)
1. **General Info:** Fill in the week number, dates, and trainer names.
2. **Review AI Data:** Check the text boxes for *Benefits*, *Objectives*, and *Outcomes*. You can edit these manually if you want to add more details.
3. **Interactive Outline Table:** The AI will build a detailed Topic/Sub-topic table. Click directly into this spreadsheet to edit text, or add/delete rows to match your exact class flow.
4. **Metrics & Observations:** Type out the class attendance, your personal observations, and any Action Items in the provided grids.

### Step 4: Upload Media
1. Scroll down to the **Graphical Media Portfolio Upload** section.
2. Upload **exactly 5 photos** (JPG/PNG) from the training week.
3. Type a short caption for each photo in the boxes provided.

### Step 5: Generate the Document
1. Click the large **🚀 Generate Final Word Document** button at the bottom of the screen.
2. The engine will dynamically draw the tables, resize your photos, and compile the Word document in seconds.
3. Click **📥 Download Final Generated Documentation Report (.docx)** to save the perfectly formatted file to your computer!
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

### 🚀 Admins Can Immediately start using the app with the link 
* **Weekly Report Automator** [WPA](https://weeklyreportautomator-hdzeappkogbdghrjbrvavfv.streamlit.app/)

---
This project was developed by the R&D Team at the **Centre for Marine And Offshore Technology Development (CMOTD)**.

<br>
<img src="CMOTD_LOGO.jpg" alt="CMOTD LOGO" width="400">

---
## 🚀 Installation & Local Setup

**1. Clone the repository:**
```bash
git clone [https://github.com/AbiyeSamuel/Weekly_Report_Automator.git](https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git)
cd YOUR-REPO-NAME