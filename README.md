# 🧠 InfraMind AI
### Autonomous AI Infrastructure Architect

> **Turn business requirements into deployable cloud infrastructure in seconds.**

InfraMind AI is an AI-powered platform that takes plain-English business requirements and automatically generates cloud architecture, Terraform code, deployment diagrams, scalability plans, and cost estimates — all in one click.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🏗️ **Cloud Architecture Design** | AI-generated component-level architecture for AWS, Azure, and GCP |
| 📊 **Visual Deployment Diagrams** | Auto-rendered Mermaid diagrams showing service flow |
| ⚙️ **Terraform Code Generation** | Production-ready `.tf` files (main, variables, outputs) |
| 💰 **Cost Estimates** | Monthly & yearly breakdown per cloud service |
| 📈 **Scalability Plans** | Stage-wise roadmap (MVP → Growth → Scale) |
| 📁 **Project History** | Save, view, and manage all generated projects |

---

## 🎯 The Problem It Solves

- 🕐 Infrastructure design takes **days** of manual effort
- 💸 Cloud cost estimation is **complex** and **error-prone**
- 📚 Writing Terraform from scratch is **time-consuming**
- 🎨 Architecture diagrams require **separate tools**
- 📈 Scalability planning is often an **afterthought**

**InfraMind AI solves all of this — in seconds.**

---

## 🛠️ Tech Stack

### **Backend**
- **Python 3.11**
- **FastAPI** — high-performance REST API
- **Google Gemini API** — LLM for architecture generation
- **SQLAlchemy + SQLite** — database
- **Pydantic v2** — data validation

### **Frontend**
- **React 18** + **Vite** — modern fast frontend
- **Tailwind CSS** — utility-first styling
- **Framer Motion** — smooth animations
- **Mermaid.js** — architecture diagrams
- **Recharts** — cost breakdown charts
- **Zustand** — state management
- **React Router v6** — routing
- **Axios** — API calls

### **DevOps & Tools**
- Git + GitHub
- Postman (API testing)
- VS Code

---

## 🎬 How It Works

```
┌────────────────────────────────────┐
│  User enters business requirement  │
│  "E-commerce site for 1L users"   │
└──────────────────┬─────────────────┘
                   ↓
┌────────────────────────────────────┐
│   FastAPI Backend receives input   │
└──────────────────┬─────────────────┘
                   ↓
┌────────────────────────────────────┐
│   Gemini LLM analyzes & generates  │
│   structured JSON output           │
└──────────────────┬─────────────────┘
                   ↓
┌────────────────────────────────────┐
│  Architecture  │  Terraform Code   │
│  Diagram       │  Cost Estimate    │
│  Scalability   │  Plan             │
└──────────────────┬─────────────────┘
                   ↓
┌────────────────────────────────────┐
│  Beautiful React UI displays all   │
└────────────────────────────────────┘
```

---

## 🚀 Quick Start

### **Prerequisites**
- Python 3.10+
- Node.js 18+
- Gemini API Key → [Get Free Key](https://aistudio.google.com/app/apikey)

### **1️⃣ Clone the Repository**

```bash
git clone https://github.com/vishakha2121/infra-mind-ai-cloudcraft-ai.git
cd infra-mind-ai-cloudcraft-ai
```

### **2️⃣ Backend Setup**

```bash
cd backend

# Create virtual environment
python -m venv venv

# Activate (Windows)
venv\Scripts\activate

# Activate (Mac/Linux)
# source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Setup environment variables
# Copy .env.example to .env and add your GEMINI_API_KEY

# Run server
uvicorn main:app --reload
```

Backend will run at: **http://localhost:8000**
API Docs: **http://localhost:8000/docs**

### **3️⃣ Frontend Setup**

```bash
cd ../frontend

# Install dependencies
npm install

# Setup environment variables
# Copy .env.example to .env

# Run dev server
npm run dev
```

Frontend will run at: **http://localhost:5173**

---

## 📁 Project Structure

```
infra-mind-ai-cloudcraft-ai/
├── backend/                    # FastAPI backend
│   ├── app/
│   │   ├── api/routes/        # API endpoints
│   │   ├── models/            # Database models
│   │   ├── schemas/           # Pydantic schemas
│   │   ├── services/          # Business logic (AI, Terraform, Cost)
│   │   ├── core/              # Security, logging
│   │   └── utils/             # Helpers
│   ├── database/              # SQLite DB
│   ├── tests/                 # Unit tests
│   ├── main.py                # Entry point
│   ├── config.py              # Config loader
│   └── requirements.txt
│
├── frontend/                   # React frontend
│   ├── src/
│   │   ├── components/        # Reusable UI
│   │   ├── pages/             # Page components
│   │   ├── services/          # API calls
│   │   ├── hooks/             # Custom hooks
│   │   ├── context/           # React context
│   │   └── utils/             # Helpers
│   ├── public/
│   └── package.json
│
├── docs/                       # Documentation
├── README.md
├── .gitignore
└── docker-compose.yml
```

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | App info |
| GET | `/api/health` | Health check |
| POST | `/api/architecture/generate` | Generate cloud architecture |
| POST | `/api/terraform/generate` | Generate Terraform code |
| POST | `/api/cost/estimate` | Estimate cloud costs |
| POST | `/api/diagram/generate` | Generate deployment diagram |
| POST | `/api/generate/full` | Generate everything at once |
| GET | `/api/history` | List all projects |
| GET | `/api/history/{id}` | Get project details |
| DELETE | `/api/history/{id}` | Delete a project |

---

## 📸 Screenshots

> *Coming soon — UI screenshots will be added after frontend is complete.*

---

## 🎯 Use Cases

- 👨‍💻 **Developers** prototyping cloud applications
- 🏢 **Startups** planning MVP infrastructure
- 🎓 **Students** learning cloud architecture
- 📊 **DevOps Engineers** estimating cloud costs
- 🧑‍🏫 **Educators** teaching infrastructure design

---

## 🔮 Future Roadmap

- [ ] Real AWS / Azure / GCP API integration (direct deploy)
- [ ] Multi-user authentication + team workspaces
- [ ] Export as PDF report
- [ ] Kubernetes YAML generation
- [ ] CI/CD pipeline (GitHub Actions) generation
- [ ] Cost comparison across cloud providers
- [ ] Infrastructure drift detection
- [ ] Voice-based requirement input

---

## 🤝 Contributing

This is a personal learning project. Suggestions and feedback are welcome!

---

## 📄 License

This project is licensed under the **MIT License** — free to use for learning and personal projects.

---

## 👤 Author

**Vishakha**
- GitHub: [@vishakha2121](https://github.com/vishakha2121)

---

## ⭐ Show Your Support

If you found this project useful, please give it a ⭐ on GitHub!

---

<div align="center">

**Built with ❤️ using Python, FastAPI, React & Google Gemini**

</div>