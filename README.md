# 🧾 InvoicePilot AI

**A local-first invoice extraction assistant powered by open-weight AI.**

InvoicePilot AI helps freelancers and small businesses extract structured information from invoices without sending invoice text to a hosted AI API.

## ✨ Features

- Extract invoice details using a locally running AI model.
- Support text-based PDF and TXT invoices.
- Review and edit extracted information.
- Download invoice data as JSON or CSV.
- Keep invoice text processing local using Ollama.

## 🛠️ Tech Stack

- Python
- Streamlit
- Ollama
- Qwen 2.5 3B
- PyMuPDF

## 🚀 Getting Started

### Prerequisites

Install Python, [Ollama](https://ollama.com/download), and Git.

### Installation

```bash
git clone YOUR_REPOSITORY_URL
cd InvoicePilotAI

python -m venv .venv
```

Activate the environment on Windows:

```powershell
.\.venv\Scripts\Activate.ps1
```

Install dependencies:

```bash
pip install streamlit requests pymupdf pillow
```

Download the model:

```bash
ollama pull qwen2.5:3b
```

Run the app:

```bash
streamlit run app.py
```

## 🔒 Why Open Innovation?

Running an open-weight model locally gives users more control over their data, reduces dependence on paid hosted AI APIs, and makes it possible to experiment with different models.

## ⚠️ Current Limitations

- Scanned PDF and image OCR are not implemented.
- Invoice history is not persisted between sessions.
- AI-extracted fields must be verified by the user.

## 🔮 Future Improvements

- OCR for scanned invoices.
- Duplicate invoice detection.
- Payment deadline tracking.
- Persistent invoice history.
- Batch invoice processing.

## 📄 License

MIT License — add a `LICENSE` file before distributing this project under the MIT license.
