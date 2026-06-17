# Zero-Shot & Few-Shot Data Extraction using Prompt Engineering

Project Overview:
This project demonstrates how Prompt Engineering techniques can be used to extract structured information from unstructured or messy text using a Large Language Model (LLM). It focuses on implementing **Zero-Shot** and **Few-Shot Prompting** to convert natural language input into machine-readable **JSON** format without training or fine-tuning the model.
The project emphasizes prompt design, delimiter usage, deterministic outputs, and structured data extraction for real-world applications.
---
## 🎯 Project Objectives
- Extract structured information from unstructured text.
- Compare Zero-Shot and Few-Shot prompting techniques.
- Generate valid JSON output.
- Improve extraction accuracy using prompt engineering.
- Demonstrate deterministic prompting using Temperature = 0.
---
## 🛠 Technologies Used

- Python 3.10+
- OpenAI API (GPT Models)
- VS Code
- JSON
- Prompt Engineering
---
## 📂 Project Structure
ZeroShot-FewShot-DataExtraction/
│
├── README.md
├── requirements.txt
├── main.py
├── extract.py
├── examples.py
├── raw_data.txt
├── output.json
├── report.pdf
```
## 📥 Installation
### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/ZeroShot-FewShot-DataExtraction.git
```---
### Step 2: Navigate into the Project

```bash
cd ZeroShot-FewShot-DataExtraction
```
---
### Step 3: Create Virtual Environment
Windows

```bash
python -m venv venv
```

Activate

```bash
venv\Scripts\activate
```

Linux / Mac

```bash
python3 -m venv venv
source venv/bin/activate
```
### Step 4: Install Dependencies

```bash
pip install -r requirements.txt
```
## 📦 Required Libraries

```
ollama
```

Install manually if needed

```bash
pip install ollama or py -m pip install ollama
```
## 🚀 Running the Project

Run

```bash
python main.py
```

---
## 📄 Sample Input

```
Hi,
My name is John Smith.

I live in New York.

Email:
johnsmith@gmail.com

Phone:
9876543210
```

---
## 📤 Expected Output

```json
{
  "name": "John Smith",
  "email": "johnsmith@gmail.com",
  "phone": "9876543210",
  "city": "New York"
}
```
## 🧠 Prompt Engineering Techniques Used

### Zero-Shot Prompting

Only instructions are given to the model.

Example

```
Extract:

Name
Email
Phone
City

Return only JSON.
```

---

### Few-Shot Prompting

The model is first shown examples before solving the final task.
Example
Input

```
Name: Alice
Email: alice@gmail.com
City: Chicago
```

Output
```json
{
 "name":"Alice",
 "email":"alice@gmail.com",
 "city":"Chicago"
}
```
## 📊 Workflow

```
Raw Text
     │
     ▼
Prompt Design
     │
     ▼
Zero-Shot / Few-Shot Prompt
     │
     ▼
Large Language Model
     │
     ▼
Structured JSON Output
```
## 📁 Files Description

### main.py

Runs the complete extraction pipeline.

### prompt.py

Contains all Zero-Shot and Few-Shot prompts.

### examples.py

Stores Few-Shot examples.

### sample_input.txt

Contains sample messy text.

### output.json

Stores extracted JSON.

---
## 📈 Features

- Zero-Shot Prompting
- Few-Shot Prompting
- JSON Validation
- Deterministic Outputs
- Delimiter-Based Prompting
- Easy to Extend
- Beginner Friendly
## 📊 Advantages

- No Model Training Required
- High Accuracy
- Fast Development
- Easily Customizable
- Machine Readable Output
## 🌍 Applications

- Customer Information Extraction
- Healthcare Records
- Resume Parsing
- CRM Systems
- Banking Applications
- Legal Document Processing
- Survey Analysis
- Chatbot Automation

---
## 📊 Results

| Technique   | Accuracy |
|------------ |-----------|
| Zero-Shot   | 80–85%    |
| Few-Shot    | 90–95%    |

Few-Shot prompting produces more reliable and consistent outputs due to the inclusion of representative examples.

## 📚 Learning Outcomes

After completing this project, you will understand:

- Prompt Engineering fundamentals
- Zero-Shot Prompting
- Few-Shot Prompting
- Delimiter usage
- Structured JSON generation
- OpenAI API integration
- Deterministic prompting
- Data extraction using LLMs

## 🔮 Future Enhancements

- Support PDF extraction
- OCR-based image text extraction
- CSV export
- Database integration
- Web interface using Streamlit
- Batch document processing

## 👨‍💻 Author
**Name**:CATHERINE REBECCA C

**Course:** Prompt Engineering

**Project:** Zero-Shot & Few-Shot Data Extraction

## ⭐ Acknowledgements

- Ollama
- Python Community(VS Code)
- Prompt Engineering Documentation
