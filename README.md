🚀 CriticalInsight Engine
⚖️ AI-Powered Legal Clause Analyzer for Fast, Clear, Risk-Focused Insights

The CriticalInsight Engine automatically scans legal documents, splits them into clean clauses, and uses an advanced LLM (Gemma-2-9B-IT via OpenRouter) to generate:

📝 EXPLANATION – one-sentence, plain-English meaning

⚠️ RISK – high or moderate risks hidden inside the clause

🎯 ACTION – a direct, practical recommendation for the user

It also creates a Critical-Risk Summary so you jump straight to the serious issues without digging through the entire document.



⭐ Key Features

📄 Reads PDF, DOCX, TXT

✂️ Automatic clause detection

🤖 AI-powered Explanation + Risk + Action for each clause

🚫 Filters out non-critical / trivial risks

📊 Clean Pandas dataframe outputs

👨‍⚖️ Ideal for lawyers, founders, reviewers, compliance teams

💻 Works in any Python environment or Google Colab



🛠️ Tech Stack

🐍 Python 3.10+

🔗 OpenRouter API

📘 PyPDF2, python-docx

🧮 Pandas

☁️ Google Colab (optional)



📦 Installation
        pip install python-docx PyPDF2 pandas openai



🔑 Setup Your API Key

Get your OpenRouter key: https://openrouter.ai/

        os.environ["OPENAI_API_KEY"] = "YOUR_KEY"

⚙️ How It Works
1️⃣ Upload a file

Upload a PDF, DOCX, or TXT file when prompted.

2️⃣ Automatic AI processing


The script:

Reads the document

Splits it into clauses

Sends each clause to Gemma-2-9B-IT

Generates EXPLANATION, RISK, ACTION

Builds a structured dataframe

Creates a critical-only dataframe for high-risk issues

3️⃣ Review your results

You’ll get two clear tables:

📘 Full Analysis Table

🚨 Critical Risk Table

📍 Output Example
EXPLANATION: The vendor must complete the work in 30 days.  
RISK: The timeline is strict, and undefined penalties may cause disputes.  
ACTION: Add specific consequences or penalty terms for delay.



📁 Project Structure
CriticalInsight_Engine.ipynb  
│  
├── Document Parser (PDF, DOCX, TXT)  
├── Clause Segmentation Logic  
├── LLM Clause Analyzer  
├── Risk Filtering Engine  
└── Dataframe Output Generator  



🧰 Models & Tools Used

Gemma-2-9B-IT (Google DeepMind)
https://ai.google.dev/gemma

OpenRouter API
https://openrouter.ai/docs




⚠️ Limitations

🖼️ No OCR yet (scanned PDFs won’t work)

⚖️ Not legal advice — automated analysis tool only

🧩 Extremely complex drafting may need manual review

🚀 Future Enhancements

🔍 Add OCR support

🖥️ Gradio UI

📤 Export to Excel/CSV

📚 Multi-document batch analysis

📊 Severity scoring system



📜 License

MIT License — free to use, modify, and improve.
