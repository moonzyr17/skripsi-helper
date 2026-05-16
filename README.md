# Skripsi Helper 🎓

AI-powered research assistant untuk membantu mahasiswa Indonesia dari semua jurusan menemukan judul skripsi yang tepat.

![Python](https://img.shields.io/badge/Python-3.11-blue) ![Flask](https://img.shields.io/badge/Flask-3.1-green) ![Groq](https://img.shields.io/badge/AI-Groq%20Llama%203-orange) ![License](https://img.shields.io/badge/License-MIT-yellow)

## 🚀 Demo

**Live:** [https://web-production-6d647.up.railway.app](https://web-production-6d647.up.railway.app)

## ✨ Fitur

- **🎯 Generator Judul** — Generate 10 judul skripsi berdasarkan bidang & keyword via AI
- **🔍 Cek Riset** — Cek penelitian serupa di Semantic Scholar
- **🔬 Saran Metodologi** — Rekomendasi metode, tools, dataset, dan estimasi waktu
- **📝 Outline BAB 1** — Generate latar belakang, rumusan masalah, tujuan, batasan otomatis

## 🎓 Cocok untuk Semua Jurusan

Informatika, Ekonomi, Manajemen, Hukum, Keperawatan, Teknik Sipil, Psikologi, Pendidikan, dan lainnya.

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
| `/api/generate-titles` | POST | Generate 10 judul skripsi |
| `/api/check-research` | POST | Cek penelitian di Semantic Scholar |
| `/api/suggest-methodology` | POST | Saran metodologi |
| `/api/generate-outline` | POST | Generate outline BAB 1 |

## 🤖 Tech Stack

- **Backend**: Flask (Python)
- **AI**: Groq API — Llama Model 3.3 70B
- **Research**: Semantic Scholar API
- **Frontend**: HTML + Tailwind CSS
- **Deploy**: Railway

## Lisensi

MIT License
