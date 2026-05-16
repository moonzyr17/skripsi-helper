# Skripsi Helper 🎓

AI-powered research assistant untuk membantu mahasiswa informatika menemukan judul skripsi yang tepat.

![Python](https://img.shields.io/badge/Python-3.11-blue) ![Flask](https://img.shields.io/badge/Flask-3.1-green) ![Groq](https://img.shields.io/badge/AI-Groq%20Llama%203-orange) ![License](https://img.shields.io/badge/License-MIT-yellow)

## ✨ Fitur

- **🎯 Generator Judul** — Generate 5 judul skripsi berdasarkan bidang & keyword via AI
- **🔍 Cek Riset** — Cek penelitian serupa di Semantic Scholar
- **🔬 Saran Metodologi** — Rekomendasi metode, tools, dataset, dan estimasi waktu
- **📝 Outline BAB 1** — Generate latar belakang, rumusan masalah, tujuan, batasan otomatis

## 🚀 Demo

Deploy di Railway — lihat link di bagian About repo.

## 🛠️ Instalasi

```bash
git clone https://github.com/moonzyr17/skripsi-helper.git
cd skripsi-helper

python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

export GROQ_API_KEY=your_groq_api_key
python3 app.py
```

Buka `http://localhost:5000`

## ⚙️ Environment Variables

| Variable | Deskripsi |
|---|---|
| `GROQ_API_KEY` | API key dari [console.groq.com](https://console.groq.com) (gratis) |

## 🔌 API Endpoints

| Endpoint | Method | Deskripsi |
|---|---|---|
| `/` | GET | Halaman utama |
| `/api/generate-titles` | POST | Generate judul skripsi |
| `/api/check-research` | POST | Cek penelitian di Semantic Scholar |
| `/api/suggest-methodology` | POST | Saran metodologi |
| `/api/generate-outline` | POST | Generate outline BAB 1 |

## 🤖 Tech Stack

- **Backend**: Flask (Python)
- **AI**: Groq API — Llama 3.3 70B
- **Research**: Semantic Scholar API
- **Frontend**: HTML + Tailwind CSS
- **Deploy**: Railway

## Lisensi

MIT License
